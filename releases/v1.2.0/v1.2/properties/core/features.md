# Features (property)

This page documents an [OPTIMADE](https://www.optimade.org/) [Property Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/defs/v1.2/properties/core/features`](https://schemas.optimade.org/defs/v1.2/properties/core/features.md)**  
**Definition name:** `features`

**Property name:** Features  
**Description:** A list of strings that flag which special features are used by the entry.  
**Type:** list  

**Requirements/Conventions:**

- MUST be an empty list if no special features are used.
- MUST be sorted alphabetically.
- If a feature is used, the list MUST contain the corresponding string.
- If a feature is not used, the list MUST NOT contain the corresponding string.
- This is an abstract definition, meant to be inherited by more specific definitions that define specific strings.

**Examples:**

- `['feature1', 'feature2']`

**Formats:** [[JSON](features.json)] [[MD](features.md)]

**JSON definition:**

``` json
{
    "$id": "https://schemas.optimade.org/defs/v1.2/properties/core/features",
    "$schema": "https://schemas.optimade.org/meta/v1.2/optimade/property_definition.json",
    "title": "Features",
    "x-optimade-type": "list",
    "x-optimade-definition": {
        "label": "features_core",
        "kind": "property",
        "version": "1.2.0",
        "format": "1.2",
        "name": "features"
    },
    "type": [
        "array"
    ],
    "x-optimade-dimensions": {
        "names": [
            "dim_features"
        ]
    },
    "description": "A list of strings that flag which special features are used by the entry.\n\n**Requirements/Conventions:**\n\n- MUST be an empty list if no special features are used.\n- MUST be sorted alphabetically.\n- If a feature is used, the list MUST contain the corresponding string.\n- If a feature is not used, the list MUST NOT contain the corresponding string.\n- This is an abstract definition, meant to be inherited by more specific definitions that define specific strings.",
    "examples": [
        [
            "feature1",
            "feature2"
        ]
    ],
    "x-optimade-unit": "inapplicable",
    "items": {
        "type": [
            "string"
        ],
        "x-optimade-type": "string",
        "x-optimade-unit": "inapplicable"
    }
}
```
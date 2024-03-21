# structure features (property)

This page documents an [OPTIMADE](https://www.optimade.org/) [Property Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/defs/v1.2/properties/optimade/structures/structure_features`](https://schemas.optimade.org/defs/v1.2/properties/optimade/structures/structure_features.md)**  
**Definition name:** `structure_features`

**Property name:** structure features  
**Description:** A list of strings that flag which special features are used by the structure.  
**Type:** list  

**Requirements/Conventions:**

- MUST be an empty list if no special features are used.
- MUST be sorted alphabetically.
- If a special feature listed below is used, the list MUST contain the corresponding string.
- If a special feature listed below is not used, the list MUST NOT contain the corresponding string.
- **List of strings used to indicate special structure features:**

    - `disorder`: this flag MUST be present if any one entry in the species list has a `chemical_symbols` list that is longer than 1 element.
    - `implicit_atoms`: this flag MUST be present if the structure contains atoms that are not assigned to sites via the property `species_at_sites` (e.g., because their positions are unknown). When this flag is present, the properties related to the chemical formula will likely not match the type and count of atoms represented by the `species_at_sites`, `species`, and `assemblies` properties.
    - `site_attachments`: this flag MUST be present if any one entry in the species list includes `attached` and `nattached`.
    - `assemblies`: this flag MUST be present if the property assemblies is present.

**Explained examples**:

- A structure having implicit atoms and using assemblies: `["assemblies", "implicit_atoms"]`

**Examples:**

- `["assemblies", "implicit_atoms"]`

**Formats:** [[JSON](structure_features.json)] [[MD](structure_features.md)]

**JSON definition:**

``` json
{
    "$id": "https://schemas.optimade.org/defs/v1.2/properties/optimade/structures/structure_features",
    "$schema": "https://schemas.optimade.org/meta/v1.2/optimade/property_definition.json",
    "title": "structure features",
    "x-optimade-definition": {
        "label": "structure_features_optimade_structures",
        "kind": "property",
        "version": "1.2.0",
        "format": "1.2",
        "name": "structure_features"
    },
    "description": "A list of strings that flag which special features are used by the structure.\n\n**Requirements/Conventions:**\n\n- MUST be an empty list if no special features are used.\n- MUST be sorted alphabetically.\n- If a special feature listed below is used, the list MUST contain the corresponding string.\n- If a special feature listed below is not used, the list MUST NOT contain the corresponding string.\n- **List of strings used to indicate special structure features:**\n\n    - `disorder`: this flag MUST be present if any one entry in the species list has a `chemical_symbols` list that is longer than 1 element.\n    - `implicit_atoms`: this flag MUST be present if the structure contains atoms that are not assigned to sites via the property `species_at_sites` (e.g., because their positions are unknown). When this flag is present, the properties related to the chemical formula will likely not match the type and count of atoms represented by the `species_at_sites`, `species`, and `assemblies` properties.\n    - `site_attachments`: this flag MUST be present if any one entry in the species list includes `attached` and `nattached`.\n    - `assemblies`: this flag MUST be present if the property assemblies is present.\n\n**Explained examples**:\n\n- A structure having implicit atoms and using assemblies: `[\"assemblies\", \"implicit_atoms\"]`",
    "examples": [
        [
            "assemblies",
            "implicit_atoms"
        ]
    ],
    "x-optimade-type": "list",
    "type": [
        "array"
    ],
    "x-optimade-dimensions": {
        "names": [
            "dim_features"
        ]
    },
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
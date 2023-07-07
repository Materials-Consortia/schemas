# annote (property)

This page documents an [OPTIMADE](https://www.optimade.org/) [Property Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/defs/v1.2/properties/optimade/references/annote`](https://schemas.optimade.org/defs/v1.2/properties/optimade/references/annote.md)**  
**Definition name:** `annote`

**Property name:** annote  
**Description:** Additional notes or comments on the reference (the annote field in the BibTeX specification).  
**Type:** string  



**Examples:**

- `This article obtains structures via density-functional theory.`

**Formats:** [[JSON](annote.json)] [[MD](annote.md)]

**JSON definition:**

``` json
{
    "$schema": "https://schemas.optimade.org/meta/v1.2/optimade/property_definition.md",
    "$id": "https://schemas.optimade.org/defs/v1.2/properties/optimade/references/annote",
    "title": "annote",
    "x-optimade-type": "string",
    "x-optimade-definition": {
        "kind": "property",
        "version": "1.2.0",
        "format": "1.2",
        "name": "annote"
    },
    "type": [
        "string",
        "null"
    ],
    "description": "Additional notes or comments on the reference (the annote field in the BibTeX specification).",
    "examples": [
        "This article obtains structures via density-functional theory."
    ],
    "x-optimade-unit": "inapplicable"
}
```
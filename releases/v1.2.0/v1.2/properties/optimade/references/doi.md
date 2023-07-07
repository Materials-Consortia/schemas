# doi (property)

This page documents an [OPTIMADE](https://www.optimade.org/) [Property Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/defs/v1.2/properties/optimade/references/doi`](https://schemas.optimade.org/defs/v1.2/properties/optimade/references/doi.md)**  
**Definition name:** `doi`

**Property name:** doi  
**Description:** The doi identifier of the object being referenced.  
**Type:** string  



**Examples:**

- `10.1103/PhysRev.136.B864`

**Formats:** [[JSON](doi.json)] [[MD](doi.md)]

**JSON definition:**

``` json
{
    "$schema": "https://schemas.optimade.org/meta/v1.2/optimade/property_definition.md",
    "$id": "https://schemas.optimade.org/defs/v1.2/properties/optimade/references/doi",
    "title": "doi",
    "x-optimade-type": "string",
    "x-optimade-definition": {
        "kind": "property",
        "version": "1.2.0",
        "format": "1.2",
        "name": "doi"
    },
    "type": [
        "string",
        "null"
    ],
    "description": "The doi identifier of the object being referenced.",
    "examples": [
        "10.1103/PhysRev.136.B864"
    ],
    "x-optimade-unit": "inapplicable"
}
```
# key (property)
This page documents an [OPTIMADE](https://www.optimade.org/) [Property Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/properties/v1.2.0/optimade/references/key`](https://schemas.optimade.org/properties/v1.2.0/optimade/references/key)**  
**Definition name:** `key`

**Property name:** key  
**Description:** Used for alphabetizing, cross-referencing, and creating a label (the key field in the BibTeX specification).  
**Type:** string  



**Examples:**

- `smith2022`

**Formats:** [[JSON](key.json)] [[MD](key.md)]

**JSON definition:**

``` json
{
    "$id": "https://schemas.optimade.org/properties/v1.2.0/optimade/references/key",
    "title": "key",
    "x-optimade-type": "string",
    "x-optimade-definition": {
        "kind": "property",
        "version": "1.2.0",
        "format": "1.2",
        "name": "key"
    },
    "type": [
        "string",
        "null"
    ],
    "description": "Used for alphabetizing, cross-referencing, and creating a label (the key field in the BibTeX specification).",
    "examples": [
        "smith2022"
    ],
    "x-optimade-unit": "inapplicable",
    "$schema": "https://schemas.optimade.org/meta/v1.2.0/optimade/property_definition.md"
}
```
# edition (property)

This page documents an [OPTIMADE](https://www.optimade.org/) [Property Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/defs/v1.2/properties/optimade/references/edition`](https://schemas.optimade.org/defs/v1.2/properties/optimade/references/edition.md)**  
**Definition name:** `edition`

**Property name:** edition  
**Description:** The edition of a book (the edition field in the BibTeX specification).  
**Type:** string  



**Examples:**

- `Second`

**Formats:** [[JSON](edition.json)] [[MD](edition.md)]

**JSON definition:**

``` json
{
    "$schema": "https://schemas.optimade.org/meta/v1.2/optimade/property_definition.md",
    "$id": "https://schemas.optimade.org/defs/v1.2/properties/optimade/references/edition",
    "title": "edition",
    "x-optimade-type": "string",
    "x-optimade-definition": {
        "kind": "property",
        "version": "1.2.0",
        "format": "1.2",
        "name": "edition"
    },
    "type": [
        "string",
        "null"
    ],
    "description": "The edition of a book (the edition field in the BibTeX specification).",
    "examples": [
        "Second"
    ],
    "x-optimade-unit": "inapplicable"
}
```
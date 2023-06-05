# chapter (property)
This page documents an [OPTIMADE](https://www.optimade.org/) [Property Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/properties/v1.2.0/optimade/references/chapter`](https://schemas.optimade.org/properties/v1.2.0/optimade/references/chapter)**  
**Definition name:** `chapter`

**Property name:** chapter  
**Description:** The chapter, section, or similar part number (the chapter field in the BibTeX specification).  
**Type:** string  



**Examples:**

- `5`

**Formats:** [[JSON](chapter.json)] [[MD](chapter.md)]

**JSON definition:**

``` json
{
    "$id": "https://schemas.optimade.org/properties/v1.2.0/optimade/references/chapter",
    "title": "chapter",
    "x-optimade-type": "string",
    "x-optimade-definition": {
        "kind": "property",
        "version": "1.2.0",
        "format": "1.2",
        "name": "chapter"
    },
    "type": [
        "string",
        "null"
    ],
    "description": "The chapter, section, or similar part number (the chapter field in the BibTeX specification).",
    "examples": [
        "5"
    ],
    "x-optimade-unit": "inapplicable",
    "$schema": "https://schemas.optimade.org/meta/v1.2.0/optimade/property_definition.md"
}
```
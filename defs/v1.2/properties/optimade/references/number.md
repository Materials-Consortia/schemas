# number (property)

This page documents an [OPTIMADE](https://www.optimade.org/) [Property Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/defs/v1.2/properties/optimade/references/number`](https://schemas.optimade.org/defs/v1.2/properties/optimade/references/number)**  
**Definition name:** `number`

**Property name:** number  
**Description:** The number of a journal, magazine, technical report, or work in a series (the number field in the BibTeX specification).  
**Type:** string  



**Examples:**

- `3`

**Formats:** [[JSON](number.json)] [[MD](number.md)]

**JSON definition:**

``` json
{
    "$schema": "https://schemas.optimade.org/meta/v1.2/optimade/property_definition.md",
    "$id": "https://schemas.optimade.org/defs/v1.2/properties/optimade/references/number",
    "title": "number",
    "x-optimade-type": "string",
    "x-optimade-definition": {
        "kind": "property",
        "version": "1.2.0",
        "format": "1.2",
        "name": "number"
    },
    "type": [
        "string",
        "null"
    ],
    "description": "The number of a journal, magazine, technical report, or work in a series (the number field in the BibTeX specification).",
    "examples": [
        "3"
    ],
    "x-optimade-unit": "inapplicable"
}
```
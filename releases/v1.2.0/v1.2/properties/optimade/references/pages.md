# pages (property)

This page documents an [OPTIMADE](https://www.optimade.org/) [Property Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/defs/v1.2/properties/optimade/references/pages`](https://schemas.optimade.org/defs/v1.2/properties/optimade/references/pages.md)**  
**Definition name:** `pages`

**Property name:** pages  
**Description:** The page number(s) of the reference (the pages field in the BibTeX specification).  
**Type:** string  



**Examples:**

- `147--154`

**Formats:** [[JSON](pages.json)] [[MD](pages.md)]

**JSON definition:**

``` json
{
    "$id": "https://schemas.optimade.org/defs/v1.2/properties/optimade/references/pages",
    "$schema": "https://schemas.optimade.org/meta/v1.2/optimade/property_definition.json",
    "title": "pages",
    "x-optimade-type": "string",
    "x-optimade-definition": {
        "label": "pages_optimade_references",
        "kind": "property",
        "version": "1.2.0",
        "format": "1.2",
        "name": "pages"
    },
    "type": [
        "string",
        "null"
    ],
    "description": "The page number(s) of the reference (the pages field in the BibTeX specification).",
    "examples": [
        "147--154"
    ],
    "x-optimade-unit": "inapplicable"
}
```
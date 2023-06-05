# pages (property)
This page documents an [OPTIMADE](https://www.optimade.org/) [Property Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/properties/v1.2.0/optimade/references/pages`](https://schemas.optimade.org/properties/v1.2.0/optimade/references/pages)**  
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
    "$id": "https://schemas.optimade.org/properties/v1.2.0/optimade/references/pages",
    "title": "pages",
    "x-optimade-type": "string",
    "x-optimade-definition": {
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
    "x-optimade-unit": "inapplicable",
    "$schema": "https://schemas.optimade.org/meta/v1.2.0/optimade/property_definition.md"
}
```
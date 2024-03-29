# title (property)

This page documents an [OPTIMADE](https://www.optimade.org/) [Property Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/defs/v1.2/properties/optimade/references/title`](https://schemas.optimade.org/defs/v1.2/properties/optimade/references/title.md)**  
**Definition name:** `title`

**Property name:** title  
**Description:** The title of the work (the title field in the BibTeX specification).  
**Type:** string  



**Examples:**

- `"A Study on the Effects of Sleep Deprivation on Cognitive Performance"`

**Formats:** [[JSON](title.json)] [[MD](title.md)]

**JSON definition:**

``` json
{
    "$id": "https://schemas.optimade.org/defs/v1.2/properties/optimade/references/title",
    "$schema": "https://schemas.optimade.org/meta/v1.2/optimade/property_definition.json",
    "title": "title",
    "x-optimade-type": "string",
    "x-optimade-definition": {
        "label": "title_optimade_references",
        "kind": "property",
        "version": "1.2.0",
        "format": "1.2",
        "name": "title"
    },
    "type": [
        "string",
        "null"
    ],
    "description": "The title of the work (the title field in the BibTeX specification).",
    "examples": [
        "A Study on the Effects of Sleep Deprivation on Cognitive Performance"
    ],
    "x-optimade-unit": "inapplicable"
}
```
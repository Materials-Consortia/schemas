# series (property)

This page documents an [OPTIMADE](https://www.optimade.org/) [Property Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/defs/v1.2/properties/optimade/references/series`](https://schemas.optimade.org/defs/v1.2/properties/optimade/references/series.md)**  
**Definition name:** `series`

**Property name:** series  
**Description:** The name of a series or set of books (the series field in the BibTeX specification).  
**Type:** string  



**Examples:**

- `Lecture Notes in Computer Science`

**Formats:** [[JSON](series.json)] [[MD](series.md)]

**JSON definition:**

``` json
{
    "$schema": "https://schemas.optimade.org/meta/v1.2/optimade/property_definition.md",
    "$id": "https://schemas.optimade.org/defs/v1.2/properties/optimade/references/series",
    "title": "series",
    "x-optimade-type": "string",
    "x-optimade-definition": {
        "label": "series_optimade_references",
        "kind": "property",
        "version": "1.2.0",
        "format": "1.2",
        "name": "series"
    },
    "type": [
        "string",
        "null"
    ],
    "description": "The name of a series or set of books (the series field in the BibTeX specification).",
    "examples": [
        "Lecture Notes in Computer Science"
    ],
    "x-optimade-unit": "inapplicable"
}
```
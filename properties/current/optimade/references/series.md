# series (property)
This page documents an [OPTIMADE](https://www.optimade.org/) [Property Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/properties/v1.2.0/optimade/references/series`](https://schemas.optimade.org/properties/v1.2.0/optimade/references/series)**  
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
    "$id": "https://schemas.optimade.org/properties/v1.2.0/optimade/references/series",
    "title": "series",
    "x-optimade-type": "string",
    "x-optimade-definition": {
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
    "x-optimade-unit": "inapplicable",
    "$schema": "https://schemas.optimade.org/meta/v1.2.0/optimade/property_definition.md"
}
```
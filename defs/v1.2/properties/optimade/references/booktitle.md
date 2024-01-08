# booktitle (property)

This page documents an [OPTIMADE](https://www.optimade.org/) [Property Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/defs/v1.2/properties/optimade/references/booktitle`](https://schemas.optimade.org/defs/v1.2/properties/optimade/references/booktitle.md)**  
**Definition name:** `booktitle`

**Property name:** booktitle  
**Description:** The title of a book being cited; for parts of a book, use the title field instead (the booktitle field in the BibTeX specification).  
**Type:** string  



**Examples:**

- `Density-functional Theory of Atoms and Molecules`

**Formats:** [[JSON](booktitle.json)] [[MD](booktitle.md)]

**JSON definition:**

``` json
{
    "$schema": "https://schemas.optimade.org/meta/v1.2/optimade/property_definition.md",
    "$id": "https://schemas.optimade.org/defs/v1.2/properties/optimade/references/booktitle",
    "title": "booktitle",
    "x-optimade-type": "string",
    "x-optimade-definition": {
        "label": "booktitle_optimade_references",
        "kind": "property",
        "version": "1.2.0",
        "format": "1.2",
        "name": "booktitle"
    },
    "type": [
        "string",
        "null"
    ],
    "description": "The title of a book being cited; for parts of a book, use the title field instead (the booktitle field in the BibTeX specification).",
    "examples": [
        "Density-functional Theory of Atoms and Molecules"
    ],
    "x-optimade-unit": "inapplicable"
}
```
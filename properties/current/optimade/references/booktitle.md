# booktitle (property)
This page documents an [OPTIMADE](https://www.optimade.org/) [Property Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/properties/v1.2.0/optimade/references/booktitle`](https://schemas.optimade.org/properties/v1.2.0/optimade/references/booktitle)**  
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
    "$id": "https://schemas.optimade.org/properties/v1.2.0/optimade/references/booktitle",
    "title": "booktitle",
    "x-optimade-type": "string",
    "x-optimade-definition": {
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
    "x-optimade-unit": "inapplicable",
    "$schema": "https://schemas.optimade.org/meta/v1.2.0/optimade/property_definition.md"
}
```
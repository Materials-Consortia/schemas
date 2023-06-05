# crossref (property)
This page documents an [OPTIMADE](https://www.optimade.org/) [Property Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/properties/v1.2.0/optimade/references/crossref`](https://schemas.optimade.org/properties/v1.2.0/optimade/references/crossref)**  
**Definition name:** `crossref`

**Property name:** crossref  
**Description:** The database key of the entry being cross referenced (the crossref field in the BibTeX specification).  
**Type:** string  



**Examples:**

- `smith2022`

**Formats:** [[JSON](crossref.json)] [[MD](crossref.md)]

**JSON definition:**

``` json
{
    "$id": "https://schemas.optimade.org/properties/v1.2.0/optimade/references/crossref",
    "title": "crossref",
    "x-optimade-type": "string",
    "x-optimade-definition": {
        "kind": "property",
        "version": "1.2.0",
        "format": "1.2",
        "name": "crossref"
    },
    "type": [
        "string",
        "null"
    ],
    "description": "The database key of the entry being cross referenced (the crossref field in the BibTeX specification).",
    "examples": [
        "smith2022"
    ],
    "x-optimade-unit": "inapplicable",
    "$schema": "https://schemas.optimade.org/meta/v1.2.0/optimade/property_definition.md"
}
```
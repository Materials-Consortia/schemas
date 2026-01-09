# how published (property)

This page documents an [OPTIMADE](https://www.optimade.org/) [Property Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/defs/v1.2/properties/optimade/references/howpublished`](https://schemas.optimade.org/defs/v1.2/properties/optimade/references/howpublished.md)**  
**Definition name:** `howpublished`

**Property name:** how published  
**Description:** The method of publication (the howpublished field in the BibTeX specification)  
**Type:** string  



**Examples:**

- `"\\url{https://www.example.com/papers/example_paper}"`

**Formats:** [[JSON](howpublished.json)] [[MD](howpublished.md)]

**JSON definition:**

``` json
{
    "$id": "https://schemas.optimade.org/defs/v1.2/properties/optimade/references/howpublished",
    "$schema": "https://schemas.optimade.org/meta/v1.2/optimade/property_definition.json",
    "title": "how published",
    "x-optimade-type": "string",
    "x-optimade-definition": {
        "label": "howpublished_optimade_references",
        "kind": "property",
        "version": "1.2.0",
        "format": "1.2",
        "name": "howpublished"
    },
    "type": [
        "string",
        "null"
    ],
    "description": "The method of publication (the howpublished field in the BibTeX specification)",
    "examples": [
        "\\url{https://www.example.com/papers/example_paper}"
    ],
    "x-optimade-unit": "inapplicable"
}
```
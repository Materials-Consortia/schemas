# publisher (property)

This page documents an [OPTIMADE](https://www.optimade.org/) [Property Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/defs/v1.2/properties/optimade/references/publisher`](https://schemas.optimade.org/defs/v1.2/properties/optimade/references/publisher.md)**  
**Definition name:** `publisher`

**Property name:** publisher  
**Description:** The name of the publisher (the publisher field in the BibTeX specification).  
**Type:** string  



**Examples:**

- `ACM`

**Formats:** [[JSON](publisher.json)] [[MD](publisher.md)]

**JSON definition:**

``` json
{
    "$id": "https://schemas.optimade.org/defs/v1.2/properties/optimade/references/publisher",
    "$schema": "https://schemas.optimade.org/meta/v1.2/optimade/property_definition.json",
    "title": "publisher",
    "x-optimade-type": "string",
    "x-optimade-definition": {
        "label": "publisher_optimade_references",
        "kind": "property",
        "version": "1.2.0",
        "format": "1.2",
        "name": "publisher"
    },
    "type": [
        "string",
        "null"
    ],
    "description": "The name of the publisher (the publisher field in the BibTeX specification).",
    "examples": [
        "ACM"
    ],
    "x-optimade-unit": "inapplicable"
}
```
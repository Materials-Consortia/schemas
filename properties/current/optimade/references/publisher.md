# publisher (property)
This page documents an [OPTIMADE](https://www.optimade.org/) [Property Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/properties/v1.2.0/optimade/references/publisher`](https://schemas.optimade.org/properties/v1.2.0/optimade/references/publisher)**  
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
    "$id": "https://schemas.optimade.org/properties/v1.2.0/optimade/references/publisher",
    "title": "publisher",
    "x-optimade-type": "string",
    "x-optimade-definition": {
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
    "x-optimade-unit": "inapplicable",
    "$schema": "https://schemas.optimade.org/meta/v1.2.0/optimade/property_definition.md"
}
```
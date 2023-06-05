# address (property)
This page documents an [OPTIMADE](https://www.optimade.org/) [Property Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/properties/v1.2.0/optimade/references/address`](https://schemas.optimade.org/properties/v1.2.0/optimade/references/address)**  
**Definition name:** `address`

**Property name:** address  
**Description:** Typically the location of the publisher or institution (the address field in the BibTeX specification).  
**Type:** string  



**Examples:**

- `New York, NY`

**Formats:** [[JSON](address.json)] [[MD](address.md)]

**JSON definition:**

``` json
{
    "$id": "https://schemas.optimade.org/properties/v1.2.0/optimade/references/address",
    "title": "address",
    "x-optimade-type": "string",
    "x-optimade-definition": {
        "kind": "property",
        "version": "1.2.0",
        "format": "1.2",
        "name": "address"
    },
    "type": [
        "string",
        "null"
    ],
    "description": "Typically the location of the publisher or institution (the address field in the BibTeX specification).",
    "examples": [
        "New York, NY"
    ],
    "x-optimade-unit": "inapplicable",
    "$schema": "https://schemas.optimade.org/meta/v1.2.0/optimade/property_definition.md"
}
```
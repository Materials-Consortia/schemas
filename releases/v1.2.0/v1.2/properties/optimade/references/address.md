# address (property)

This page documents an [OPTIMADE](https://www.optimade.org/) [Property Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/defs/v1.2/properties/optimade/references/address`](https://schemas.optimade.org/defs/v1.2/properties/optimade/references/address.md)**  
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
    "$schema": "https://schemas.optimade.org/meta/v1.2/optimade/property_definition.md",
    "$id": "https://schemas.optimade.org/defs/v1.2/properties/optimade/references/address",
    "title": "address",
    "x-optimade-type": "string",
    "x-optimade-definition": {
        "label": "address_optimade_references",
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
    "x-optimade-unit": "inapplicable"
}
```
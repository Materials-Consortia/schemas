# year (property)

This page documents an [OPTIMADE](https://www.optimade.org/) [Property Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/defs/v1.2/properties/optimade/references/year`](https://schemas.optimade.org/defs/v1.2/properties/optimade/references/year.md)**  
**Definition name:** `year`

**Property name:** year  
**Description:** The year of publication or writing.  
**Type:** string  



**Examples:**

- `1984`

**Formats:** [[JSON](year.json)] [[MD](year.md)]

**JSON definition:**

``` json
{
    "$schema": "https://schemas.optimade.org/meta/v1.2/optimade/property_definition.md",
    "$id": "https://schemas.optimade.org/defs/v1.2/properties/optimade/references/year",
    "title": "year",
    "x-optimade-type": "string",
    "x-optimade-definition": {
        "kind": "property",
        "version": "1.2.0",
        "format": "1.2",
        "name": "year"
    },
    "type": [
        "string",
        "null"
    ],
    "description": "The year of publication or writing.",
    "examples": [
        "1984"
    ],
    "x-optimade-unit": "inapplicable"
}
```
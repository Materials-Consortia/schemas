# year (property)
This page documents an [OPTIMADE](https://www.optimade.org/) [Property Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/properties/v1.2.0/optimade/references/year`](https://schemas.optimade.org/properties/v1.2.0/optimade/references/year)**  
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
    "$id": "https://schemas.optimade.org/properties/v1.2.0/optimade/references/year",
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
    "x-optimade-unit": "inapplicable",
    "$schema": "https://schemas.optimade.org/meta/v1.2.0/optimade/property_definition.md"
}
```
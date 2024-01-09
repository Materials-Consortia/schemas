# month (property)

This page documents an [OPTIMADE](https://www.optimade.org/) [Property Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/defs/v1.2/properties/optimade/references/month`](https://schemas.optimade.org/defs/v1.2/properties/optimade/references/month.md)**  
**Definition name:** `month`

**Property name:** month  
**Description:** The three letter abbreviation of the month of publication or writing (the month field in the BibTeX specification).  
**Type:** string  



**Examples:**

- `jul`

**Formats:** [[JSON](month.json)] [[MD](month.md)]

**JSON definition:**

``` json
{
    "$id": "https://schemas.optimade.org/defs/v1.2/properties/optimade/references/month",
    "$schema": "https://schemas.optimade.org/meta/v1.2/optimade/property_definition.json",
    "title": "month",
    "x-optimade-type": "string",
    "x-optimade-definition": {
        "label": "month_optimade_references",
        "kind": "property",
        "version": "1.2.0",
        "format": "1.2",
        "name": "month"
    },
    "type": [
        "string",
        "null"
    ],
    "description": "The three letter abbreviation of the month of publication or writing (the month field in the BibTeX specification).",
    "examples": [
        "jul"
    ],
    "x-optimade-unit": "inapplicable"
}
```
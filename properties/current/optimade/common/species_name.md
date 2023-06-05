# Name of the species (property)
This page documents an [OPTIMADE](https://www.optimade.org/) [Property Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/properties/v1.2.0/optimade/common/species_name`](https://schemas.optimade.org/properties/v1.2.0/optimade/common/species_name)**  
**Definition name:** `species_name`

**Property name:** Name of the species  
**Description:** The name of the species.  
**Type:** string  



**Examples:**

- `Na`
- `Si[32982]`
- `quop`

**Formats:** [[JSON](species_name.json)] [[MD](species_name.md)]

**JSON definition:**

``` json
{
    "$id": "https://schemas.optimade.org/properties/v1.2.0/optimade/common/species_name",
    "title": "Name of the species",
    "x-optimade-type": "string",
    "x-optimade-definition": {
        "kind": "property",
        "version": "1.2.0",
        "format": "1.2",
        "name": "species_name"
    },
    "type": [
        "string"
    ],
    "description": "The name of the species.",
    "examples": [
        "Na",
        "Si[32982]",
        "quop"
    ],
    "x-optimade-unit": "inapplicable",
    "$schema": "https://schemas.optimade.org/meta/v1.2.0/optimade/property_definition.md"
}
```
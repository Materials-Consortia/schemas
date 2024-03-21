# description (property)

This page documents an [OPTIMADE](https://www.optimade.org/) [Property Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/defs/v1.2/properties/optimade/files/description`](https://schemas.optimade.org/defs/v1.2/properties/optimade/files/description.md)**  
**Definition name:** `description`

**Property name:** description  
**Description:** Free-form description of a file.  
**Type:** string  



**Examples:**

- `POSCAR format file`

**Formats:** [[JSON](description.json)] [[MD](description.md)]

**JSON definition:**

``` json
{
    "$id": "https://schemas.optimade.org/defs/v1.2/properties/optimade/files/description",
    "$schema": "https://schemas.optimade.org/meta/v1.2/optimade/property_definition.json",
    "title": "description",
    "x-optimade-type": "string",
    "x-optimade-definition": {
        "label": "description_optimade_files",
        "kind": "property",
        "version": "1.2.0",
        "format": "1.2",
        "name": "description"
    },
    "type": [
        "string",
        "null"
    ],
    "description": "Free-form description of a file.",
    "examples": [
        "POSCAR format file"
    ],
    "x-optimade-unit": "inapplicable"
}
```
# volume (property)

This page documents an [OPTIMADE](https://www.optimade.org/) [Property Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/defs/v1.2/properties/optimade/references/volume`](https://schemas.optimade.org/defs/v1.2/properties/optimade/references/volume.md)**  
**Definition name:** `volume`

**Property name:** volume  
**Description:** The volume number of a journal or multivolume book (the volume field in the BibTeX specification).  
**Type:** string  



**Examples:**

- `14`

**Formats:** [[JSON](volume.json)] [[MD](volume.md)]

**JSON definition:**

``` json
{
    "$schema": "https://schemas.optimade.org/meta/v1.2/optimade/property_definition.md",
    "$id": "https://schemas.optimade.org/defs/v1.2/properties/optimade/references/volume",
    "title": "volume",
    "x-optimade-type": "string",
    "x-optimade-definition": {
        "kind": "property",
        "version": "1.2.0",
        "format": "1.2",
        "name": "volume"
    },
    "type": [
        "string",
        "null"
    ],
    "description": "The volume number of a journal or multivolume book (the volume field in the BibTeX specification).",
    "examples": [
        "14"
    ],
    "x-optimade-unit": "inapplicable"
}
```
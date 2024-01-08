# note (property)

This page documents an [OPTIMADE](https://www.optimade.org/) [Property Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/defs/v1.2/properties/optimade/references/note`](https://schemas.optimade.org/defs/v1.2/properties/optimade/references/note.md)**  
**Definition name:** `note`

**Property name:** note  
**Description:** Additional information about the reference (the note field in the BibTeX specification).  
**Type:** string  



**Examples:**

- `Accessed: 2022-11-04`

**Formats:** [[JSON](note.json)] [[MD](note.md)]

**JSON definition:**

``` json
{
    "$schema": "https://schemas.optimade.org/meta/v1.2/optimade/property_definition.md",
    "$id": "https://schemas.optimade.org/defs/v1.2/properties/optimade/references/note",
    "title": "note",
    "x-optimade-type": "string",
    "x-optimade-definition": {
        "label": "note_optimade_references",
        "kind": "property",
        "version": "1.2.0",
        "format": "1.2",
        "name": "note"
    },
    "type": [
        "string",
        "null"
    ],
    "description": "Additional information about the reference (the note field in the BibTeX specification).",
    "examples": [
        "Accessed: 2022-11-04"
    ],
    "x-optimade-unit": "inapplicable"
}
```
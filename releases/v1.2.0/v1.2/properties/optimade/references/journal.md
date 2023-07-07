# journal (property)

This page documents an [OPTIMADE](https://www.optimade.org/) [Property Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/defs/v1.2/properties/optimade/references/journal`](https://schemas.optimade.org/defs/v1.2/properties/optimade/references/journal.md)**  
**Definition name:** `journal`

**Property name:** journal  
**Description:** The name of a journal (the journal field in the BibTeX specification).  
**Type:** string  



**Examples:**

- `Journal of Environmental Science`

**Formats:** [[JSON](journal.json)] [[MD](journal.md)]

**JSON definition:**

``` json
{
    "$schema": "https://schemas.optimade.org/meta/v1.2/optimade/property_definition.md",
    "$id": "https://schemas.optimade.org/defs/v1.2/properties/optimade/references/journal",
    "title": "journal",
    "x-optimade-type": "string",
    "x-optimade-definition": {
        "kind": "property",
        "version": "1.2.0",
        "format": "1.2",
        "name": "journal"
    },
    "type": [
        "string",
        "null"
    ],
    "description": "The name of a journal (the journal field in the BibTeX specification).",
    "examples": [
        "Journal of Environmental Science"
    ],
    "x-optimade-unit": "inapplicable"
}
```
# institution (property)

This page documents an [OPTIMADE](https://www.optimade.org/) [Property Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/defs/v1.2/properties/optimade/references/institution`](https://schemas.optimade.org/defs/v1.2/properties/optimade/references/institution.md)**  
**Definition name:** `institution`

**Property name:** institution  
**Description:** The sponsoring institution of a technical report (the institution field in the BibTeX specification).  
**Type:** string  



**Examples:**

- `"Massachusetts Institute of Technology"`

**Formats:** [[JSON](institution.json)] [[MD](institution.md)]

**JSON definition:**

``` json
{
    "$id": "https://schemas.optimade.org/defs/v1.2/properties/optimade/references/institution",
    "$schema": "https://schemas.optimade.org/meta/v1.2/optimade/property_definition.json",
    "title": "institution",
    "x-optimade-type": "string",
    "x-optimade-definition": {
        "label": "institution_optimade_references",
        "kind": "property",
        "version": "1.2.0",
        "format": "1.2",
        "name": "institution"
    },
    "type": [
        "string",
        "null"
    ],
    "description": "The sponsoring institution of a technical report (the institution field in the BibTeX specification).",
    "examples": [
        "Massachusetts Institute of Technology"
    ],
    "x-optimade-unit": "inapplicable"
}
```
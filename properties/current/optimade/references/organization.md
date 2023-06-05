# organization (property)
This page documents an [OPTIMADE](https://www.optimade.org/) [Property Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/properties/v1.2.0/optimade/references/organization`](https://schemas.optimade.org/properties/v1.2.0/optimade/references/organization)**  
**Definition name:** `organization`

**Property name:** organization  
**Description:** The organization sponsoring a conference or publishing a manual (the organization field in the BibTeX specification)  
**Type:** string  



**Examples:**

- `International Association of Engineers`

**Formats:** [[JSON](organization.json)] [[MD](organization.md)]

**JSON definition:**

``` json
{
    "$id": "https://schemas.optimade.org/properties/v1.2.0/optimade/references/organization",
    "title": "organization",
    "x-optimade-type": "string",
    "x-optimade-definition": {
        "kind": "property",
        "version": "1.2.0",
        "format": "1.2",
        "name": "organization"
    },
    "type": [
        "string",
        "null"
    ],
    "description": "The organization sponsoring a conference or publishing a manual (the organization field in the BibTeX specification)",
    "examples": [
        "International Association of Engineers"
    ],
    "x-optimade-unit": "inapplicable",
    "$schema": "https://schemas.optimade.org/meta/v1.2.0/optimade/property_definition.md"
}
```
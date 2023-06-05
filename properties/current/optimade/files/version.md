# Version (property)
This page documents an [OPTIMADE](https://www.optimade.org/) [Property Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/properties/v1.2.0/optimade/files/version`](https://schemas.optimade.org/properties/v1.2.0/optimade/files/version)**  
**Definition name:** `version`

**Property name:** Version  
**Description:** Version information of a file (e.g. commit, revision, timestamp).  
**Type:** string  

**Requirements/Conventions:**

- If provided, it MUST be guaranteed that file contents pertaining to the same combination of id and version are the same.

**Examples:**

- `3.2.6`

**Formats:** [[JSON](version.json)] [[MD](version.md)]

**JSON definition:**

``` json
{
    "$id": "https://schemas.optimade.org/properties/v1.2.0/optimade/files/version",
    "title": "Version",
    "x-optimade-type": "string",
    "x-optimade-definition": {
        "kind": "property",
        "version": "1.2.0",
        "format": "1.2",
        "name": "version"
    },
    "type": [
        "string",
        "null"
    ],
    "description": "Version information of a file (e.g. commit, revision, timestamp).\n\n**Requirements/Conventions:**\n\n- If provided, it MUST be guaranteed that file contents pertaining to the same combination of id and version are the same.",
    "examples": [
        "3.2.6"
    ],
    "x-optimade-unit": "inapplicable",
    "$schema": "https://schemas.optimade.org/meta/v1.2.0/optimade/property_definition.md"
}
```
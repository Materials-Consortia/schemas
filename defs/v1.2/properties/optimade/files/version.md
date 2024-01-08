# Version (property)

This page documents an [OPTIMADE](https://www.optimade.org/) [Property Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/defs/v1.2/properties/optimade/files/version`](https://schemas.optimade.org/defs/v1.2/properties/optimade/files/version.md)**  
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
    "$schema": "https://schemas.optimade.org/meta/v1.2/optimade/property_definition.md",
    "$id": "https://schemas.optimade.org/defs/v1.2/properties/optimade/files/version",
    "title": "Version",
    "x-optimade-type": "string",
    "x-optimade-definition": {
        "label": "version_optimade_files",
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
    "x-optimade-unit": "inapplicable"
}
```
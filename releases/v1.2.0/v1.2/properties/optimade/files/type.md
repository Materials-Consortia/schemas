# type (property)

This page documents an [OPTIMADE](https://www.optimade.org/) [Property Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/defs/v1.2/properties/core/type`](https://schemas.optimade.org/defs/v1.2/properties/core/type.md)**  
**Definition name:** `type`

**Property name:** type  
**Description:** The name of the type of an entry.  
**Type:** string  

**Requirements/Conventions:**

- MUST be an existing entry type.
- The entry of type <type> and ID <id> MUST be returned in response to a request for /<type>/<id> under the versioned or unversioned base URL serving the API.

**Examples:**

- `structures`

**Formats:** [[JSON](type.json)] [[MD](type.md)]

**JSON definition:**

``` json
{
    "$id": "https://schemas.optimade.org/defs/v1.2/properties/core/type",
    "$schema": "https://schemas.optimade.org/meta/v1.2/optimade/property_definition.json",
    "title": "type",
    "x-optimade-type": "string",
    "x-optimade-definition": {
        "label": "type_core",
        "kind": "property",
        "version": "1.2.0",
        "format": "1.2",
        "name": "type"
    },
    "type": [
        "string"
    ],
    "description": "The name of the type of an entry.\n\n**Requirements/Conventions:**\n\n- MUST be an existing entry type.\n- The entry of type <type> and ID <id> MUST be returned in response to a request for /<type>/<id> under the versioned or unversioned base URL serving the API.",
    "examples": [
        "structures"
    ],
    "x-optimade-unit": "inapplicable"
}
```
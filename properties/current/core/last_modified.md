# Last modified (property)
This page documents an [OPTIMADE](https://www.optimade.org/) [Property Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/properties/v1.2.0/core/last_modified`](https://schemas.optimade.org/properties/v1.2.0/core/last_modified)**  
**Definition name:** `last_modified`

**Property name:** Last modified  
**Description:** Date and time representing when the entry was last modified.  
**Type:** timestamp  



**Examples:**

- `2007-04-05T14:30:20Z`

**Formats:** [[JSON](last_modified.json)] [[MD](last_modified.md)]

**JSON definition:**

``` json
{
    "$id": "https://schemas.optimade.org/properties/v1.2.0/core/last_modified",
    "title": "Last modified",
    "x-optimade-type": "timestamp",
    "x-optimade-definition": {
        "kind": "property",
        "version": "1.2.0",
        "format": "1.2",
        "name": "last_modified"
    },
    "type": [
        "string",
        "null"
    ],
    "format": "date-time",
    "description": "Date and time representing when the entry was last modified.",
    "examples": [
        "2007-04-05T14:30:20Z"
    ],
    "x-optimade-unit": "inapplicable",
    "$schema": "https://schemas.optimade.org/meta/v1.2.0/optimade/property_definition.md"
}
```
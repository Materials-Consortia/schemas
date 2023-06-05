# Access time (property)
This page documents an [OPTIMADE](https://www.optimade.org/) [Property Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/properties/v1.2.0/optimade/files/atime`](https://schemas.optimade.org/properties/v1.2.0/optimade/files/atime)**  
**Definition name:** `atime`

**Property name:** Access time  
**Description:** Time of last access of a file as per POSIX standard.  
**Type:** timestamp  



**Examples:**

- `2007-04-05T14:30:20Z`

**Formats:** [[JSON](atime.json)] [[MD](atime.md)]

**JSON definition:**

``` json
{
    "$id": "https://schemas.optimade.org/properties/v1.2.0/optimade/files/atime",
    "title": "Access time",
    "x-optimade-type": "timestamp",
    "x-optimade-definition": {
        "kind": "property",
        "version": "1.2.0",
        "format": "1.2",
        "name": "atime"
    },
    "type": [
        "string",
        "null"
    ],
    "format": "date-time",
    "description": "Time of last access of a file as per POSIX standard.",
    "examples": [
        "2007-04-05T14:30:20Z"
    ],
    "x-optimade-unit": "inapplicable",
    "$schema": "https://schemas.optimade.org/meta/v1.2.0/optimade/property_definition.md"
}
```
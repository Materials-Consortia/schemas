# access time (property)

This page documents an [OPTIMADE](https://www.optimade.org/) [Property Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/defs/v1.2/properties/optimade/files/atime`](https://schemas.optimade.org/defs/v1.2/properties/optimade/files/atime.md)**  
**Definition name:** `atime`

**Property name:** access time  
**Description:** Time of last access of a file as per POSIX standard.  
**Type:** timestamp  



**Examples:**

- `"2007-04-05T14:30:20Z"`

**Formats:** [[JSON](atime.json)] [[MD](atime.md)]

**JSON definition:**

``` json
{
    "$id": "https://schemas.optimade.org/defs/v1.2/properties/optimade/files/atime",
    "$schema": "https://schemas.optimade.org/meta/v1.2/optimade/property_definition.json",
    "title": "access time",
    "x-optimade-type": "timestamp",
    "x-optimade-definition": {
        "label": "atime_optimade_files",
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
    "x-optimade-unit": "inapplicable"
}
```
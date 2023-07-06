# Change time (property)

This page documents an [OPTIMADE](https://www.optimade.org/) [Property Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/defs/v1.2/properties/optimade/files/ctime`](https://schemas.optimade.org/defs/v1.2/properties/optimade/files/ctime)**  
**Definition name:** `ctime`

**Property name:** Change time  
**Description:** Time of last status change of a file as per POSIX standard.  
**Type:** timestamp  



**Examples:**

- `2007-04-05T14:30:20Z`

**Formats:** [[JSON](ctime.json)] [[MD](ctime.md)]

**JSON definition:**

``` json
{
    "$schema": "https://schemas.optimade.org/meta/v1.2/optimade/property_definition.md",
    "$id": "https://schemas.optimade.org/defs/v1.2/properties/optimade/files/ctime",
    "title": "Change time",
    "x-optimade-type": "timestamp",
    "x-optimade-definition": {
        "kind": "property",
        "version": "1.2.0",
        "format": "1.2",
        "name": "ctime"
    },
    "type": [
        "string",
        "null"
    ],
    "format": "date-time",
    "description": "Time of last status change of a file as per POSIX standard.",
    "examples": [
        "2007-04-05T14:30:20Z"
    ],
    "x-optimade-unit": "inapplicable"
}
```
# Size (property)

This page documents an [OPTIMADE](https://www.optimade.org/) [Property Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/defs/v1.2/properties/optimade/files/size`](https://schemas.optimade.org/defs/v1.2/properties/optimade/files/size.md)**  
**Definition name:** `size`

**Property name:** Size  
**Description:** Size of a file in bytes.  
**Type:** integer  

**Requirements/Conventions:**

- If provided, it MUST be guaranteed that either exact size of a file is given or its upper bound.
  This way if a client reserves a static buffer or truncates the download stream after this many bytes the whole file would be received.
  Such provision is included to allow the providers to serve on-the-fly compressed files.

**Examples:**

- `4711`

**Formats:** [[JSON](size.json)] [[MD](size.md)]

**JSON definition:**

``` json
{
    "$schema": "https://schemas.optimade.org/meta/v1.2/optimade/property_definition.md",
    "$id": "https://schemas.optimade.org/defs/v1.2/properties/optimade/files/size",
    "title": "Size",
    "x-optimade-type": "integer",
    "x-optimade-definition": {
        "label": "size_optimade_files",
        "kind": "property",
        "version": "1.2.0",
        "format": "1.2",
        "name": "size"
    },
    "x-optimade-unit-definitions": [
        {
            "$id": "https://schemas.optimade.org/defs/v1.2/units/iso-iec-80000/2008/information_science_and_technology/byte",
            "title": "byte",
            "symbol": "B",
            "display-symbol": "B",
            "description": "A unit of digital information representing eight bits, defined in the International System of Quantities in ISO/IEC 80000-13 (2008).\n\n\"In English, the name byte, symbol B, is used as a synonym for octet. Here byte means an eight-bit byte.\" [ISO/IEC 80000-13 (2008)]",
            "resources": [
                {
                    "relation": "Defining standard",
                    "resource-id": "https://www.iso.org/standard/31898.html"
                },
                {
                    "relation": "Wikipedia article describing the unit",
                    "resource-id": "https://en.wikipedia.org/wiki/Byte"
                }
            ],
            "defining-relation": {
                "base-units": [
                    {
                        "symbol": "bit",
                        "id": "https://schemas.optimade.org/defs/v1.2/units/independent/1948/information/bit"
                    }
                ],
                "base-units-expression": "bit",
                "scale": {
                    "numerator": 8
                }
            },
            "standard": {
                "name": "iso-iec-80000",
                "year": 2008,
                "category": "information_science_and_technology",
                "symbol": "B"
            },
            "x-optimade-definition": {
                "label": "byte_iso_iec_80000_2008_information_science_and_technology",
                "kind": "unit",
                "format": "1.2",
                "version": "1.2.0",
                "name": "byte"
            }
        }
    ],
    "type": [
        "integer",
        "null"
    ],
    "description": "Size of a file in bytes.\n\n**Requirements/Conventions:**\n\n- If provided, it MUST be guaranteed that either exact size of a file is given or its upper bound.\n  This way if a client reserves a static buffer or truncates the download stream after this many bytes the whole file would be received.\n  Such provision is included to allow the providers to serve on-the-fly compressed files.",
    "examples": [
        4711
    ],
    "x-optimade-unit": "byte"
}
```
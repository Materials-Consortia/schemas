# byte, B (unit)

This page documents an [OPTIMADE](https://www.optimade.org/) [Unit Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/defs/v1.2/units/iso-iec-80000/2008/information_science_and_technology/byte`](https://schemas.optimade.org/defs/v1.2/units/iso-iec-80000/2008/information_science_and_technology/byte.md)**  
**Definition name:** `byte`

**Unit name:** byte  
**Latin symbol:** B  
**Display symbol:** B  
  
**Description:** A unit of digital information representing eight bits, defined in the International System of Quantities in ISO/IEC 80000-13 (2008).

"In English, the name byte, symbol B, is used as a synonym for octet. Here byte means an eight-bit byte." [ISO/IEC 80000-13 (2008)]

**Resources:**

- [Defining standard](https://www.iso.org/standard/31898.html)
- [Wikipedia article describing the unit](https://en.wikipedia.org/wiki/Byte)


**Formats:** [[JSON](byte.json)] [[MD](byte.md)]

**JSON definition:**

``` json
{
    "$schema": "https://schemas.optimade.org/meta/v1.2/optimade/physical_unit_definition.md",
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
```
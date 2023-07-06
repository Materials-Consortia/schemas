# hertz, Hz (unit)

This page documents an [OPTIMADE](https://www.optimade.org/) [Unit Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/defs/v1.2/units/si/1960/named/hertz`](https://schemas.optimade.org/defs/v1.2/units/si/1960/named/hertz)**  
**Definition name:** `hertz`

**Unit name:** hertz  
**Latin symbol:** Hz  
**Display symbol:** Hz  
  
**Description:** A derived SI unit for frequency equal to s⁻¹ in the 1960 SI base units.

"The frequency of a periodic phenomenon is expressed in hertz, as the inverse of its period expressed in seconds." [9th CGPM meeting in 1946]

**Resources:**

- [Definition at the 9st CGPM meeting (1948)](https://www.bipm.org/en/committees/cg/cgpm/9-1948)
- [Definition and establishment of the SI unit system at the 11th CGPM meeting (1960), resolution 12.](https://www.bipm.org/en/committees/cg/cgpm/11-1960/resolution-12)
- [Wikipedia article describing the unit](https://en.wikipedia.org/wiki/Hertz)


**Formats:** [[JSON](hertz.json)] [[MD](hertz.md)]

**JSON definition:**

``` json
{
    "$schema": "https://schemas.optimade.org/meta/v1.2/optimade/physical_unit_definition.md",
    "$id": "https://schemas.optimade.org/defs/v1.2/units/si/1960/named/hertz",
    "title": "hertz",
    "symbol": "Hz",
    "display-symbol": "Hz",
    "description": "A derived SI unit for frequency equal to s\u207b\u00b9 in the 1960 SI base units.\n\n\"The frequency of a periodic phenomenon is expressed in hertz, as the inverse of its period expressed in seconds.\" [9th CGPM meeting in 1946]",
    "standard": {
        "name": "gnu units",
        "version": "3.15",
        "symbol": "hertz"
    },
    "resources": [
        {
            "relation": "Definition at the 9st CGPM meeting (1948)",
            "resource-id": "https://www.bipm.org/en/committees/cg/cgpm/9-1948"
        },
        {
            "relation": "Definition and establishment of the SI unit system at the 11th CGPM meeting (1960), resolution 12.",
            "resource-id": "https://www.bipm.org/en/committees/cg/cgpm/11-1960/resolution-12"
        },
        {
            "relation": "Wikipedia article describing the unit",
            "resource-id": "https://en.wikipedia.org/wiki/Hertz"
        }
    ],
    "defining-relation": {
        "base-units": [
            {
                "symbol": "s",
                "id": "https://schemas.optimade.org/units/v1.2/si/1960/base/s"
            }
        ],
        "base-units-expression": "s^-1"
    },
    "x-optimade-definition": {
        "kind": "unit",
        "format": "1.2",
        "version": "1.2.0",
        "name": "hertz"
    }
}
```
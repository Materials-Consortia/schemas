# second, s (unit)

This page documents an [OPTIMADE](https://www.optimade.org/) [Unit Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/defs/v1.2/units/si/1960/base/second`](https://schemas.optimade.org/defs/v1.2/units/si/1960/base/second.md)**  
**Definition name:** `second`

**Unit name:** second  
**Latin symbol:** s  
**Display symbol:** s  
  
**Description:** The SI base unit of time defined as a specific fraction of the tropical year 1900 at the 11th CGPM Meeting in 1960.

"The second is the fraction 1/31556925.9747 of the tropical year for 1900 January 0 at 12 hours ephemeris time." [11th CGPM Meeting in 1960, resolution 9]
The second was included into SI at the 11th CGPM Meeting in 1960 in resolution 12.

**Resources:**

- [Definition at the 11th CGPM meeting (1960), resolution 6.](https://www.bipm.org/en/committees/cg/cgpm/11-1960/resolution-6)
- [Establishment of the SI unit system at the 11th CGPM meeting (1960), resolution 12.](https://www.bipm.org/en/committees/cg/cgpm/11-1960/resolution-12)
- [Wikipedia article describing the unit](https://en.wikipedia.org/wiki/Second)


**Formats:** [[JSON](second.json)] [[MD](second.md)]

**JSON definition:**

``` json
{
    "$id": "https://schemas.optimade.org/defs/v1.2/units/si/1960/base/second",
    "$schema": "https://schemas.optimade.org/meta/v1.2/optimade/physical_unit_definition.json",
    "title": "second",
    "symbol": "s",
    "display-symbol": "s",
    "description": "The SI base unit of time defined as a specific fraction of the tropical year 1900 at the 11th CGPM Meeting in 1960.\n\n\"The second is the fraction 1/31556925.9747 of the tropical year for 1900 January 0 at 12 hours ephemeris time.\" [11th CGPM Meeting in 1960, resolution 9]\nThe second was included into SI at the 11th CGPM Meeting in 1960 in resolution 12.",
    "resources": [
        {
            "relation": "Definition at the 11th CGPM meeting (1960), resolution 6.",
            "resource-id": "https://www.bipm.org/en/committees/cg/cgpm/11-1960/resolution-6"
        },
        {
            "relation": "Establishment of the SI unit system at the 11th CGPM meeting (1960), resolution 12.",
            "resource-id": "https://www.bipm.org/en/committees/cg/cgpm/11-1960/resolution-12"
        },
        {
            "relation": "Wikipedia article describing the unit",
            "resource-id": "https://en.wikipedia.org/wiki/Second"
        }
    ],
    "standard": {
        "name": "si",
        "year": 1960,
        "category": "base",
        "symbol": "s"
    },
    "x-optimade-definition": {
        "label": "second_si_1960_base",
        "kind": "unit",
        "format": "1.2",
        "version": "1.2.0",
        "name": "second"
    }
}
```
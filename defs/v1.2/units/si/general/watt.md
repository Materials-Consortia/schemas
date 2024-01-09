# watt, W (unit)

This page documents an [OPTIMADE](https://www.optimade.org/) [Unit Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/defs/v1.2/units/si/general/watt`](https://schemas.optimade.org/defs/v1.2/units/si/general/watt.md)**  
**Definition name:** `watt`

**Unit name:** watt  
**Latin symbol:** W  
**Display symbol:** W  
  
**Description:** A unit for power and radiant flux equal to kg·m²·s⁻³ using the current, or one of the historical, definitions of the SI units.

"The watt is the power that produces one joule per second." [9th CGPM meeting in 1946]

The watt was defined at the 9th CGPM Meeting in 1946, included in SI at the 11th CGPM meeting in 1960, resolution 12, implicitly redefined via the redefinitions of the second at the 13th CGPM Meeting in 1967, resolution 1; the metre at the 17th CGPM meeting (1983), resolution 1; and the kilogram at the 26th CGPM Meeting (2018), resolution 1.

This is a generalized definition taken to reference the current, or one of the historical, SI unit definitions.
This definition is intended for situations when it is not possible to be more precise, e.g., in contexts where data have been collected that uses different historical SI definitions.

**Resources:**

- [Definition and establishment of the SI unit system at the 11th CGPM meeting (1960), resolution 12.](https://www.bipm.org/en/committees/cg/cgpm/11-1960/resolution-12)
- [Redefinition of the metre at the 17th CGPM meeting (1983), resolution 1](https://www.bipm.org/en/committees/cg/cgpm/17-1983/resolution-1)
- [Redefinition of the second in the 13th CGPM Meeting (1967), resolution 1](https://www.bipm.org/en/committees/cg/cgpm/13-1967/resolution-1)
- [Redefinition of the metre at the 17th CGPM meeting (1983), resolution 1](https://www.bipm.org/en/committees/cg/cgpm/17-1983/resolution-1)
- [Wikipedia article describing the unit](https://en.wikipedia.org/wiki/Watt)


**Compatibility:** (other definitions that are covered by the above definition)

- [`https://schemas.optimade.org/defs/v1.2/units/si/1960/named/watt`](https://schemas.optimade.org/defs/v1.2/units/si/1960/named/watt.md)
- [`https://schemas.optimade.org/defs/v1.2/units/si/1967/named/watt`](https://schemas.optimade.org/defs/v1.2/units/si/1967/named/watt.md)
- [`https://schemas.optimade.org/defs/v1.2/units/si/1983/named/watt`](https://schemas.optimade.org/defs/v1.2/units/si/1983/named/watt.md)
- [`https://schemas.optimade.org/defs/v1.2/units/si/2019/named/watt`](https://schemas.optimade.org/defs/v1.2/units/si/2019/named/watt.md)


**Formats:** [[JSON](watt.json)] [[MD](watt.md)]

**JSON definition:**

``` json
{
    "$id": "https://schemas.optimade.org/defs/v1.2/units/si/general/watt",
    "$schema": "https://schemas.optimade.org/meta/v1.2/optimade/physical_unit_definition.json",
    "title": "watt",
    "symbol": "W",
    "display-symbol": "W",
    "description": "A unit for power and radiant flux equal to kg\u00b7m\u00b2\u00b7s\u207b\u00b3 using the current, or one of the historical, definitions of the SI units.\n\n\"The watt is the power that produces one joule per second.\" [9th CGPM meeting in 1946]\n\nThe watt was defined at the 9th CGPM Meeting in 1946, included in SI at the 11th CGPM meeting in 1960, resolution 12, implicitly redefined via the redefinitions of the second at the 13th CGPM Meeting in 1967, resolution 1; the metre at the 17th CGPM meeting (1983), resolution 1; and the kilogram at the 26th CGPM Meeting (2018), resolution 1.\n\nThis is a generalized definition taken to reference the current, or one of the historical, SI unit definitions.\nThis definition is intended for situations when it is not possible to be more precise, e.g., in contexts where data have been collected that uses different historical SI definitions.",
    "compatibility": [
        "https://schemas.optimade.org/defs/v1.2/units/si/1960/named/watt",
        "https://schemas.optimade.org/defs/v1.2/units/si/1967/named/watt",
        "https://schemas.optimade.org/defs/v1.2/units/si/1983/named/watt",
        "https://schemas.optimade.org/defs/v1.2/units/si/2019/named/watt"
    ],
    "resources": [
        {
            "relation": "Definition and establishment of the SI unit system at the 11th CGPM meeting (1960), resolution 12.",
            "resource-id": "https://www.bipm.org/en/committees/cg/cgpm/11-1960/resolution-12"
        },
        {
            "relation": "Redefinition of the metre at the 17th CGPM meeting (1983), resolution 1",
            "resource-id": "https://www.bipm.org/en/committees/cg/cgpm/17-1983/resolution-1"
        },
        {
            "relation": "Redefinition of the second in the 13th CGPM Meeting (1967), resolution 1",
            "resource-id": "https://www.bipm.org/en/committees/cg/cgpm/13-1967/resolution-1"
        },
        {
            "relation": "Redefinition of the metre at the 17th CGPM meeting (1983), resolution 1",
            "resource-id": "https://www.bipm.org/en/committees/cg/cgpm/17-1983/resolution-1"
        },
        {
            "relation": "Wikipedia article describing the unit",
            "resource-id": "https://en.wikipedia.org/wiki/Watt"
        }
    ],
    "defining-relation": {
        "base-units": [
            {
                "symbol": "kg",
                "id": "https://schemas.optimade.org/defs/v1.2/units/si/general/kilogram"
            },
            {
                "symbol": "m",
                "id": "https://schemas.optimade.org/defs/v1.2/units/si/general/metre"
            },
            {
                "symbol": "s",
                "id": "https://schemas.optimade.org/defs/v1.2/units/si/general/second"
            }
        ],
        "base-units-expression": "kg*m^2*s^-3"
    },
    "x-optimade-definition": {
        "label": "watt_si_general",
        "kind": "unit",
        "format": "1.2",
        "version": "1.2.0",
        "name": "watt"
    }
}
```
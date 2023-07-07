# lux, lx (unit)

This page documents an [OPTIMADE](https://www.optimade.org/) [Unit Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/defs/v1.2/units/si/general/lux`](https://schemas.optimade.org/defs/v1.2/units/si/general/lux.md)**  
**Definition name:** `lux`

**Unit name:** lux  
**Latin symbol:** lx  
**Display symbol:** lx  
  
**Description:** A derived SI unit for illuminance equal to cd⋅sr⋅m⁻² using the current, or one of the historical, definitions of the SI units.

"The lux is the illuminance of a surface that receives a uniformly distributed luminous flux of one lumen per square meter." [9th CGPM meeting in 1946]

The lux was defined at the 9th CGPM meeting in 1946, and implicitly redefined via the redefinitions of the second at the 13th CGPM Meeting in 1967, resolution 1, the candela at the 16th CGPM Meeting in 1979, resolution 3, the metre at the 17th CGPM meeting (1983), resolution 1, and the candela (implicitly redefined via the kilogram) at the 26th CGPM Meeting (2018), resolution 1.

This is a generalized definition taken to reference the current, or one of the historical, SI unit definitions.
This definition is intended for situations when it is not possible to be more precise, e.g., in contexts where data have been collected that uses different historical SI definitions.

**Resources:**

- [Definition at the 9st CGPM meeting (1948)](https://www.bipm.org/en/committees/cg/cgpm/9-1948)
- [Definition and establishment of the SI unit system at the 11th CGPM meeting (1960), resolution 12.](https://www.bipm.org/en/committees/cg/cgpm/11-1960/resolution-12)
- [Redefinition of the candela at the 16th CGPM Meeting in 1979, resolution 3.](https://www.bipm.org/en/committees/cg/cgpm/16-1979/resolution-3)
- [Redefinition of the metre at the 17th CGPM meeting (1983), resolution 1](https://www.bipm.org/en/committees/cg/cgpm/17-1983/resolution-1)
- [Redefinition of the second in the 13th CGPM Meeting (1967), resolution 1](https://www.bipm.org/en/committees/cg/cgpm/13-1967/resolution-1)
- [Redefinition of the kilogram at the 26th CGPM Meeting (2018), resolution 1](https://www.bipm.org/en/committees/cg/cgpm/26-2018/resolution-1)
- [Wikipedia article describing the unit](https://en.wikipedia.org/wiki/Lux)


**Formats:** [[JSON](lux.json)] [[MD](lux.md)]

**JSON definition:**

``` json
{
    "$schema": "https://schemas.optimade.org/meta/v1.2/optimade/physical_unit_definition.md",
    "$id": "https://schemas.optimade.org/defs/v1.2/units/si/general/lux",
    "title": "lux",
    "symbol": "lx",
    "display-symbol": "lx",
    "description": "A derived SI unit for illuminance equal to cd\u22c5sr\u22c5m\u207b\u00b2 using the current, or one of the historical, definitions of the SI units.\n\n\"The lux is the illuminance of a surface that receives a uniformly distributed luminous flux of one lumen per square meter.\" [9th CGPM meeting in 1946]\n\nThe lux was defined at the 9th CGPM meeting in 1946, and implicitly redefined via the redefinitions of the second at the 13th CGPM Meeting in 1967, resolution 1, the candela at the 16th CGPM Meeting in 1979, resolution 3, the metre at the 17th CGPM meeting (1983), resolution 1, and the candela (implicitly redefined via the kilogram) at the 26th CGPM Meeting (2018), resolution 1.\n\nThis is a generalized definition taken to reference the current, or one of the historical, SI unit definitions.\nThis definition is intended for situations when it is not possible to be more precise, e.g., in contexts where data have been collected that uses different historical SI definitions.",
    "compatibility": [
        "https://schemas.optimade.org/units/v1.2/si/1960/named/lux",
        "https://schemas.optimade.org/units/v1.2/si/1967/named/lux",
        "https://schemas.optimade.org/units/v1.2/si/1979/named/lux",
        "https://schemas.optimade.org/units/v1.2/si/1983/named/lux",
        "https://schemas.optimade.org/units/v1.2/si/2019/named/lux"
    ],
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
            "relation": "Redefinition of the candela at the 16th CGPM Meeting in 1979, resolution 3.",
            "resource-id": "https://www.bipm.org/en/committees/cg/cgpm/16-1979/resolution-3"
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
            "relation": "Redefinition of the kilogram at the 26th CGPM Meeting (2018), resolution 1",
            "resource-id": "https://www.bipm.org/en/committees/cg/cgpm/26-2018/resolution-1"
        },
        {
            "relation": "Wikipedia article describing the unit",
            "resource-id": "https://en.wikipedia.org/wiki/Lux"
        }
    ],
    "defining-relation": {
        "base-units": [
            {
                "symbol": "cd",
                "id": "https://schemas.optimade.org/units/v1.2/si/general/candela"
            },
            {
                "symbol": "sr",
                "id": "https://schemas.optimade.org/units/v1.2/si/general/steradian"
            },
            {
                "symbol": "m",
                "id": "https://schemas.optimade.org/units/v1.2/si/general/metre"
            }
        ],
        "base-units-expression": "cd*m^-2*sr"
    },
    "x-optimade-definition": {
        "kind": "unit",
        "format": "1.2",
        "version": "1.2.0",
        "name": "lux"
    }
}
```
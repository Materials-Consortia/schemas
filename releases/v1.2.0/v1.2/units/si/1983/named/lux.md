# lux, lx (unit)

This page documents an [OPTIMADE](https://www.optimade.org/) [Unit Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/defs/v1.2/units/si/1983/named/lux`](https://schemas.optimade.org/defs/v1.2/units/si/1983/named/lux.md)**  
**Definition name:** `lux`

**Unit name:** lux  
**Latin symbol:** lx  
**Display symbol:** lx  
  
**Description:** A derived SI unit for illuminance equal to cd⋅sr⋅m⁻² in 1983 SI units.

"The lux is the illuminance of a surface that receives a uniformly distributed luminous flux of one lumen per square meter." [9th CGPM meeting in 1946]

The lux was defined at the 9th CGPM meeting in 1946, and implicitly redefined via the redefinitions of the second at the 13th CGPM Meeting in 1967, resolution 1, the candela at the 16th CGPM Meeting in 1979, resolution 3, and the metre at the 17th CGPM meeting (1983), resolution 1.

**Resources:**

- [Definition at the 9st CGPM meeting (1948)](https://www.bipm.org/en/committees/cg/cgpm/9-1948)
- [Definition and establishment of the SI unit system at the 11th CGPM meeting (1960), resolution 12.](https://www.bipm.org/en/committees/cg/cgpm/11-1960/resolution-12)
- [Redefinition of the metre at the 17th CGPM meeting (1983), resolution 1](https://www.bipm.org/en/committees/cg/cgpm/17-1983/resolution-1)
- [Redefinition of the second in the 13th CGPM Meeting (1967), resolution 1](https://www.bipm.org/en/committees/cg/cgpm/13-1967/resolution-1)
- [Redefinition of the candela at the 16th CGPM Meeting in 1979, resolution 3.](https://www.bipm.org/en/committees/cg/cgpm/16-1979/resolution-3)
- [Wikipedia article describing the unit](https://en.wikipedia.org/wiki/Lux)


**Formats:** [[JSON](lux.json)] [[MD](lux.md)]

**JSON definition:**

``` json
{
    "$schema": "https://schemas.optimade.org/meta/v1.2/optimade/physical_unit_definition.md",
    "$id": "https://schemas.optimade.org/defs/v1.2/units/si/1983/named/lux",
    "title": "lux",
    "symbol": "lx",
    "display-symbol": "lx",
    "description": "A derived SI unit for illuminance equal to cd\u22c5sr\u22c5m\u207b\u00b2 in 1983 SI units.\n\n\"The lux is the illuminance of a surface that receives a uniformly distributed luminous flux of one lumen per square meter.\" [9th CGPM meeting in 1946]\n\nThe lux was defined at the 9th CGPM meeting in 1946, and implicitly redefined via the redefinitions of the second at the 13th CGPM Meeting in 1967, resolution 1, the candela at the 16th CGPM Meeting in 1979, resolution 3, and the metre at the 17th CGPM meeting (1983), resolution 1.",
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
            "relation": "Redefinition of the metre at the 17th CGPM meeting (1983), resolution 1",
            "resource-id": "https://www.bipm.org/en/committees/cg/cgpm/17-1983/resolution-1"
        },
        {
            "relation": "Redefinition of the second in the 13th CGPM Meeting (1967), resolution 1",
            "resource-id": "https://www.bipm.org/en/committees/cg/cgpm/13-1967/resolution-1"
        },
        {
            "relation": "Redefinition of the candela at the 16th CGPM Meeting in 1979, resolution 3.",
            "resource-id": "https://www.bipm.org/en/committees/cg/cgpm/16-1979/resolution-3"
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
                "id": "https://schemas.optimade.org/defs/v1.2/units/si/1983/base/candela"
            },
            {
                "symbol": "sr",
                "id": "https://schemas.optimade.org/defs/v1.2/units/si/1960/supplementary/steradian"
            },
            {
                "symbol": "m",
                "id": "https://schemas.optimade.org/defs/v1.2/units/si/1983/base/metre"
            }
        ],
        "base-units-expression": "cd*m^-2*sr"
    },
    "standard": {
        "name": "si",
        "year": 1983,
        "category": "named",
        "symbol": "lx"
    },
    "x-optimade-definition": {
        "label": "lux_si_1983_named",
        "kind": "unit",
        "format": "1.2",
        "version": "1.2.0",
        "name": "lux"
    }
}
```
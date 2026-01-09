# lux, lx (unit)

This page documents an [OPTIMADE](https://www.optimade.org/) [Unit Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/defs/v1.2/units/si/1979/named/lux`](https://schemas.optimade.org/defs/v1.2/units/si/1979/named/lux.md)**  
**Definition name:** `lux`

**Unit name:** lux  
**Latin symbol:** lx  
**Display symbol:** lx  
  
**Description:** A derived SI unit for illuminance equal to cd⋅sr⋅m⁻² in the 1979 SI units.

"The lux is the illuminance of a surface that receives a uniformly distributed luminous flux of one lumen per square meter." [9th CGPM meeting in 1946]

The lux was defined at the 9th CGPM meeting in 1946, and implicitly redefined via the redefinition of the second at the 13th CGPM Meeting in 1967, resolution 1 and the redefinition of the candela at the 16th CGPM Meeting in 1979, resolution 3.

**Resources:**

- [Definition and establishment of the SI unit system at the 11th CGPM meeting (1960), resolution 12.](https://www.bipm.org/en/committees/cg/cgpm/11-1960/resolution-12)
- [Redefinition of the candela at the 16th CGPM Meeting in 1979, resolution 3.](https://www.bipm.org/en/committees/cg/cgpm/16-1979/resolution-3)
- [Redefinition of the second in the 13th CGPM Meeting (1967), resolution 1](https://www.bipm.org/en/committees/cg/cgpm/13-1967/resolution-1)
- [Wikipedia article describing the unit](https://en.wikipedia.org/wiki/Lux)


**Formats:** [[JSON](lux.json)] [[MD](lux.md)]

**JSON definition:**

``` json
{
    "$id": "https://schemas.optimade.org/defs/v1.2/units/si/1979/named/lux",
    "$schema": "https://schemas.optimade.org/meta/v1.2/optimade/physical_unit_definition.json",
    "title": "lux",
    "symbol": "lx",
    "display-symbol": "lx",
    "description": "A derived SI unit for illuminance equal to cd\u22c5sr\u22c5m\u207b\u00b2 in the 1979 SI units.\n\n\"The lux is the illuminance of a surface that receives a uniformly distributed luminous flux of one lumen per square meter.\" [9th CGPM meeting in 1946]\n\nThe lux was defined at the 9th CGPM meeting in 1946, and implicitly redefined via the redefinition of the second at the 13th CGPM Meeting in 1967, resolution 1 and the redefinition of the candela at the 16th CGPM Meeting in 1979, resolution 3.",
    "resources": [
        {
            "relation": "Definition and establishment of the SI unit system at the 11th CGPM meeting (1960), resolution 12.",
            "resource-id": "https://www.bipm.org/en/committees/cg/cgpm/11-1960/resolution-12"
        },
        {
            "relation": "Redefinition of the candela at the 16th CGPM Meeting in 1979, resolution 3.",
            "resource-id": "https://www.bipm.org/en/committees/cg/cgpm/16-1979/resolution-3"
        },
        {
            "relation": "Redefinition of the second in the 13th CGPM Meeting (1967), resolution 1",
            "resource-id": "https://www.bipm.org/en/committees/cg/cgpm/13-1967/resolution-1"
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
                "id": "https://schemas.optimade.org/defs/v1.2/units/si/1979/base/candela"
            },
            {
                "symbol": "sr",
                "id": "https://schemas.optimade.org/defs/v1.2/units/si/1960/supplementary/steradian"
            },
            {
                "symbol": "m",
                "id": "https://schemas.optimade.org/defs/v1.2/units/si/1960/base/metre"
            }
        ],
        "base-units-expression": "cd*m^-2*sr"
    },
    "standard": {
        "name": "si",
        "year": 1979,
        "category": "named",
        "symbol": "lx"
    },
    "x-optimade-definition": {
        "label": "lux_si_1979_named",
        "kind": "unit",
        "format": "1.2",
        "version": "1.2.0",
        "name": "lux"
    }
}
```
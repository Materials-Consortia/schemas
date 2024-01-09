# lumen, lm (unit)

This page documents an [OPTIMADE](https://www.optimade.org/) [Unit Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/defs/v1.2/units/si/1960/named/lumen`](https://schemas.optimade.org/defs/v1.2/units/si/1960/named/lumen.md)**  
**Definition name:** `lumen`

**Unit name:** lumen  
**Latin symbol:** lm  
**Display symbol:** lm  
  
**Description:** A derived SI unit for luminous flux equal to cd·sr in the 1960 SI base units.

"The lumen is the luminous flux emitted in a steradian by a uniform point source with a luminous intensity of one candela." [9th CGPM meeting in 1946]

**Resources:**

- [Definition at the 9st CGPM meeting (1948)](https://www.bipm.org/en/committees/cg/cgpm/9-1948)
- [Definition and establishment of the SI unit system at the 11th CGPM meeting (1960), resolution 12.](https://www.bipm.org/en/committees/cg/cgpm/11-1960/resolution-12)
- [Wikipedia article describing the unit](https://en.wikipedia.org/wiki/Lumen_(unit))


**Formats:** [[JSON](lumen.json)] [[MD](lumen.md)]

**JSON definition:**

``` json
{
    "$id": "https://schemas.optimade.org/defs/v1.2/units/si/1960/named/lumen",
    "$schema": "https://schemas.optimade.org/meta/v1.2/optimade/physical_unit_definition.json",
    "title": "lumen",
    "symbol": "lm",
    "display-symbol": "lm",
    "description": "A derived SI unit for luminous flux equal to cd\u00b7sr in the 1960 SI base units.\n\n\"The lumen is the luminous flux emitted in a steradian by a uniform point source with a luminous intensity of one candela.\" [9th CGPM meeting in 1946]",
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
            "resource-id": "https://en.wikipedia.org/wiki/Lumen_(unit)"
        }
    ],
    "defining-relation": {
        "base-units": [
            {
                "symbol": "cd",
                "id": "https://schemas.optimade.org/defs/v1.2/units/si/1960/base/candela"
            },
            {
                "symbol": "sr",
                "id": "https://schemas.optimade.org/defs/v1.2/units/si/1960/supplementary/steradian"
            }
        ],
        "base-units-expression": "cd*sr"
    },
    "standard": {
        "name": "si",
        "year": 1960,
        "category": "named",
        "symbol": "lm"
    },
    "x-optimade-definition": {
        "label": "lumen_si_1960_named",
        "kind": "unit",
        "format": "1.2",
        "version": "1.2.0",
        "name": "lumen"
    }
}
```
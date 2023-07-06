# coulomb, C (unit)

This page documents an [OPTIMADE](https://www.optimade.org/) [Unit Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/defs/v1.2/units/si/general/coulomb`](https://schemas.optimade.org/defs/v1.2/units/si/general/coulomb)**  
**Definition name:** `coulomb`

**Unit name:** coulomb  
**Latin symbol:** coulomb  
**Display symbol:** C  
  
**Description:** A unit for electric charge equal to s·A using the current, or one of the historical, definitions of the SI units.

"The coulomb is the amount of electricity transported in one second by a current of one ampere." [9th CGPM meeting in 1946]

The coulomb was defined at the 9th CGPM Meeting in 1946, included in SI at the 11th CGPM meeting in 1960, resolution 12, implicitly redefined via the redefinitions of the second at the 13th CGPM Meeting in 1967, resolution 1; the metre at the 17th CGPM meeting (1983), resolution 1; and the kilogram at the 26th CGPM Meeting (2018), resolution 1.

This is a generalized definition taken to reference the current, or one of the historical, SI unit definitions.
This definition is intended for situations when it is not possible to be more precise, e.g., in contexts where data have been collected that uses different historical SI definitions.

**Resources:**

- [Definition at the 9st CGPM meeting (1948)](https://www.bipm.org/en/committees/cg/cgpm/9-1948)
- [Definition and establishment of the SI unit system at the 11th CGPM meeting (1960), resolution 12.](https://www.bipm.org/en/committees/cg/cgpm/11-1960/resolution-12)
- [Redefinition of the second in the 13th CGPM Meeting (1967), resolution 1](https://www.bipm.org/en/committees/cg/cgpm/13-1967/resolution-1)
- [Redefinition of the kilogram in the 26th CGPM Meeting (2018), resolution 1](https://www.bipm.org/en/committees/cg/cgpm/26-2018/resolution-1)
- [Wikipedia article describing the unit](https://en.wikipedia.org/wiki/Coulomb)


**Formats:** [[JSON](coulomb.json)] [[MD](coulomb.md)]

**JSON definition:**

``` json
{
    "$schema": "https://schemas.optimade.org/meta/v1.2/optimade/physical_unit_definition.md",
    "$id": "https://schemas.optimade.org/defs/v1.2/units/si/general/coulomb",
    "title": "coulomb",
    "symbol": "coulomb",
    "display-symbol": "C",
    "description": "A unit for electric charge equal to s\u00b7A using the current, or one of the historical, definitions of the SI units.\n\n\"The coulomb is the amount of electricity transported in one second by a current of one ampere.\" [9th CGPM meeting in 1946]\n\nThe coulomb was defined at the 9th CGPM Meeting in 1946, included in SI at the 11th CGPM meeting in 1960, resolution 12, implicitly redefined via the redefinitions of the second at the 13th CGPM Meeting in 1967, resolution 1; the metre at the 17th CGPM meeting (1983), resolution 1; and the kilogram at the 26th CGPM Meeting (2018), resolution 1.\n\nThis is a generalized definition taken to reference the current, or one of the historical, SI unit definitions.\nThis definition is intended for situations when it is not possible to be more precise, e.g., in contexts where data have been collected that uses different historical SI definitions.",
    "compatibility": [
        "https://schemas.optimade.org/units/v1.2/si/1960/named/coulomb",
        "https://schemas.optimade.org/units/v1.2/si/1967/named/coulomb",
        "https://schemas.optimade.org/units/v1.2/si/1983/named/coulomb",
        "https://schemas.optimade.org/units/v1.2/si/2019/named/coulomb"
    ],
    "standard": {
        "name": "gnu units",
        "version": "3.15",
        "symbol": "coulomb"
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
            "relation": "Redefinition of the second in the 13th CGPM Meeting (1967), resolution 1",
            "resource-id": "https://www.bipm.org/en/committees/cg/cgpm/13-1967/resolution-1"
        },
        {
            "relation": "Redefinition of the kilogram in the 26th CGPM Meeting (2018), resolution 1",
            "resource-id": "https://www.bipm.org/en/committees/cg/cgpm/26-2018/resolution-1"
        },
        {
            "relation": "Wikipedia article describing the unit",
            "resource-id": "https://en.wikipedia.org/wiki/Coulomb"
        }
    ],
    "defining-relation": {
        "base-units": [
            {
                "symbol": "s",
                "id": "https://schemas.optimade.org/units/v1.2/si/general/second"
            },
            {
                "symbol": "A",
                "id": "https://schemas.optimade.org/units/v1.2/si/general/ampere"
            }
        ],
        "base-units-expression": "A*s"
    },
    "x-optimade-definition": {
        "kind": "unit",
        "format": "1.2",
        "version": "1.2.0",
        "name": "coulomb"
    }
}
```
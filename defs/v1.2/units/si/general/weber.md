# weber, Wb (unit)

This page documents an [OPTIMADE](https://www.optimade.org/) [Unit Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/defs/v1.2/units/si/general/weber`](https://schemas.optimade.org/defs/v1.2/units/si/general/weber)**  
**Definition name:** `weber`

**Unit name:** weber  
**Latin symbol:** weber  
**Display symbol:** Wb  
  
**Description:** A unit for magnetic flux equal to kg·m²·s⁻³·A⁻¹ using the current, or one of the historical, definitions of the SI units.

"The weber is the magnetic induction flux that, passing through a single-turn circuit, produces an electromotive force of one volt if it is reduced to zero in one second by uniform decay." [9th CGPM meeting in 1946]

The weber was defined at the 9th CGPM Meeting in 1946, included in SI at the 11th CGPM meeting in 1960, resolution 12, implicitly redefined via the redefinitions of the second at the 13th CGPM Meeting in 1967, resolution 1; the metre at the 17th CGPM meeting (1983), resolution 1; and the kilogram at the 26th CGPM Meeting (2018), resolution 1.

This is a generalized definition taken to reference the current, or one of the historical, SI unit definitions.
This definition is intended for situations when it is not possible to be more precise, e.g., in contexts where data have been collected that uses different historical SI definitions.

**Resources:**

- [Definition at the 9st CGPM meeting (1948)](https://www.bipm.org/en/committees/cg/cgpm/9-1948)
- [Definition and establishment of the SI unit system at the 11th CGPM meeting (1960), resolution 12.](https://www.bipm.org/en/committees/cg/cgpm/11-1960/resolution-12)
- [Redefinition of the kilogram in the 26th CGPM Meeting (2018), resolution 1](https://www.bipm.org/en/committees/cg/cgpm/26-2018/resolution-1)
- [Wikipedia article describing the unit](https://en.wikipedia.org/wiki/Weber_(unit))


**Formats:** [[JSON](weber.json)] [[MD](weber.md)]

**JSON definition:**

``` json
{
    "$schema": "https://schemas.optimade.org/meta/v1.2/optimade/physical_unit_definition.md",
    "$id": "https://schemas.optimade.org/defs/v1.2/units/si/general/weber",
    "title": "weber",
    "symbol": "weber",
    "display-symbol": "Wb",
    "description": "A unit for magnetic flux equal to kg\u00b7m\u00b2\u00b7s\u207b\u00b3\u00b7A\u207b\u00b9 using the current, or one of the historical, definitions of the SI units.\n\n\"The weber is the magnetic induction flux that, passing through a single-turn circuit, produces an electromotive force of one volt if it is reduced to zero in one second by uniform decay.\" [9th CGPM meeting in 1946]\n\nThe weber was defined at the 9th CGPM Meeting in 1946, included in SI at the 11th CGPM meeting in 1960, resolution 12, implicitly redefined via the redefinitions of the second at the 13th CGPM Meeting in 1967, resolution 1; the metre at the 17th CGPM meeting (1983), resolution 1; and the kilogram at the 26th CGPM Meeting (2018), resolution 1.\n\nThis is a generalized definition taken to reference the current, or one of the historical, SI unit definitions.\nThis definition is intended for situations when it is not possible to be more precise, e.g., in contexts where data have been collected that uses different historical SI definitions.",
    "compatibility": [
        "https://schemas.optimade.org/units/v1.2/si/1960/named/weber",
        "https://schemas.optimade.org/units/v1.2/si/1967/named/weber",
        "https://schemas.optimade.org/units/v1.2/si/1983/named/weber",
        "https://schemas.optimade.org/units/v1.2/si/2019/named/weber"
    ],
    "standard": {
        "name": "gnu units",
        "version": "3.15",
        "symbol": "weber"
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
            "relation": "Redefinition of the kilogram in the 26th CGPM Meeting (2018), resolution 1",
            "resource-id": "https://www.bipm.org/en/committees/cg/cgpm/26-2018/resolution-1"
        },
        {
            "relation": "Wikipedia article describing the unit",
            "resource-id": "https://en.wikipedia.org/wiki/Weber_(unit)"
        }
    ],
    "defining-relation": {
        "base-units": [
            {
                "symbol": "A",
                "id": "https://schemas.optimade.org/units/v1.2/si/general/ampere"
            },
            {
                "symbol": "kg",
                "id": "https://schemas.optimade.org/units/v1.2/si/general/kilogram"
            },
            {
                "symbol": "m",
                "id": "https://schemas.optimade.org/units/v1.2/si/general/metre"
            },
            {
                "symbol": "s",
                "id": "https://schemas.optimade.org/units/v1.2/si/general/second"
            }
        ],
        "base-units-expression": "A^-1*kg*m^2*s^-3"
    },
    "x-optimade-definition": {
        "kind": "unit",
        "format": "1.2",
        "version": "1.2.0",
        "name": "weber"
    }
}
```
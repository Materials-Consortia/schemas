# joule, J (unit)

This page documents an [OPTIMADE](https://www.optimade.org/) [Unit Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/defs/v1.2/units/si/1960/named/joule`](https://schemas.optimade.org/defs/v1.2/units/si/1960/named/joule.md)**  
**Definition name:** `joule`

**Unit name:** joule  
**Latin symbol:** J  
**Display symbol:** J  
  
**Description:** A derived SI unit for energy, work, and heat equal to kg·m²·s⁻² in the 1960 SI base units.

"The joule is the work produced by a newton whose point of application moves one meter in the direction of the force." [9th CGPM meeting in 1946]

**Resources:**

- [Definition at the 9st CGPM meeting (1948)](https://www.bipm.org/en/committees/cg/cgpm/9-1948)
- [Definition and establishment of the SI unit system at the 11th CGPM meeting (1960), resolution 12.](https://www.bipm.org/en/committees/cg/cgpm/11-1960/resolution-12)
- [Wikipedia article describing the unit](https://en.wikipedia.org/wiki/Joule)


**Formats:** [[JSON](joule.json)] [[MD](joule.md)]

**JSON definition:**

``` json
{
    "$id": "https://schemas.optimade.org/defs/v1.2/units/si/1960/named/joule",
    "$schema": "https://schemas.optimade.org/meta/v1.2/optimade/physical_unit_definition.json",
    "title": "joule",
    "symbol": "J",
    "display-symbol": "J",
    "description": "A derived SI unit for energy, work, and heat equal to kg\u00b7m\u00b2\u00b7s\u207b\u00b2 in the 1960 SI base units.\n\n\"The joule is the work produced by a newton whose point of application moves one meter in the direction of the force.\" [9th CGPM meeting in 1946]",
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
            "resource-id": "https://en.wikipedia.org/wiki/Joule"
        }
    ],
    "defining-relation": {
        "base-units": [
            {
                "symbol": "kg",
                "id": "https://schemas.optimade.org/defs/v1.2/units/si/1960/base/kilogram"
            },
            {
                "symbol": "m",
                "id": "https://schemas.optimade.org/defs/v1.2/units/si/1960/base/metre"
            },
            {
                "symbol": "s",
                "id": "https://schemas.optimade.org/defs/v1.2/units/si/1960/base/second"
            }
        ],
        "base-units-expression": "kg*m^2*s^-2"
    },
    "standard": {
        "name": "si",
        "year": 1960,
        "category": "named",
        "symbol": "J"
    },
    "x-optimade-definition": {
        "label": "joule_si_1960_named",
        "kind": "unit",
        "format": "1.2",
        "version": "1.2.0",
        "name": "joule"
    }
}
```
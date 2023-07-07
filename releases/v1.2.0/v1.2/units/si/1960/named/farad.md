# farad, F (unit)

This page documents an [OPTIMADE](https://www.optimade.org/) [Unit Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/defs/v1.2/units/si/1960/named/farad`](https://schemas.optimade.org/defs/v1.2/units/si/1960/named/farad.md)**  
**Definition name:** `farad`

**Unit name:** farad  
**Latin symbol:** farad  
**Display symbol:** F  
  
**Description:** A derived SI unit for electrical capacitance equal to kg⁻¹·m⁻²·s⁴·A² in the 1960 SI base units.

"The farad is the capacitance of an electric capacitor between whose plates an electric potential difference of one volt appears when it is charged with an amount of electricity equal to one coulomb." [9th CGPM meeting in 1946]

**Resources:**

- [Definition at the 9st CGPM meeting (1948)](https://www.bipm.org/en/committees/cg/cgpm/9-1948)
- [Definition and establishment of the SI unit system at the 11th CGPM meeting (1960), resolution 12.](https://www.bipm.org/en/committees/cg/cgpm/11-1960/resolution-12)
- [Wikipedia article describing the unit](https://en.wikipedia.org/wiki/Farad)


**Formats:** [[JSON](farad.json)] [[MD](farad.md)]

**JSON definition:**

``` json
{
    "$schema": "https://schemas.optimade.org/meta/v1.2/optimade/physical_unit_definition.md",
    "$id": "https://schemas.optimade.org/defs/v1.2/units/si/1960/named/farad",
    "title": "farad",
    "symbol": "farad",
    "display-symbol": "F",
    "description": "A derived SI unit for electrical capacitance equal to kg\u207b\u00b9\u00b7m\u207b\u00b2\u00b7s\u2074\u00b7A\u00b2 in the 1960 SI base units.\n\n\"The farad is the capacitance of an electric capacitor between whose plates an electric potential difference of one volt appears when it is charged with an amount of electricity equal to one coulomb.\" [9th CGPM meeting in 1946]",
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
            "resource-id": "https://en.wikipedia.org/wiki/Farad"
        }
    ],
    "defining-relation": {
        "base-units": [
            {
                "symbol": "A",
                "id": "https://schemas.optimade.org/units/v1.2/si/1960/base/ampere"
            },
            {
                "symbol": "kg",
                "id": "https://schemas.optimade.org/units/v1.2/si/1960/base/kilogram"
            },
            {
                "symbol": "m",
                "id": "https://schemas.optimade.org/units/v1.2/si/1960/base/metre"
            },
            {
                "symbol": "s",
                "id": "https://schemas.optimade.org/units/v1.2/si/1960/base/second"
            }
        ],
        "base-units-expression": "A^2*kg^-1*m^-2*s^4"
    },
    "x-optimade-definition": {
        "kind": "unit",
        "format": "1.2",
        "version": "1.2.0",
        "name": "farad"
    }
}
```
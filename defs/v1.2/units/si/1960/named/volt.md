# volt, V (unit)

This page documents an [OPTIMADE](https://www.optimade.org/) [Unit Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/defs/v1.2/units/si/1960/named/volt`](https://schemas.optimade.org/defs/v1.2/units/si/1960/named/volt.md)**  
**Definition name:** `volt`

**Unit name:** volt  
**Latin symbol:** V  
**Display symbol:** V  
  
**Description:** The volt is a derived SI unit for electric potential, voltage, and electromotive force equal to kg·m²·s⁻³·A⁻¹ in the 1960 SI base units.

"The volt is the electric potential difference that exists between two points of a conducting wire carrying a constant current of one ampere when the power dissipated between these points is equal to one watt." [9th CGPM meeting in 1946]

**Resources:**

- [Definition at the 9st CGPM meeting (1948)](https://www.bipm.org/en/committees/cg/cgpm/9-1948)
- [Definition and establishment of the SI unit system at the 11th CGPM meeting (1960), resolution 12.](https://www.bipm.org/en/committees/cg/cgpm/11-1960/resolution-12)
- [Wikipedia article describing the unit](https://en.wikipedia.org/wiki/Volt)


**Formats:** [[JSON](volt.json)] [[MD](volt.md)]

**JSON definition:**

``` json
{
    "$id": "https://schemas.optimade.org/defs/v1.2/units/si/1960/named/volt",
    "$schema": "https://schemas.optimade.org/meta/v1.2/optimade/physical_unit_definition.json",
    "title": "volt",
    "symbol": "V",
    "display-symbol": "V",
    "description": "The volt is a derived SI unit for electric potential, voltage, and electromotive force equal to kg\u00b7m\u00b2\u00b7s\u207b\u00b3\u00b7A\u207b\u00b9 in the 1960 SI base units.\n\n\"The volt is the electric potential difference that exists between two points of a conducting wire carrying a constant current of one ampere when the power dissipated between these points is equal to one watt.\" [9th CGPM meeting in 1946]",
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
            "resource-id": "https://en.wikipedia.org/wiki/Volt"
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
            },
            {
                "symbol": "A",
                "id": "https://schemas.optimade.org/defs/v1.2/units/si/1960/base/ampere"
            }
        ],
        "base-units-expression": "A^-1*kg*m^2*s^-3"
    },
    "standard": {
        "name": "si",
        "year": 1960,
        "category": "named",
        "symbol": "V"
    },
    "x-optimade-definition": {
        "label": "volt_si_1960_named",
        "kind": "unit",
        "format": "1.2",
        "version": "1.2.0",
        "name": "volt"
    }
}
```
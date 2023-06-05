# henry, H (unit)
This page documents an [OPTIMADE](https://www.optimade.org/) [Unit Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/units/v1.2.0/si/1960/named/henry`](https://schemas.optimade.org/units/v1.2.0/si/1960/named/henry)**  
**Definition name:** `henry`

**Unit name:** henry  
**Latin symbol:** H  
**Display symbol:** H  
  
**Description:** A derived SI unit for inductance equal to kg·m²·s⁻²·A⁻² in the 1960 SI base units.

"The henry is the inductance of a closed circuit in which an electromotive force of one volt is produced when the electric current passing through the circuit varies uniformly at a rate of one ampere per second." [9th CGPM meeting in 1946]

**Resources:**

- [Definition at the 9st CGPM meeting (1948)](https://www.bipm.org/en/committees/cg/cgpm/9-1948)
- [Definition and establishment of the SI unit system at the 11th CGPM meeting (1960), resolution 12.](https://www.bipm.org/en/committees/cg/cgpm/11-1960/resolution-12)
- [Wikipedia article describing the unit](https://en.wikipedia.org/wiki/Henry_(unit))


**Formats:** [[JSON](henry.json)] [[MD](henry.md)]

**JSON definition:**

``` json
{
    "title": "henry",
    "symbol": "H",
    "display-symbol": "H",
    "$id": "https://schemas.optimade.org/units/v1.2.0/si/1960/named/henry",
    "description": "A derived SI unit for inductance equal to kg\u00b7m\u00b2\u00b7s\u207b\u00b2\u00b7A\u207b\u00b2 in the 1960 SI base units.\n\n\"The henry is the inductance of a closed circuit in which an electromotive force of one volt is produced when the electric current passing through the circuit varies uniformly at a rate of one ampere per second.\" [9th CGPM meeting in 1946]",
    "standard": {
        "name": "gnu units",
        "version": "3.15",
        "symbol": "henry"
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
            "relation": "Wikipedia article describing the unit",
            "resource-id": "https://en.wikipedia.org/wiki/Henry_(unit)"
        }
    ],
    "defining-relation": {
        "base-units": [
            {
                "symbol": "A",
                "id": "https://schemas.optimade.org/units/v1.2.0/si/1960/base/ampere"
            },
            {
                "symbol": "kg",
                "id": "https://schemas.optimade.org/units/v1.2.0/si/1960/base/kilogram"
            },
            {
                "symbol": "m",
                "id": "https://schemas.optimade.org/units/v1.2.0/si/1960/base/metre"
            },
            {
                "symbol": "s",
                "id": "https://schemas.optimade.org/units/v1.2.0/si/1960/base/second"
            }
        ],
        "base-units-expression": "A^-2*kg*m^2*s^-2"
    },
    "x-optimade-definition": {
        "kind": "unit",
        "format": "1.2",
        "version": "1.2.0",
        "name": "henry"
    },
    "$schema": "https://schemas.optimade.org/meta/v1.2.0/optimade/physical_unit_definition.md"
}
```
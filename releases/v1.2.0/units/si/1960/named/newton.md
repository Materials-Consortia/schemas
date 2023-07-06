# newton, N (unit)

This page documents an [OPTIMADE](https://www.optimade.org/) [Unit Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/defs/v1.2/units/si/1960/named/newton`](https://schemas.optimade.org/defs/v1.2/units/si/1960/named/newton)**  
**Definition name:** `newton`

**Unit name:** newton  
**Latin symbol:** newton  
**Display symbol:** N  
  
**Description:** A derived SI unit for force and weight equal to kg·m·s⁻² in the 1960 SI base units.

"The newton is the force that, in one second, imparts to a mass equal to one kilogram an increase in speed of one meter per second." [9th CGPM meeting in 1946]

**Resources:**

- [Definition at the 9st CGPM meeting (1948)](https://www.bipm.org/en/committees/cg/cgpm/9-1948)
- [Definition and establishment of the SI unit system at the 11th CGPM meeting (1960), resolution 12.](https://www.bipm.org/en/committees/cg/cgpm/11-1960/resolution-12)
- [Wikipedia article describing the unit](https://en.wikipedia.org/wiki/Newton_(unit))


**Formats:** [[JSON](newton.json)] [[MD](newton.md)]

**JSON definition:**

``` json
{
    "$schema": "https://schemas.optimade.org/meta/v1.2/optimade/physical_unit_definition.md",
    "$id": "https://schemas.optimade.org/defs/v1.2/units/si/1960/named/newton",
    "title": "newton",
    "symbol": "newton",
    "display-symbol": "N",
    "description": "A derived SI unit for force and weight equal to kg\u00b7m\u00b7s\u207b\u00b2 in the 1960 SI base units.\n\n\"The newton is the force that, in one second, imparts to a mass equal to one kilogram an increase in speed of one meter per second.\" [9th CGPM meeting in 1946]\n",
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
            "resource-id": "https://en.wikipedia.org/wiki/Newton_(unit)"
        }
    ],
    "defining-relation": {
        "base-units": [
            {
                "symbol": "kg",
                "id": "https://schemas.optimade.org/units/v1.2/si/1960/base/kilogram"
            },
            {
                "symbol": "m",
                "id": "https://schemas.optimade.org/units/v1.2/si/1960/base/meter"
            },
            {
                "symbol": "s",
                "id": "https://schemas.optimade.org/units/v1.2/si/1960/base/second"
            }
        ],
        "base-units-expression": "kg*m*s^-2"
    },
    "x-optimade-definition": {
        "kind": "unit",
        "format": "1.2",
        "version": "1.2.0",
        "name": "newton"
    }
}
```
# newton, N (unit)

This page documents an [OPTIMADE](https://www.optimade.org/) [Unit Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/defs/v1.2/units/si/1983/named/newton`](https://schemas.optimade.org/defs/v1.2/units/si/1983/named/newton)**  
**Definition name:** `newton`

**Unit name:** newton  
**Latin symbol:** newton  
**Display symbol:** N  
  
**Description:** The newton is a derived SI unit for force and weight equal to kg·m·s⁻² in 1983 SI units.

"The newton is the force that, in one second, imparts to a mass equal to one kilogram an increase in speed of one meter per second." [9th CGPM meeting in 1946]

The newton was defined at the 9th CGPM Meeting in 1946, included in SI at the 11th CGPM meeting in 1960, resolution 12, implicitly redefined via the redefinition of the second at the 13th CGPM Meeting in 1967, resolution 1, and again implicity redefined via the redefinition of the metre at the 17th CGPM meeting (1983), resolution 1.

**Resources:**

- [Definition and establishment of the SI unit system at the 11th CGPM meeting (1960), resolution 12.](https://www.bipm.org/en/committees/cg/cgpm/11-1960/resolution-12)
- [Redefinition of the second in the 13th CGPM Meeting (1967), resolution 1](https://www.bipm.org/en/committees/cg/cgpm/13-1967/resolution-1)
- [Redefinition of the metre at the 17th CGPM meeting (1983), resolution 1](https://www.bipm.org/en/committees/cg/cgpm/17-1983/resolution-1)
- [Wikipedia article describing the unit](https://en.wikipedia.org/wiki/Newton_(unit))


**Formats:** [[JSON](newton.json)] [[MD](newton.md)]

**JSON definition:**

``` json
{
    "$schema": "https://schemas.optimade.org/meta/v1.2/optimade/physical_unit_definition.md",
    "$id": "https://schemas.optimade.org/defs/v1.2/units/si/1983/named/newton",
    "title": "newton",
    "symbol": "newton",
    "display-symbol": "N",
    "description": "The newton is a derived SI unit for force and weight equal to kg\u00b7m\u00b7s\u207b\u00b2 in 1983 SI units.\n\n\"The newton is the force that, in one second, imparts to a mass equal to one kilogram an increase in speed of one meter per second.\" [9th CGPM meeting in 1946]\n\nThe newton was defined at the 9th CGPM Meeting in 1946, included in SI at the 11th CGPM meeting in 1960, resolution 12, implicitly redefined via the redefinition of the second at the 13th CGPM Meeting in 1967, resolution 1, and again implicity redefined via the redefinition of the metre at the 17th CGPM meeting (1983), resolution 1.",
    "standard": {
        "name": "gnu units",
        "version": "3.15",
        "symbol": "newton"
    },
    "resources": [
        {
            "relation": "Definition and establishment of the SI unit system at the 11th CGPM meeting (1960), resolution 12.",
            "resource-id": "https://www.bipm.org/en/committees/cg/cgpm/11-1960/resolution-12"
        },
        {
            "relation": "Redefinition of the second in the 13th CGPM Meeting (1967), resolution 1",
            "resource-id": "https://www.bipm.org/en/committees/cg/cgpm/13-1967/resolution-1"
        },
        {
            "relation": "Redefinition of the metre at the 17th CGPM meeting (1983), resolution 1",
            "resource-id": "https://www.bipm.org/en/committees/cg/cgpm/17-1983/resolution-1"
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
                "id": "https://schemas.optimade.org/units/v1.2/si/1983/base/metre"
            },
            {
                "symbol": "s",
                "id": "https://schemas.optimade.org/units/v1.2/si/1967/base/second"
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
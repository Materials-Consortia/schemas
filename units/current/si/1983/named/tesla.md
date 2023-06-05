# tesla, T (unit)
This page documents an [OPTIMADE](https://www.optimade.org/) [Unit Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/units/v1.2.0/si/1983/named/tesla`](https://schemas.optimade.org/units/v1.2.0/si/1983/named/tesla)**  
**Definition name:** `tesla`

**Unit name:** tesla  
**Latin symbol:** tesla  
**Display symbol:** T  
  
**Description:** A derived SI unit for magnetic flux density equal to kg·s⁻²·A⁻¹ in the 1983 SI units.

The tesla was defined as 1 Wb/m in the introduction of the SI unit system the 11th CGPM Meeting in 1960, resolution 12, implicitly redefined via the redefinition of the second at the 13th CGPM Meeting in 1967, resolution 1, and again implicitly redefined with the redefinition of the ampere (implcitly via the redefinition of the metre) at the 17th CGPM Meeting in 1983, resolution 1.

**Resources:**

- [Definition and establishment of the SI unit system at the 11th CGPM meeting (1960), resolution 12.](https://www.bipm.org/en/committees/cg/cgpm/11-1960/resolution-12)
- [Redefinition of the metre at the 17th CGPM meeting (1983), resolution 1](https://www.bipm.org/en/committees/cg/cgpm/17-1983/resolution-1)
- [Wikipedia article describing the unit](https://en.wikipedia.org/wiki/Tesla_(unit))


**Formats:** [[JSON](tesla.json)] [[MD](tesla.md)]

**JSON definition:**

``` json
{
    "$id": "https://schemas.optimade.org/units/v1.2.0/si/1983/named/tesla",
    "title": "tesla",
    "symbol": "tesla",
    "display-symbol": "T",
    "description": "A derived SI unit for magnetic flux density equal to kg\u00b7s\u207b\u00b2\u00b7A\u207b\u00b9 in the 1983 SI units.\n\nThe tesla was defined as 1 Wb/m in the introduction of the SI unit system the 11th CGPM Meeting in 1960, resolution 12, implicitly redefined via the redefinition of the second at the 13th CGPM Meeting in 1967, resolution 1, and again implicitly redefined with the redefinition of the ampere (implcitly via the redefinition of the metre) at the 17th CGPM Meeting in 1983, resolution 1.",
    "standard": {
        "name": "gnu units",
        "version": "3.15",
        "symbol": "tesla"
    },
    "resources": [
        {
            "relation": "Definition and establishment of the SI unit system at the 11th CGPM meeting (1960), resolution 12.",
            "resource-id": "https://www.bipm.org/en/committees/cg/cgpm/11-1960/resolution-12"
        },
        {
            "relation": "Redefinition of the metre at the 17th CGPM meeting (1983), resolution 1",
            "resource-id": "https://www.bipm.org/en/committees/cg/cgpm/17-1983/resolution-1"
        },
        {
            "relation": "Wikipedia article describing the unit",
            "resource-id": "https://en.wikipedia.org/wiki/Tesla_(unit)"
        }
    ],
    "defining-relation": {
        "base-units": [
            {
                "symbol": "A",
                "id": "https://schemas.optimade.org/units/v1.2.0/si/1983/base/ampere"
            },
            {
                "symbol": "kg",
                "id": "https://schemas.optimade.org/units/v1.2.0/si/1960/base/kilogram"
            },
            {
                "symbol": "s",
                "id": "https://schemas.optimade.org/units/v1.2.0/si/1967/base/second"
            }
        ],
        "base-units-expression": "A^-1*kg*s^-2"
    },
    "x-optimade-definition": {
        "kind": "unit",
        "format": "1.2",
        "version": "1.2.0",
        "name": "tesla"
    },
    "$schema": "https://schemas.optimade.org/meta/v1.2.0/optimade/physical_unit_definition.md"
}
```
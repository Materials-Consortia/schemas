# tesla, T (unit)

This page documents an [OPTIMADE](https://www.optimade.org/) [Unit Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/defs/v1.2/units/si/1960/named/tesla`](https://schemas.optimade.org/defs/v1.2/units/si/1960/named/tesla.md)**  
**Definition name:** `tesla`

**Unit name:** tesla  
**Latin symbol:** T  
**Display symbol:** T  
  
**Description:** The tesla is a derived SI unit for magnetic flux density equal to kg·s⁻²·A⁻¹ in the 1960 SI base units.

The tesla was defined as 1 Wb/m in the introduction of the SI unit system at the 11th CGPM Meeting in 1960.

**Resources:**

- [Definition and establishment of the SI unit system at the 11th CGPM meeting (1960), resolution 12.](https://www.bipm.org/en/committees/cg/cgpm/11-1960/resolution-12)
- [Wikipedia article describing the unit](https://en.wikipedia.org/wiki/Tesla_(unit))


**Formats:** [[JSON](tesla.json)] [[MD](tesla.md)]

**JSON definition:**

``` json
{
    "$id": "https://schemas.optimade.org/defs/v1.2/units/si/1960/named/tesla",
    "$schema": "https://schemas.optimade.org/meta/v1.2/optimade/physical_unit_definition.json",
    "title": "tesla",
    "symbol": "T",
    "display-symbol": "T",
    "description": "The tesla is a derived SI unit for magnetic flux density equal to kg\u00b7s\u207b\u00b2\u00b7A\u207b\u00b9 in the 1960 SI base units.\n\nThe tesla was defined as 1 Wb/m in the introduction of the SI unit system at the 11th CGPM Meeting in 1960.",
    "resources": [
        {
            "relation": "Definition and establishment of the SI unit system at the 11th CGPM meeting (1960), resolution 12.",
            "resource-id": "https://www.bipm.org/en/committees/cg/cgpm/11-1960/resolution-12"
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
                "id": "https://schemas.optimade.org/defs/v1.2/units/si/1960/base/ampere"
            },
            {
                "symbol": "kg",
                "id": "https://schemas.optimade.org/defs/v1.2/units/si/1960/base/kilogram"
            },
            {
                "symbol": "s",
                "id": "https://schemas.optimade.org/defs/v1.2/units/si/1960/base/second"
            }
        ],
        "base-units-expression": "A^-1*kg*s^-2"
    },
    "standard": {
        "name": "si",
        "year": 1960,
        "category": "named",
        "symbol": "T"
    },
    "x-optimade-definition": {
        "label": "tesla_si_1960_named",
        "kind": "unit",
        "format": "1.2",
        "version": "1.2.0",
        "name": "tesla"
    }
}
```
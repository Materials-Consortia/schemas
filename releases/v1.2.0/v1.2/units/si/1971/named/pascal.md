# pascal, Pa (unit)

This page documents an [OPTIMADE](https://www.optimade.org/) [Unit Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/defs/v1.2/units/si/1971/named/pascal`](https://schemas.optimade.org/defs/v1.2/units/si/1971/named/pascal.md)**  
**Definition name:** `pascal`

**Unit name:** pascal  
**Latin symbol:** Pa  
**Display symbol:** Pa  
  
**Description:** A derived SI unit for pressure and stress equal to kg·m⁻¹·s⁻² using the 1967 SI base units, defined at the 14th CGPM Meeting (1971).

"The International Committee will ask the General Conference to approve two special names: pascal (symbol Pa) for the SI unit of pressure (N/m²), [...]" [14th CGPM Meeting (1971)].

**Resources:**

- [Definition at the 14th CGPM Meeting (1971)](https://www.bipm.org/en/committees/cg/cgpm/14-1971)
- [Wikipedia article describing the unit](https://en.wikipedia.org/wiki/Pascal_(unit))


**Formats:** [[JSON](pascal.json)] [[MD](pascal.md)]

**JSON definition:**

``` json
{
    "$schema": "https://schemas.optimade.org/meta/v1.2/optimade/physical_unit_definition.md",
    "$id": "https://schemas.optimade.org/defs/v1.2/units/si/1971/named/pascal",
    "title": "pascal",
    "symbol": "Pa",
    "display-symbol": "Pa",
    "description": "A derived SI unit for pressure and stress equal to kg\u00b7m\u207b\u00b9\u00b7s\u207b\u00b2 using the 1967 SI base units, defined at the 14th CGPM Meeting (1971).\n\n\"The International Committee will ask the General Conference to approve two special names: pascal (symbol Pa) for the SI unit of pressure (N/m\u00b2), [...]\" [14th CGPM Meeting (1971)].",
    "resources": [
        {
            "relation": "Definition at the 14th CGPM Meeting (1971)",
            "resource-id": "https://www.bipm.org/en/committees/cg/cgpm/14-1971"
        },
        {
            "relation": "Wikipedia article describing the unit",
            "resource-id": "https://en.wikipedia.org/wiki/Pascal_(unit)"
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
                "id": "https://schemas.optimade.org/units/v1.2/si/1960/base/metre"
            },
            {
                "symbol": "s",
                "id": "https://schemas.optimade.org/units/v1.2/si/1967/base/second"
            }
        ],
        "base-units-expression": "kg*m^-1*s^-2"
    },
    "x-optimade-definition": {
        "kind": "unit",
        "format": "1.2",
        "version": "1.2.0",
        "name": "pascal"
    }
}
```
# pascal, Pa (unit)
This page documents an [OPTIMADE](https://www.optimade.org/) [Unit Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/units/v1.2.0/si/2019/named/pascal`](https://schemas.optimade.org/units/v1.2.0/si/2019/named/pascal)**  
**Definition name:** `pascal`

**Unit name:** pascal  
**Latin symbol:** Pa  
**Display symbol:** Pa  
  
**Description:** A derived SI unit for pressure and stress equal to kg·m⁻¹·s⁻² using the 2019 SI units.

"The International Committee will ask the General Conference to approve two special names: pascal (symbol Pa) for the SI unit of pressure (N/m²), [...]" [14th CGPM Meeting (1971)].

The pascal was defined at the 14th CGPM Meeting in 1971 and implicitly redefined via the redefinitions of the metre at the 17th CGPM Meeting in 1983, resolution 1, and the kilogram at the 26th CGPM Meeting (2018), resolution 1.

**Resources:**

- [Definition at the 14th CGPM Meeting (1971)](https://www.bipm.org/en/committees/cg/cgpm/14-1971)
- [Wikipedia article describing the unit](https://en.wikipedia.org/wiki/Pascal_(unit))
- [Redefinition of the metre at the 17th CGPM meeting (1983), resolution 1](https://www.bipm.org/en/committees/cg/cgpm/17-1983/resolution-1)
- [Redefinition of the kilogram at the 26th CGPM Meeting (2018), resolution 1](https://www.bipm.org/en/committees/cg/cgpm/26-2018/resolution-1)


**Formats:** [[JSON](pascal.json)] [[MD](pascal.md)]

**JSON definition:**

``` json
{
    "$id": "https://schemas.optimade.org/units/v1.2.0/si/2019/named/pascal",
    "title": "pascal",
    "symbol": "Pa",
    "display-symbol": "Pa",
    "description": "A derived SI unit for pressure and stress equal to kg\u00b7m\u207b\u00b9\u00b7s\u207b\u00b2 using the 2019 SI units.\n\n\"The International Committee will ask the General Conference to approve two special names: pascal (symbol Pa) for the SI unit of pressure (N/m\u00b2), [...]\" [14th CGPM Meeting (1971)].\n\nThe pascal was defined at the 14th CGPM Meeting in 1971 and implicitly redefined via the redefinitions of the metre at the 17th CGPM Meeting in 1983, resolution 1, and the kilogram at the 26th CGPM Meeting (2018), resolution 1.",
    "standard": {
        "name": "gnu units",
        "version": "3.15",
        "symbol": "pascal"
    },
    "resources": [
        {
            "relation": "Definition at the 14th CGPM Meeting (1971)",
            "resource-id": "https://www.bipm.org/en/committees/cg/cgpm/14-1971"
        },
        {
            "relation": "Wikipedia article describing the unit",
            "resource-id": "https://en.wikipedia.org/wiki/Pascal_(unit)"
        },
        {
            "relation": "Redefinition of the metre at the 17th CGPM meeting (1983), resolution 1",
            "resource-id": "https://www.bipm.org/en/committees/cg/cgpm/17-1983/resolution-1"
        },
        {
            "relation": "Redefinition of the kilogram at the 26th CGPM Meeting (2018), resolution 1",
            "resource-id": "https://www.bipm.org/en/committees/cg/cgpm/26-2018/resolution-1"
        }
    ],
    "defining-relation": {
        "base-units": [
            {
                "symbol": "kg",
                "id": "https://schemas.optimade.org/units/v1.2.0/si/2019/base/kilogram"
            },
            {
                "symbol": "m",
                "id": "https://schemas.optimade.org/units/v1.2.0/si/1983/base/metre"
            },
            {
                "symbol": "s",
                "id": "https://schemas.optimade.org/units/v1.2.0/si/1967/base/second"
            }
        ],
        "base-units-expression": "kg*m^-1*s^-2"
    },
    "x-optimade-definition": {
        "kind": "unit",
        "format": "1.2",
        "version": "1.2.0",
        "name": "pascal"
    },
    "$schema": "https://schemas.optimade.org/meta/v1.2.0/optimade/physical_unit_definition.md"
}
```
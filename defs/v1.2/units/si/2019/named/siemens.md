# siemens, S (unit)

This page documents an [OPTIMADE](https://www.optimade.org/) [Unit Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/defs/v1.2/units/si/2019/named/siemens`](https://schemas.optimade.org/defs/v1.2/units/si/2019/named/siemens)**  
**Definition name:** `siemens`

**Unit name:** siemens  
**Latin symbol:** S  
**Display symbol:** S  
  
**Description:** A derived SI unit for electrical conductance equal to kg⁻¹·m⁻²·s³·A² using the 2019 SI base units.

"The International Committee will ask the General Conference to approve two special names: [...] siemens (symbol S) for the SI unit of conductance (Ω⁻¹)." [14th CGPM Meeting (1971)].

The siemens was defined at the 14th CGPM Meeting in 1971 and implicitly redefined via the redefinitions of the meter at the 17th CGPM Meeting in 1983, resolution 1 and the kilogram at the 26th CGPM Meeting (2018), resolution 1.

**Resources:**

- [Definition at the 14th CGPM Meeting (1971)](https://www.bipm.org/en/committees/cg/cgpm/14-1971)
- [Redefinition of the metre at the 17th CGPM meeting (1983), resolution 1](https://www.bipm.org/en/committees/cg/cgpm/17-1983/resolution-1)
- [Redefinition of the kilogram at the 26th CGPM Meeting (2018), resolution 1](https://www.bipm.org/en/committees/cg/cgpm/26-2018/resolution-1)
- [Wikipedia article describing the unit](https://en.wikipedia.org/wiki/Siemens_(unit))


**Formats:** [[JSON](siemens.json)] [[MD](siemens.md)]

**JSON definition:**

``` json
{
    "$schema": "https://schemas.optimade.org/meta/v1.2/optimade/physical_unit_definition.md",
    "$id": "https://schemas.optimade.org/defs/v1.2/units/si/2019/named/siemens",
    "title": "siemens",
    "symbol": "S",
    "display-symbol": "S",
    "description": "A derived SI unit for electrical conductance equal to kg\u207b\u00b9\u00b7m\u207b\u00b2\u00b7s\u00b3\u00b7A\u00b2 using the 2019 SI base units.\n\n\"The International Committee will ask the General Conference to approve two special names: [...] siemens (symbol S) for the SI unit of conductance (\u03a9\u207b\u00b9).\" [14th CGPM Meeting (1971)].\n\nThe siemens was defined at the 14th CGPM Meeting in 1971 and implicitly redefined via the redefinitions of the meter at the 17th CGPM Meeting in 1983, resolution 1 and the kilogram at the 26th CGPM Meeting (2018), resolution 1.",
    "standard": {
        "name": "gnu units",
        "version": "3.15",
        "symbol": "siemens"
    },
    "resources": [
        {
            "relation": "Definition at the 14th CGPM Meeting (1971)",
            "resource-id": "https://www.bipm.org/en/committees/cg/cgpm/14-1971"
        },
        {
            "relation": "Redefinition of the metre at the 17th CGPM meeting (1983), resolution 1",
            "resource-id": "https://www.bipm.org/en/committees/cg/cgpm/17-1983/resolution-1"
        },
        {
            "relation": "Redefinition of the kilogram at the 26th CGPM Meeting (2018), resolution 1",
            "resource-id": "https://www.bipm.org/en/committees/cg/cgpm/26-2018/resolution-1"
        },
        {
            "relation": "Wikipedia article describing the unit",
            "resource-id": "https://en.wikipedia.org/wiki/Siemens_(unit)"
        }
    ],
    "defining-relation": {
        "base-units": [
            {
                "symbol": "A",
                "id": "https://schemas.optimade.org/units/v1.2/si/2019/base/ampere"
            },
            {
                "symbol": "kg",
                "id": "https://schemas.optimade.org/units/v1.2/si/2019/base/kilogram"
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
        "base-units-expression": "A^2*kg^-1*m^-2*s^3"
    },
    "x-optimade-definition": {
        "kind": "unit",
        "format": "1.2",
        "version": "1.2.0",
        "name": "siemens"
    }
}
```
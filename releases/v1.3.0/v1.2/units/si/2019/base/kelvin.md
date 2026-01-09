# kelvin, K (unit)

This page documents an [OPTIMADE](https://www.optimade.org/) [Unit Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/defs/v1.2/units/si/2019/base/kelvin`](https://schemas.optimade.org/defs/v1.2/units/si/2019/base/kelvin.md)**  
**Definition name:** `kelvin`

**Unit name:** kelvin  
**Latin symbol:** K  
**Display symbol:** K  
  
**Description:** The SI base unit of thermodynamic temperature defined by fixing the value of the Boltzmann constant as defined at the 26th CGPM Meeting (2018) and adopted into SI in 2019.

"The kelvin, symbol K, is the SI unit of thermodynamic temperature. It is defined by taking the fixed numerical value of the Boltzmann constant k to be 1.380649×10⁻²³ when expressed in the unit J⋅K⁻¹, which is equal to kg⋅m²⋅s⁻²⋅K⁻¹, where the kilogram, metre and second are defined in terms of \(h\), \(c\) and \(\Delta \nu_\textrm{Cs}\)." [26th CGPM Meeting (2018), resolution 1].

This definition references the 2019 SI derived joule unit (https://schemas.optimade.org/defs/v1.2/units/si/2019/named/joule).

**Resources:**

- [Definition in the 26th CGPM Meeting in 2018, resolution 1](https://www.bipm.org/en/committees/cg/cgpm/26-2018/resolution-1)
- [Definition in the International System of Units (SI), 9th Edition](https://www.bipm.org/en/publications/si-brochure)
- [Wikipedia article describing the unit](https://en.wikipedia.org/wiki/Kelvin)


**Formats:** [[JSON](kelvin.json)] [[MD](kelvin.md)]

**JSON definition:**

``` json
{
    "$id": "https://schemas.optimade.org/defs/v1.2/units/si/2019/base/kelvin",
    "$schema": "https://schemas.optimade.org/meta/v1.2/optimade/physical_unit_definition.json",
    "title": "kelvin",
    "symbol": "K",
    "display-symbol": "K",
    "description": "The SI base unit of thermodynamic temperature defined by fixing the value of the Boltzmann constant as defined at the 26th CGPM Meeting (2018) and adopted into SI in 2019.\n\n\"The kelvin, symbol K, is the SI unit of thermodynamic temperature. It is defined by taking the fixed numerical value of the Boltzmann constant k to be 1.380649\u00d710\u207b\u00b2\u00b3 when expressed in the unit J\u22c5K\u207b\u00b9, which is equal to kg\u22c5m\u00b2\u22c5s\u207b\u00b2\u22c5K\u207b\u00b9, where the kilogram, metre and second are defined in terms of \\(h\\), \\(c\\) and \\(\\Delta \\nu_\\textrm{Cs}\\).\" [26th CGPM Meeting (2018), resolution 1].\n\nThis definition references the 2019 SI derived joule unit (https://schemas.optimade.org/defs/v1.2/units/si/2019/named/joule).",
    "resources": [
        {
            "relation": "Definition in the 26th CGPM Meeting in 2018, resolution 1",
            "resource-id": "https://www.bipm.org/en/committees/cg/cgpm/26-2018/resolution-1"
        },
        {
            "relation": "Definition in the International System of Units (SI), 9th Edition",
            "resource-id": "https://www.bipm.org/en/publications/si-brochure"
        },
        {
            "relation": "Wikipedia article describing the unit",
            "resource-id": "https://en.wikipedia.org/wiki/Kelvin"
        }
    ],
    "standard": {
        "name": "si",
        "year": 2019,
        "category": "base",
        "symbol": "K"
    },
    "x-optimade-definition": {
        "label": "kelvin_si_2019_base",
        "kind": "unit",
        "format": "1.2",
        "version": "1.2.0",
        "name": "kelvin"
    }
}
```
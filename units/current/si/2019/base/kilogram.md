# kilogram, kg (unit)
This page documents an [OPTIMADE](https://www.optimade.org/) [Unit Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/units/v1.2.0/si/2019/base/kilogram`](https://schemas.optimade.org/units/v1.2.0/si/2019/base/kilogram)**  
**Definition name:** `kilogram`

**Unit name:** kilogram  
**Latin symbol:** kg  
**Display symbol:** kg  
  
**Description:** The SI base unit of mass defined by fixing the value of the Planck constant as defined at the 26th CGPM Meeting (2018) and adopted into SI in 2019.

"The kilogram, symbol kg, is the SI unit of mass. It is defined by taking the fixed numerical value of the Planck constant \(h\) to be 6.62607015×10⁻³⁴ when expressed in the unit J⋅s, which is equal to kg⋅m²⋅s⁻¹, where the metre and the second are defined in terms of \(c\) and \(\Delta \nu_\textrm{Cs}\)." [26th CGPM Meeting (2018), resolution 1].

This definition references:

- The 2019 SI derived joule unit (https://schemas.optimade.org/units/v1.2.0/si/2019/named/joule).
- The 1967 SI base second unit (https://schemas.optimade.org/units/v1.2.0/si/1967/base/second).

**Resources:**

- [Definition in the 26th CGPM Meeting in 2018, resolution 1](https://www.bipm.org/en/committees/cg/cgpm/26-2018/resolution-1)
- [Definition in the International System of Units (SI), 9th Edition](https://www.bipm.org/en/publications/si-brochure)
- [Wikipedia article describing the unit](https://en.wikipedia.org/wiki/Kilogram)


**Formats:** [[JSON](kilogram.json)] [[MD](kilogram.md)]

**JSON definition:**

``` json
{
    "$id": "https://schemas.optimade.org/units/v1.2.0/si/2019/base/kilogram",
    "title": "kilogram",
    "symbol": "kg",
    "display-symbol": "kg",
    "description": "The SI base unit of mass defined by fixing the value of the Planck constant as defined at the 26th CGPM Meeting (2018) and adopted into SI in 2019.\n\n\"The kilogram, symbol kg, is the SI unit of mass. It is defined by taking the fixed numerical value of the Planck constant \\(h\\) to be 6.62607015\u00d710\u207b\u00b3\u2074 when expressed in the unit J\u22c5s, which is equal to kg\u22c5m\u00b2\u22c5s\u207b\u00b9, where the metre and the second are defined in terms of \\(c\\) and \\(\\Delta \\nu_\\textrm{Cs}\\).\" [26th CGPM Meeting (2018), resolution 1].\n\nThis definition references:\n\n- The 2019 SI derived joule unit (https://schemas.optimade.org/units/v1.2.0/si/2019/named/joule).\n- The 1967 SI base second unit (https://schemas.optimade.org/units/v1.2.0/si/1967/base/second).",
    "standard": {
        "name": "gnu units",
        "version": "3.15",
        "symbol": "kilogram"
    },
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
            "resource-id": "https://en.wikipedia.org/wiki/Kilogram"
        }
    ],
    "x-optimade-definition": {
        "kind": "unit",
        "format": "1.2",
        "version": "1.2.0",
        "name": "kilogram"
    },
    "$schema": "https://schemas.optimade.org/meta/v1.2.0/optimade/physical_unit_definition.md"
}
```
# ampere, A (unit)

This page documents an [OPTIMADE](https://www.optimade.org/) [Unit Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/defs/v1.2/units/si/2019/base/ampere`](https://schemas.optimade.org/defs/v1.2/units/si/2019/base/ampere.md)**  
**Definition name:** `ampere`

**Unit name:** ampere  
**Latin symbol:** A  
**Display symbol:** A  
  
**Description:** The SI base unit of electric current defined by fixing the value of the elementary charge as defined at the 26th CGPM Meeting (2018) and adopted into SI in 2019.

"The ampere, symbol A, is the SI unit of electric current. It is defined by taking the fixed numerical value of the elementary charge \(e\) to be 1.602176634×10⁻¹⁹ when expressed in the unit C, which is equal to A⋅s, where the second is defined in terms of \(\Delta \nu_\textrm{Cs}\)." [26th CGPM Meeting (2018), resolution 1].

This definition references the 1976 SI base second unit (https://schemas.optimade.org/defs/v1.2/units/si/1976/base/second).

**Resources:**

- [Definition in the 26th CGPM Meeting in 2018, resolution 1](https://www.bipm.org/en/committees/cg/cgpm/26-2018/resolution-1)
- [Definition in the International System of Units (SI), 9th Edition](https://www.bipm.org/en/publications/si-brochure)
- [Wikipedia article describing the unit](https://en.wikipedia.org/wiki/Ampere)


**Formats:** [[JSON](ampere.json)] [[MD](ampere.md)]

**JSON definition:**

``` json
{
    "$id": "https://schemas.optimade.org/defs/v1.2/units/si/2019/base/ampere",
    "$schema": "https://schemas.optimade.org/meta/v1.2/optimade/physical_unit_definition.json",
    "title": "ampere",
    "symbol": "A",
    "display-symbol": "A",
    "description": "The SI base unit of electric current defined by fixing the value of the elementary charge as defined at the 26th CGPM Meeting (2018) and adopted into SI in 2019.\n\n\"The ampere, symbol A, is the SI unit of electric current. It is defined by taking the fixed numerical value of the elementary charge \\(e\\) to be 1.602176634\u00d710\u207b\u00b9\u2079 when expressed in the unit C, which is equal to A\u22c5s, where the second is defined in terms of \\(\\Delta \\nu_\\textrm{Cs}\\).\" [26th CGPM Meeting (2018), resolution 1].\n\nThis definition references the 1976 SI base second unit (https://schemas.optimade.org/defs/v1.2/units/si/1976/base/second).",
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
            "resource-id": "https://en.wikipedia.org/wiki/Ampere"
        }
    ],
    "standard": {
        "name": "si",
        "year": 2019,
        "category": "base",
        "symbol": "A"
    },
    "x-optimade-definition": {
        "label": "ampere_si_2019_base",
        "kind": "unit",
        "format": "1.2",
        "version": "1.2.0",
        "name": "ampere"
    }
}
```
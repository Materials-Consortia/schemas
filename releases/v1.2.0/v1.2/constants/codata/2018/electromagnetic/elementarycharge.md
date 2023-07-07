# Elementary charge, \(e\) (unit)

This page documents an [OPTIMADE](https://www.optimade.org/) [Unit Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/defs/v1.2/constants/codata/2018/electromagnetic/elementarycharge`](https://schemas.optimade.org/defs/v1.2/constants/codata/2018/electromagnetic/elementarycharge.md)**  
**Definition name:** `elementarycharge`

**Unit name:** Elementary charge  
**Latin symbol:** e  
**Display symbol:** \(e\)  
  
**Description:** The CODATA 2018 value for the absolute value of the charge of the electron.

This constant is described in Rev. Mod. Phys. 93, 025010 (2021) as "Absolute value of the charge of the electron and one of the seven defining constants of the SI".
It is exactly 1.602176634·10⁻¹⁹ C following the 2019 redefinition of the SI base units.

**Resources:**

- [Definition in: E. Tiesinga, P. J. Mohr, D. B. Newell, and B. N. Taylor, Rev. Mod. Phys. 93, 025010 (2021)](https://doi.org/10.1103/RevModPhys.93.025010)
- [Wikipedia article describing the constant](https://en.wikipedia.org/wiki/Elementary_charge)


**Formats:** [[JSON](elementarycharge.json)] [[MD](elementarycharge.md)]

**JSON definition:**

``` json
{
    "$schema": "https://schemas.optimade.org/meta/v1.2/optimade/constant_definition.md",
    "$id": "https://schemas.optimade.org/defs/v1.2/constants/codata/2018/electromagnetic/elementarycharge",
    "title": "Elementary charge",
    "symbol": "e",
    "display-symbol": "\\(e\\)",
    "description": "The CODATA 2018 value for the absolute value of the charge of the electron.\n\nThis constant is described in Rev. Mod. Phys. 93, 025010 (2021) as \"Absolute value of the charge of the electron and one of the seven defining constants of the SI\".\nIt is exactly 1.602176634\u00b710\u207b\u00b9\u2079 C following the 2019 redefinition of the SI base units.",
    "resources": [
        {
            "relation": "Definition in: E. Tiesinga, P. J. Mohr, D. B. Newell, and B. N. Taylor, Rev. Mod. Phys. 93, 025010 (2021)",
            "resource-id": "https://doi.org/10.1103/RevModPhys.93.025010"
        },
        {
            "relation": "Wikipedia article describing the constant",
            "resource-id": "https://en.wikipedia.org/wiki/Elementary_charge"
        }
    ],
    "defining-relation": {
        "base-units": [
            {
                "symbol": "coulomb",
                "id": "https://schema.optimade.org/units/si/2019/named/coulomb"
            }
        ],
        "base-units-expression": "coulomb",
        "scale": {
            "numerator": 1602176634,
            "exponent": -28
        }
    },
    "x-optimade-definition": {
        "kind": "unit",
        "format": "1.2",
        "version": "1.2.0",
        "name": "elementarycharge"
    }
}
```
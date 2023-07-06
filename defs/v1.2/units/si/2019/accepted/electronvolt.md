# electron volt, eV (unit)

This page documents an [OPTIMADE](https://www.optimade.org/) [Unit Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/defs/v1.2/units/si/2019/accepted/electronvolt`](https://schemas.optimade.org/defs/v1.2/units/si/2019/accepted/electronvolt)**  
**Definition name:** `electronvolt`

**Unit name:** electron volt  
**Latin symbol:** eV  
**Display symbol:** eV  
  
**Description:** A unit of energy equal to the amount of kinetic energy acquired by an electron as it accelerates through a 1 volt potential difference in a vacuum using the 2019 SI units.

The electronvolt appear in The International System of Units (SI), 1th ed. (1970) defined as "1 electronvolt is the energy acquired by an electron after traversing a potential difference of 1 V in a vacuum; 1 eV = 1.60219×10⁻¹⁹ J approximately."
This definition makes the unit equal to 1 volt times the value of the elementary charge.
In the 2019 redefinition of the SI units the elementary charge is exactly 1.602176634·10⁻¹⁹ C, making the electron volt exactly equal to 1.602176634·10⁻¹⁹ J.
The International System of Units (SI), 9th ed. (2019) accordingly notes the exact relationship with the SI 2019 derived unit joule as "1 eV = 1.602176634·10⁻¹⁹ J" but retains the definition from 1970 in a footnote.

The unit is categorized in The International System of Units (SI), 9th ed. (2019) as "Non-SI units accepted for use with the SI units".

**Resources:**

- [Definition in the International System of Units (SI), 9th Edition](https://www.bipm.org/en/publications/si-brochure)
- [Wikipedia article describing the unit](https://en.wikipedia.org/wiki/Electronvolt)


**Formats:** [[JSON](electronvolt.json)] [[MD](electronvolt.md)]

**JSON definition:**

``` json
{
    "$schema": "https://schemas.optimade.org/meta/v1.2/optimade/physical_unit_definition.md",
    "$id": "https://schemas.optimade.org/defs/v1.2/units/si/2019/accepted/electronvolt",
    "title": "electron volt",
    "symbol": "eV",
    "display-symbol": "eV",
    "description": "A unit of energy equal to the amount of kinetic energy acquired by an electron as it accelerates through a 1 volt potential difference in a vacuum using the 2019 SI units.\n\nThe electronvolt appear in The International System of Units (SI), 1th ed. (1970) defined as \"1 electronvolt is the energy acquired by an electron after traversing a potential difference of 1 V in a vacuum; 1 eV = 1.60219\u00d710\u207b\u00b9\u2079 J approximately.\"\nThis definition makes the unit equal to 1 volt times the value of the elementary charge.\nIn the 2019 redefinition of the SI units the elementary charge is exactly 1.602176634\u00b710\u207b\u00b9\u2079 C, making the electron volt exactly equal to 1.602176634\u00b710\u207b\u00b9\u2079 J.\nThe International System of Units (SI), 9th ed. (2019) accordingly notes the exact relationship with the SI 2019 derived unit joule as \"1 eV = 1.602176634\u00b710\u207b\u00b9\u2079 J\" but retains the definition from 1970 in a footnote.\n\nThe unit is categorized in The International System of Units (SI), 9th ed. (2019) as \"Non-SI units accepted for use with the SI units\".",
    "standard": {
        "name": "gnu units",
        "version": "3.15",
        "symbol": "angstrom"
    },
    "resources": [
        {
            "relation": "Definition in the International System of Units (SI), 9th Edition",
            "resource-id": "https://www.bipm.org/en/publications/si-brochure"
        },
        {
            "relation": "Wikipedia article describing the unit",
            "resource-id": "https://en.wikipedia.org/wiki/Electronvolt"
        }
    ],
    "defining-relation": {
        "base-units": [
            {
                "symbol": "V",
                "id": "https://schema.optimade.org/units/si/2019/named/volt"
            },
            {
                "symbol": "e",
                "id": "https://schema.optimade.org/constants/codata/2018/electromagnetic/elementarycharge"
            }
        ],
        "base-units-expression": "e*V"
    },
    "x-optimade-definition": {
        "kind": "unit",
        "format": "1.2",
        "version": "1.2.0",
        "name": "electronvolt"
    }
}
```
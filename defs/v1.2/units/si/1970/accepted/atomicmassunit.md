# atomic mass unit, u (unit)

This page documents an [OPTIMADE](https://www.optimade.org/) [Unit Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/defs/v1.2/units/si/1970/accepted/atomicmassunit`](https://schemas.optimade.org/defs/v1.2/units/si/1970/accepted/atomicmassunit.md)**  
**Definition name:** `atomicmassunit`

**Unit name:** atomic mass unit  
**Latin symbol:** u  
**Display symbol:** u  
  
**Description:** A unit of mass defined as 1/12 of the mass of a free carbon 12 atom, at rest and in its ground state.

The International System of Units (SI), 1st ed. (1970) defines the atomic mass unit in the section "Units used with the International System" (known as "Non-SI units accepted for use with the SI units" in later editions).
The unit is defined in a footnote as: "The atomic mass unit (unified) is equal to 1/12 of the mass of an atom of the nuclide ¹²C; 1 u = 1.66053 x 10⁻²⁷ kg approximately."

The definition is retained in the International System of Units up to the 7th edition (1998), where the conditions are slightly clarified and dalton (Da) is introduced as an alternative name: "The unified atomic mass unit is equal to 1/12 of the mass of an unbound atom of the nuclide ¹²C, at rest, and in its ground state. In the field of biochemistry, the unified atomic mass unit is also called the dalton, symbol Da."

In the 8th ed. (2006) the definition is slightly adjusted, replacing "unbound" with "free": "The dalton (Da) and the unified atomic mass unit (u) are alternative names (and symbols) for the same unit, equal to 1/12 times the mass of a free carbon 12 atom, at rest and in its ground state."

All editions of the International System of Units note approximate relationships to the kilogram.
The 9th ed. states "1 Da = 1.660 539 066 60(50)×10⁻²⁷ kg", where the 2018 CODATA value has been used and the 2019 SI kilogram is referenced (https://schemas.optimade.org/defs/v1.2/units/si/2019/base/kilogram).

In the 2019 redefinition of the SI units, the atomic mass unit is the only unit listed as accepted for use with SI that has an experimental relationship to the base SI units.

**Resources:**

- [Definition in the International System of Units (SI), 9th Edition](https://www.bipm.org/en/publications/si-brochure)
- [Wikipedia article describing the unit](https://en.wikipedia.org/wiki/Dalton_(unit))
- [CODATA unified atomic mass unit fundamental physical constant: source for relationship to kg](https://physics.nist.gov/cgi-bin/cuu/Value?ukg)


**Formats:** [[JSON](atomicmassunit.json)] [[MD](atomicmassunit.md)]

**JSON definition:**

``` json
{
    "$id": "https://schemas.optimade.org/defs/v1.2/units/si/1970/accepted/atomicmassunit",
    "$schema": "https://schemas.optimade.org/meta/v1.2/optimade/physical_unit_definition.json",
    "title": "atomic mass unit",
    "symbol": "u",
    "display-symbol": "u",
    "alternate-symbols": [
        "dalton",
        "Da"
    ],
    "description": "A unit of mass defined as 1/12 of the mass of a free carbon 12 atom, at rest and in its ground state.\n\nThe International System of Units (SI), 1st ed. (1970) defines the atomic mass unit in the section \"Units used with the International System\" (known as \"Non-SI units accepted for use with the SI units\" in later editions).\nThe unit is defined in a footnote as: \"The atomic mass unit (unified) is equal to 1/12 of the mass of an atom of the nuclide \u00b9\u00b2C; 1 u = 1.66053 x 10\u207b\u00b2\u2077 kg approximately.\"\n\nThe definition is retained in the International System of Units up to the 7th edition (1998), where the conditions are slightly clarified and dalton (Da) is introduced as an alternative name: \"The unified atomic mass unit is equal to 1/12 of the mass of an unbound atom of the nuclide \u00b9\u00b2C, at rest, and in its ground state. In the field of biochemistry, the unified atomic mass unit is also called the dalton, symbol Da.\"\n\nIn the 8th ed. (2006) the definition is slightly adjusted, replacing \"unbound\" with \"free\": \"The dalton (Da) and the unified atomic mass unit (u) are alternative names (and symbols) for the same unit, equal to 1/12 times the mass of a free carbon 12 atom, at rest and in its ground state.\"\n\nAll editions of the International System of Units note approximate relationships to the kilogram.\nThe 9th ed. states \"1 Da = 1.660 539 066 60(50)\u00d710\u207b\u00b2\u2077 kg\", where the 2018 CODATA value has been used and the 2019 SI kilogram is referenced (https://schemas.optimade.org/defs/v1.2/units/si/2019/base/kilogram).\n\nIn the 2019 redefinition of the SI units, the atomic mass unit is the only unit listed as accepted for use with SI that has an experimental relationship to the base SI units.",
    "resources": [
        {
            "relation": "Definition in the International System of Units (SI), 9th Edition",
            "resource-id": "https://www.bipm.org/en/publications/si-brochure"
        },
        {
            "relation": "Wikipedia article describing the unit",
            "resource-id": "https://en.wikipedia.org/wiki/Dalton_(unit)"
        },
        {
            "relation": "CODATA unified atomic mass unit fundamental physical constant: source for relationship to kg",
            "resource-id": "https://physics.nist.gov/cgi-bin/cuu/Value?ukg"
        }
    ],
    "approximate-relations": [
        {
            "base-units": [
                {
                    "symbol": "kg",
                    "id": "https://schemas.optimade.org/defs/v1.2/units/si/2019/base/kilogram"
                }
            ],
            "base-units-expression": "kg",
            "scale": {
                "value": 1.6605390666e-27,
                "standard_uncertainty": 5e-37
            }
        }
    ],
    "x-optimade-definition": {
        "label": "atomicmassunit_si_1970_accepted",
        "kind": "unit",
        "format": "1.2",
        "version": "1.2.0",
        "name": "atomicmassunit"
    }
}
```
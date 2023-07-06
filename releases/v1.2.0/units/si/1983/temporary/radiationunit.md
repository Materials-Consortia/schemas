# radiation unit, rad (unit)

This page documents an [OPTIMADE](https://www.optimade.org/) [Unit Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/defs/v1.2/units/si/1983/temporary/radiationunit`](https://schemas.optimade.org/defs/v1.2/units/si/1983/temporary/radiationunit)**  
**Definition name:** `radiationunit`

**Unit name:** radiation unit  
**Latin symbol:** radiationunit  
**Display symbol:** rad  
  
**Description:** A unit used to express the absorbed dose of ionizing radiation defined as 10⁻² J/kg using the 1983 SI units.

This unit definition uses "radiationunit" as the symbol for this unit despite "rad" being in common use to distiguish it from the radian, which is an SI unit with rad as its symbol.

The radiation unit appear in the International System of Units (SI), 1th ed. (1970) defined as "1 rad = 10⁻² J/kg" with the footnote: "The rad is a special unit employed to express absorbed dose of ionizing radiation. When there is risk of confusion with the symbol for radian, rd may be used as the symbol for rad."

The International System of Units (SI), 1th ed. (1970) categorizes the unit as "Units in use temporarily with the International System."
The International System of Units (SI), 3rd ed. (1977) changes the definition to use the unit gray: "1 rad = cGy = 10⁻² Gy."
The International System of Units (SI), 7th ed. (1998) changes the categorization to "Examples of other non-SI units" and adds the additional footnote: "Note that this non-SI unit is exactly equivalent to an SI unit with an appropriate submultiple prefix."
The International System of Units (SI), 8th ed. (2006) omits the unit.

The roentgen was implicitly redefined via the redefinition of the metre at the 17th CGPM meeting (1983), resolution 1.

**Resources:**

- [Definition in the International System of Units (SI), 1st Edition](https://www.bipm.org/en/publications/si-brochure)
- [Redefinition of the metre at the 17th CGPM meeting (1983), resolution 1](https://www.bipm.org/en/committees/cg/cgpm/17-1983/resolution-1)
- [Wikipedia article describing the unit](https://en.wikipedia.org/wiki/Rad_(radiation_unit))


**Formats:** [[JSON](radiationunit.json)] [[MD](radiationunit.md)]

**JSON definition:**

``` json
{
    "$schema": "https://schemas.optimade.org/meta/v1.2/optimade/physical_unit_definition.md",
    "$id": "https://schemas.optimade.org/defs/v1.2/units/si/1983/temporary/radiationunit",
    "title": "radiation unit",
    "symbol": "radiationunit",
    "display-symbol": "rad",
    "description": "A unit used to express the absorbed dose of ionizing radiation defined as 10\u207b\u00b2 J/kg using the 1983 SI units.\n\nThis unit definition uses \"radiationunit\" as the symbol for this unit despite \"rad\" being in common use to distiguish it from the radian, which is an SI unit with rad as its symbol.\n\nThe radiation unit appear in the International System of Units (SI), 1th ed. (1970) defined as \"1 rad = 10\u207b\u00b2 J/kg\" with the footnote: \"The rad is a special unit employed to express absorbed dose of ionizing radiation. When there is risk of confusion with the symbol for radian, rd may be used as the symbol for rad.\"\n\nThe International System of Units (SI), 1th ed. (1970) categorizes the unit as \"Units in use temporarily with the International System.\"\nThe International System of Units (SI), 3rd ed. (1977) changes the definition to use the unit gray: \"1 rad = cGy = 10\u207b\u00b2 Gy.\"\nThe International System of Units (SI), 7th ed. (1998) changes the categorization to \"Examples of other non-SI units\" and adds the additional footnote: \"Note that this non-SI unit is exactly equivalent to an SI unit with an appropriate submultiple prefix.\"\nThe International System of Units (SI), 8th ed. (2006) omits the unit.\n\nThe roentgen was implicitly redefined via the redefinition of the metre at the 17th CGPM meeting (1983), resolution 1.",
    "standard": {
        "name": "gnu units",
        "version": "3.15",
        "symbol": "rad"
    },
    "resources": [
        {
            "relation": "Definition in the International System of Units (SI), 1st Edition",
            "resource-id": "https://www.bipm.org/en/publications/si-brochure"
        },
        {
            "relation": "Redefinition of the metre at the 17th CGPM meeting (1983), resolution 1",
            "resource-id": "https://www.bipm.org/en/committees/cg/cgpm/17-1983/resolution-1"
        },
        {
            "relation": "Wikipedia article describing the unit",
            "resource-id": "https://en.wikipedia.org/wiki/Rad_(radiation_unit)"
        }
    ],
    "defining-relation": {
        "base-units": [
            {
                "symbol": "J",
                "id": "https://schema.optimade.org/units/si/1983/named/joule"
            },
            {
                "symbol": "kg",
                "id": "https://schema.optimade.org/units/si/1960/base/kilogram"
            }
        ],
        "base-units-expression": "J*kg^-1",
        "scale": {
            "exponent": -2
        }
    },
    "x-optimade-definition": {
        "kind": "unit",
        "format": "1.2",
        "version": "1.2.0",
        "name": "radiationunit"
    }
}
```
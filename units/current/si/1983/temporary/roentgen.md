# roentgen, R (unit)
This page documents an [OPTIMADE](https://www.optimade.org/) [Unit Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/units/v1.2.0/si/1983/temporary/roentgen`](https://schemas.optimade.org/units/v1.2.0/si/1983/temporary/roentgen)**  
**Definition name:** `roentgen`

**Unit name:** roentgen  
**Latin symbol:** R  
**Display symbol:** R  
  
**Description:** A unit used to express the exposure of ionizing radiation defined as 2.58 x 10⁻⁴ C/kg using the 1983 SI units.

The roentgen appear in the International System of Units (SI), 1th ed. (1970) defined as "1 R = 2.58 x 10⁻⁴ C/kg" with the footnote: "The roentgen is a special unit used to express the ionization exposure of ionizing radiation."

The International System of Units (SI), 1th ed. (1970) categorizes the unit as "Units in use temporarily with the International Sytem."
The International System of Units (SI), 2nd ed. (1973) rephrases the footnote to: "The roentgen is a special unit used to express the exposure of X or gamma radiation."
The International System of Units (SI), 7th ed. (1998) changes the categorization to "Examples of other non-SI units".
The International System of Units (SI), 8th ed. (2006) omits the unit.

The roentgen was implicitly redefined via the redefinition of the metre at the 17th CGPM meeting (1983), resolution 1.

**Resources:**

- [Definition in the International System of Units (SI), 1st Edition](https://www.bipm.org/en/publications/si-brochure)
- [Redefinition of the metre at the 17th CGPM meeting (1983), resolution 1](https://www.bipm.org/en/committees/cg/cgpm/17-1983/resolution-1)
- [Wikipedia article describing the unit](https://en.wikipedia.org/wiki/Roentgen_(unit))


**Formats:** [[JSON](roentgen.json)] [[MD](roentgen.md)]

**JSON definition:**

``` json
{
    "$id": "https://schemas.optimade.org/units/v1.2.0/si/1983/temporary/roentgen",
    "title": "roentgen",
    "symbol": "R",
    "display-symbol": "R",
    "description": "A unit used to express the exposure of ionizing radiation defined as 2.58 x 10\u207b\u2074 C/kg using the 1983 SI units.\n\nThe roentgen appear in the International System of Units (SI), 1th ed. (1970) defined as \"1 R = 2.58 x 10\u207b\u2074 C/kg\" with the footnote: \"The roentgen is a special unit used to express the ionization exposure of ionizing radiation.\"\n\nThe International System of Units (SI), 1th ed. (1970) categorizes the unit as \"Units in use temporarily with the International Sytem.\"\nThe International System of Units (SI), 2nd ed. (1973) rephrases the footnote to: \"The roentgen is a special unit used to express the exposure of X or gamma radiation.\"\nThe International System of Units (SI), 7th ed. (1998) changes the categorization to \"Examples of other non-SI units\".\nThe International System of Units (SI), 8th ed. (2006) omits the unit.\n\nThe roentgen was implicitly redefined via the redefinition of the metre at the 17th CGPM meeting (1983), resolution 1.",
    "standard": {
        "name": "gnu units",
        "version": "3.15",
        "symbol": "roentgen"
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
            "resource-id": "https://en.wikipedia.org/wiki/Roentgen_(unit)"
        }
    ],
    "defining-relation": {
        "base-units": [
            {
                "symbol": "C",
                "id": "https://schema.optimade.org/units/v1.2.0/si/1983/named/coulomb"
            },
            {
                "symbol": "kg",
                "id": "https://schema.optimade.org/units/v1.2.0/si/1976/named/kilogram"
            }
        ],
        "base-units-expression": "C*kg^-1",
        "scale": {
            "exponent": -4
        }
    },
    "x-optimade-definition": {
        "kind": "unit",
        "format": "1.2",
        "version": "1.2.0",
        "name": "roentgen"
    },
    "$schema": "https://schemas.optimade.org/meta/v1.2.0/optimade/physical_unit_definition.md"
}
```
# roentgen, R (unit)

This page documents an [OPTIMADE](https://www.optimade.org/) [Unit Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/defs/v1.2/units/si/1970/temporary/roentgen`](https://schemas.optimade.org/defs/v1.2/units/si/1970/temporary/roentgen.md)**  
**Definition name:** `roentgen`

**Unit name:** roentgen  
**Latin symbol:** R  
**Display symbol:** R  
  
**Description:** A unit used to express the exposure of ionizing radiation defined as 2.58 x 10⁻⁴ C/kg using the 1967 SI units.

The roentgen appear in the International System of Units (SI), 1th ed. (1970) defined as "1 R = 2.58 x 10⁻⁴ C/kg" with the footnote: "The roentgen is a special unit used to express the ionization exposure of ionizing radiation."

- The International System of Units (SI), 1th ed. (1970) categorizes the unit as "Units in use temporarily with the International System."
- The International System of Units (SI), 2nd ed. (1973) rephrases the footnote to: "The roentgen is a special unit used to express the exposure of X or gamma radiation."
- The International System of Units (SI), 7th ed. (1998) changes the categorization to "Examples of other non-SI units".
- The International System of Units (SI), 8th ed. (2006) omits the unit.

**Resources:**

- [Definition in the International System of Units (SI), 1st Edition](https://www.bipm.org/en/publications/si-brochure)
- [Wikipedia article describing the unit](https://en.wikipedia.org/wiki/Roentgen_(unit))


**Formats:** [[JSON](roentgen.json)] [[MD](roentgen.md)]

**JSON definition:**

``` json
{
    "$schema": "https://schemas.optimade.org/meta/v1.2/optimade/physical_unit_definition.md",
    "$id": "https://schemas.optimade.org/defs/v1.2/units/si/1970/temporary/roentgen",
    "title": "roentgen",
    "symbol": "R",
    "display-symbol": "R",
    "description": "A unit used to express the exposure of ionizing radiation defined as 2.58 x 10\u207b\u2074 C/kg using the 1967 SI units.\n\nThe roentgen appear in the International System of Units (SI), 1th ed. (1970) defined as \"1 R = 2.58 x 10\u207b\u2074 C/kg\" with the footnote: \"The roentgen is a special unit used to express the ionization exposure of ionizing radiation.\"\n\n- The International System of Units (SI), 1th ed. (1970) categorizes the unit as \"Units in use temporarily with the International System.\"\n- The International System of Units (SI), 2nd ed. (1973) rephrases the footnote to: \"The roentgen is a special unit used to express the exposure of X or gamma radiation.\"\n- The International System of Units (SI), 7th ed. (1998) changes the categorization to \"Examples of other non-SI units\".\n- The International System of Units (SI), 8th ed. (2006) omits the unit.",
    "resources": [
        {
            "relation": "Definition in the International System of Units (SI), 1st Edition",
            "resource-id": "https://www.bipm.org/en/publications/si-brochure"
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
                "id": "https://schema.optimade.org/units/si/1976/named/coulomb"
            },
            {
                "symbol": "kg",
                "id": "https://schema.optimade.org/units/si/1976/named/kilogram"
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
    }
}
```
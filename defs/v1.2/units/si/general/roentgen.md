# roentgen, R (unit)

This page documents an [OPTIMADE](https://www.optimade.org/) [Unit Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/defs/v1.2/units/si/general/roentgen`](https://schemas.optimade.org/defs/v1.2/units/si/general/roentgen.md)**  
**Definition name:** `roentgen`

**Unit name:** roentgen  
**Latin symbol:** R  
**Display symbol:** R  
  
**Description:** A unit used to express the exposure of ionizing radiation defined as 2.58 x 10⁻⁴ C/kg using the current, or one of the historical, definitions of the SI units.

The roentgen unit appears in the International System of Units (SI), 1st ed. (1970) defined as "1 R = 2.58 x 10⁻⁴ C/kg" with the footnote: "The roentgen is a special unit used to express the ionization exposure of ionizing radiation."

- The International System of Units (SI), 1st ed. (1970) categorizes the unit as "Units in use temporarily with the International System."
- The International System of Units (SI), 2nd ed. (1973) rephrases the footnote to: "The roentgen is a special unit used to express the exposure of X or gamma radiation."
- The International System of Units (SI), 7th ed. (1998) changes the categorization to "Examples of other non-SI units".
- The International System of Units (SI), 8th ed. (2006) omits the unit.

The roentgen unit was implicitly redefined via the redefinition of the metre at the 17th CGPM meeting (1983), resolution 1.

This is a generalized definition taken to reference the current, or one of the historical, SI unit definitions.
This definition is intended for situations when it is not possible to be more precise, e.g., in contexts where data have been collected that uses different historical SI definitions.

**Resources:**

- [Definition in the International System of Units (SI), 1st Edition](https://www.bipm.org/en/publications/si-brochure)
- [Redefinition of the metre at the 17th CGPM meeting (1983), resolution 1](https://www.bipm.org/en/committees/cg/cgpm/17-1983/resolution-1)
- [Wikipedia article describing the unit](https://en.wikipedia.org/wiki/Roentgen_(unit))


**Compatibility:** (other definitions that are covered by the above definition)

- [`https://schemas.optimade.org/defs/v1.2/units/si/1970/temporary/roentgen`](https://schemas.optimade.org/defs/v1.2/units/si/1970/temporary/roentgen.md)
- [`https://schemas.optimade.org/defs/v1.2/units/si/1983/temporary/roentgen`](https://schemas.optimade.org/defs/v1.2/units/si/1983/temporary/roentgen.md)


**Formats:** [[JSON](roentgen.json)] [[MD](roentgen.md)]

**JSON definition:**

``` json
{
    "$id": "https://schemas.optimade.org/defs/v1.2/units/si/general/roentgen",
    "$schema": "https://schemas.optimade.org/meta/v1.2/optimade/physical_unit_definition.json",
    "title": "roentgen",
    "symbol": "R",
    "display-symbol": "R",
    "description": "A unit used to express the exposure of ionizing radiation defined as 2.58 x 10\u207b\u2074 C/kg using the current, or one of the historical, definitions of the SI units.\n\nThe roentgen unit appears in the International System of Units (SI), 1st ed. (1970) defined as \"1 R = 2.58 x 10\u207b\u2074 C/kg\" with the footnote: \"The roentgen is a special unit used to express the ionization exposure of ionizing radiation.\"\n\n- The International System of Units (SI), 1st ed. (1970) categorizes the unit as \"Units in use temporarily with the International System.\"\n- The International System of Units (SI), 2nd ed. (1973) rephrases the footnote to: \"The roentgen is a special unit used to express the exposure of X or gamma radiation.\"\n- The International System of Units (SI), 7th ed. (1998) changes the categorization to \"Examples of other non-SI units\".\n- The International System of Units (SI), 8th ed. (2006) omits the unit.\n\nThe roentgen unit was implicitly redefined via the redefinition of the metre at the 17th CGPM meeting (1983), resolution 1.\n\nThis is a generalized definition taken to reference the current, or one of the historical, SI unit definitions.\nThis definition is intended for situations when it is not possible to be more precise, e.g., in contexts where data have been collected that uses different historical SI definitions.",
    "compatibility": [
        "https://schemas.optimade.org/defs/v1.2/units/si/1970/temporary/roentgen",
        "https://schemas.optimade.org/defs/v1.2/units/si/1983/temporary/roentgen"
    ],
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
                "id": "https://schemas.optimade.org/defs/v1.2/units/si/general/coulomb"
            },
            {
                "symbol": "kg",
                "id": "https://schemas.optimade.org/defs/v1.2/units/si/general/kilogram"
            }
        ],
        "base-units-expression": "C*kg^-1",
        "scale": {
            "numerator": 258,
            "exponent": -6
        }
    },
    "x-optimade-definition": {
        "label": "roentgen_si_general",
        "kind": "unit",
        "format": "1.2",
        "version": "1.2.0",
        "name": "roentgen"
    }
}
```
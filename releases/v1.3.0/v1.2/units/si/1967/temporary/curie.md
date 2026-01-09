# curie, Ci (unit)

This page documents an [OPTIMADE](https://www.optimade.org/) [Unit Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/defs/v1.2/units/si/1967/temporary/curie`](https://schemas.optimade.org/defs/v1.2/units/si/1967/temporary/curie.md)**  
**Definition name:** `curie`

**Unit name:** curie  
**Latin symbol:** Ci  
**Display symbol:** Ci  
  
**Description:** A non-SI unit of activity with the value 3.7·10⁻¹⁰ s⁻¹ in the 1967 SI units.

Defined as outside the SI at the 12th CGPM meeting in 1964, resolution 7.
Implicitly redefined via the redefinition of the second at the 13th CGPM Meeting in 1967, resolution 1.

- The International System of Units (SI), 1st ed. (1970) categorizes the unit as "Units in use temporarily with the International System."
- The International System of Units (SI), 7th ed. (1998) changes the categorization to "Other non-SI units".
- The curie is omitted in the International System of Units (SI), 8th Edition (2006).

**Resources:**

- [Definition at the 12th CGPM meeting (1964), resolution 3](https://www.bipm.org/en/committees/cg/cgpm/12-1964/resolution-3)
- [Redefinition of the second in the 13th CGPM Meeting (1967), resolution 1](https://www.bipm.org/en/committees/cg/cgpm/13-1967/resolution-1)
- [Le Système International d'Unités (SI) (1970)](https://www.bipm.org/en/publications/si-brochure)
- [Wikipedia article describing the unit](https://en.wikipedia.org/wiki/Curie_(unit))


**Formats:** [[JSON](curie.json)] [[MD](curie.md)]

**JSON definition:**

``` json
{
    "$id": "https://schemas.optimade.org/defs/v1.2/units/si/1967/temporary/curie",
    "$schema": "https://schemas.optimade.org/meta/v1.2/optimade/physical_unit_definition.json",
    "title": "curie",
    "symbol": "Ci",
    "display-symbol": "Ci",
    "description": "A non-SI unit of activity with the value 3.7\u00b710\u207b\u00b9\u2070 s\u207b\u00b9 in the 1967 SI units.\n\nDefined as outside the SI at the 12th CGPM meeting in 1964, resolution 7.\nImplicitly redefined via the redefinition of the second at the 13th CGPM Meeting in 1967, resolution 1.\n\n- The International System of Units (SI), 1st ed. (1970) categorizes the unit as \"Units in use temporarily with the International System.\"\n- The International System of Units (SI), 7th ed. (1998) changes the categorization to \"Other non-SI units\".\n- The curie is omitted in the International System of Units (SI), 8th Edition (2006).",
    "resources": [
        {
            "relation": "Definition at the 12th CGPM meeting (1964), resolution 3",
            "resource-id": "https://www.bipm.org/en/committees/cg/cgpm/12-1964/resolution-3"
        },
        {
            "relation": "Redefinition of the second in the 13th CGPM Meeting (1967), resolution 1",
            "resource-id": "https://www.bipm.org/en/committees/cg/cgpm/13-1967/resolution-1"
        },
        {
            "relation": "Le Syst\u00e8me International d'Unit\u00e9s (SI) (1970)",
            "resource-id": "https://www.bipm.org/en/publications/si-brochure"
        },
        {
            "relation": "Wikipedia article describing the unit",
            "resource-id": "https://en.wikipedia.org/wiki/Curie_(unit)"
        }
    ],
    "defining-relation": {
        "base-units": [
            {
                "symbol": "s",
                "id": "https://schemas.optimade.org/defs/v1.2/units/si/1967/base/second"
            }
        ],
        "base-units-expression": "s^-1",
        "scale": {
            "numerator": 37,
            "exponent": -11
        }
    },
    "x-optimade-definition": {
        "label": "curie_si_1967_temporary",
        "kind": "unit",
        "format": "1.2",
        "version": "1.2.0",
        "name": "curie"
    }
}
```
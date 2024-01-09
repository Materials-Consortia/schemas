# barn, b (unit)

This page documents an [OPTIMADE](https://www.optimade.org/) [Unit Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/defs/v1.2/units/si/1970/temporary/barn`](https://schemas.optimade.org/defs/v1.2/units/si/1970/temporary/barn.md)**  
**Definition name:** `barn`

**Unit name:** barn  
**Latin symbol:** b  
**Display symbol:** b  
  
**Description:** A unit of area used in nuclear physics to express cross sections equal to 100 fm², with meter defined according to the 1960 SI units.

The International System of Units (SI), 1st ed. (1970) states: "1 b = 100 fm² = 10⁻²⁸ m" with a footnote "The barn is a special unit used in nuclear physics to express cross sections."

- The International System of Units (SI), 1st ed. (1970) categorizes the unit as "Units in use temporarily with the International System."
- The International System of Units (SI), 8th ed. (2006) categorizes the unit as "Other non-SI units currently accepted for use with the International System."
- The International System of Units (SI), 9th ed. (2019) categorizes the unit as "Other non-SI units."

**Resources:**

- [Definition in the International System of Units (SI), 9th Edition](https://www.bipm.org/en/publications/si-brochure)
- [Wikipedia article describing the unit](https://en.wikipedia.org/wiki/Barn_(unit))


**Formats:** [[JSON](barn.json)] [[MD](barn.md)]

**JSON definition:**

``` json
{
    "$schema": "https://schemas.optimade.org/meta/v1.2/optimade/physical_unit_definition.md",
    "$id": "https://schemas.optimade.org/defs/v1.2/units/si/1970/temporary/barn",
    "title": "barn",
    "symbol": "b",
    "display-symbol": "b",
    "description": "A unit of area used in nuclear physics to express cross sections equal to 100 fm\u00b2, with meter defined according to the 1960 SI units.\n\nThe International System of Units (SI), 1st ed. (1970) states: \"1 b = 100 fm\u00b2 = 10\u207b\u00b2\u2078 m\" with a footnote \"The barn is a special unit used in nuclear physics to express cross sections.\"\n\n- The International System of Units (SI), 1st ed. (1970) categorizes the unit as \"Units in use temporarily with the International System.\"\n- The International System of Units (SI), 8th ed. (2006) categorizes the unit as \"Other non-SI units currently accepted for use with the International System.\"\n- The International System of Units (SI), 9th ed. (2019) categorizes the unit as \"Other non-SI units.\"",
    "resources": [
        {
            "relation": "Definition in the International System of Units (SI), 9th Edition",
            "resource-id": "https://www.bipm.org/en/publications/si-brochure"
        },
        {
            "relation": "Wikipedia article describing the unit",
            "resource-id": "https://en.wikipedia.org/wiki/Barn_(unit)"
        }
    ],
    "defining-relation": {
        "base-units": [
            {
                "symbol": "m",
                "id": "https://schemas.optimade.org/defs/v1.2/units/si/1960/base/metre"
            }
        ],
        "scale": {
            "exponent": 4
        },
        "base-units-expression": "m^2"
    },
    "x-optimade-definition": {
        "label": "barn_si_1970_temporary",
        "kind": "unit",
        "format": "1.2",
        "version": "1.2.0",
        "name": "barn"
    }
}
```
# hectare, he (unit)

This page documents an [OPTIMADE](https://www.optimade.org/) [Unit Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/defs/v1.2/units/si/1970/temporary/hectare`](https://schemas.optimade.org/defs/v1.2/units/si/1970/temporary/hectare.md)**  
**Definition name:** `hectare`

**Unit name:** hectare  
**Latin symbol:** he  
**Display symbol:** he  
  
**Description:** A unit of area equal to 1000 square meters (1 hm²), with meter defined according to the 1960 SI base unit.

The hectare appear in the International System of Units (SI), 1th ed. (1970) defined as "1 ha = 1 hm² = 10⁴ m²" with the footnote "This unit and its symbol were adopted by the International Committee in 1879 (Proces-Verbaux C.I.P.M., 1879, p. 41).

- The International System of Units (SI), 1th ed. (1970) categorizes the unit as "units in use temporarily".
- The International System of Units (SI), 5th ed. (1985) add the clarification that the unit is "used to express agricultural areas."
- The International System of Units (SI), 7th ed. (1998) changes the categorisation to "Other non-SI units currently accepted for use with the International System."

**Resources:**

- [Definition in the International System of Units (SI), 9th Edition](https://www.bipm.org/en/publications/si-brochure)
- [Wikipedia article describing the unit](https://en.wikipedia.org/wiki/Hectare)


**Formats:** [[JSON](hectare.json)] [[MD](hectare.md)]

**JSON definition:**

``` json
{
    "$schema": "https://schemas.optimade.org/meta/v1.2/optimade/physical_unit_definition.md",
    "$id": "https://schemas.optimade.org/defs/v1.2/units/si/1970/temporary/hectare",
    "title": "hectare",
    "symbol": "he",
    "display-symbol": "he",
    "description": "A unit of area equal to 1000 square meters (1 hm\u00b2), with meter defined according to the 1960 SI base unit.\n\nThe hectare appear in the International System of Units (SI), 1th ed. (1970) defined as \"1 ha = 1 hm\u00b2 = 10\u2074 m\u00b2\" with the footnote \"This unit and its symbol were adopted by the International Committee in 1879 (Proces-Verbaux C.I.P.M., 1879, p. 41).\n\n- The International System of Units (SI), 1th ed. (1970) categorizes the unit as \"units in use temporarily\".\n- The International System of Units (SI), 5th ed. (1985) add the clarification that the unit is \"used to express agricultural areas.\"\n- The International System of Units (SI), 7th ed. (1998) changes the categorisation to \"Other non-SI units currently accepted for use with the International System.\"",
    "resources": [
        {
            "relation": "Definition in the International System of Units (SI), 9th Edition",
            "resource-id": "https://www.bipm.org/en/publications/si-brochure"
        },
        {
            "relation": "Wikipedia article describing the unit",
            "resource-id": "https://en.wikipedia.org/wiki/Hectare"
        }
    ],
    "defining-relation": {
        "base-units": [
            {
                "symbol": "m",
                "id": "https://schema.optimade.org/units/si/2019/base/metre"
            }
        ],
        "base-units-expression": "m^2",
        "scale": {
            "exponent": 4
        }
    },
    "x-optimade-definition": {
        "kind": "unit",
        "format": "1.2",
        "version": "1.2.0",
        "name": "hectare"
    }
}
```
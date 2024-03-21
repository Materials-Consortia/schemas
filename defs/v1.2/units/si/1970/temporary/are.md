# are, a (unit)

This page documents an [OPTIMADE](https://www.optimade.org/) [Unit Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/defs/v1.2/units/si/1970/temporary/are`](https://schemas.optimade.org/defs/v1.2/units/si/1970/temporary/are.md)**  
**Definition name:** `are`

**Unit name:** are  
**Latin symbol:** a  
**Display symbol:** a  
  
**Description:** A unit of area equal to 100 square meters (10² m²), with meter defined according to the 1960 SI base units.

The are unit appears in the International System of Units (SI), 1st ed. (1970) defined as "1 a = 1 dam² = 10² m²" with the footnote "This unit and its symbol were adopted by the International Committee in 1879 (Proces-Verbaux C.I.P.M., 1879, p. 41)."

- The International System of Units (SI), 1st ed. (1970) categorizes the unit as "units in use temporarily".
- The International System of Units (SI), 5th ed. (1985) adds the clarification that the unit is "used to express agrarian areas."
- The International System of Units (SI), 7th ed. (1998) changes the categorization to "Other non-SI units currently accepted for use with the International System."
- The International System of Units (SI), 8th ed. (2006) completely removes the unit (but still defines the hectare).

**Resources:**

- [Definition in the International System of Units (SI), 1st Edition](https://www.bipm.org/en/publications/si-brochure)
- [Wikipedia article describing the unit](https://en.wikipedia.org/wiki/Hectare#Are)


**Formats:** [[JSON](are.json)] [[MD](are.md)]

**JSON definition:**

``` json
{
    "$id": "https://schemas.optimade.org/defs/v1.2/units/si/1970/temporary/are",
    "$schema": "https://schemas.optimade.org/meta/v1.2/optimade/physical_unit_definition.json",
    "title": "are",
    "symbol": "a",
    "display-symbol": "a",
    "description": "A unit of area equal to 100 square meters (10\u00b2 m\u00b2), with meter defined according to the 1960 SI base units.\n\nThe are unit appears in the International System of Units (SI), 1st ed. (1970) defined as \"1 a = 1 dam\u00b2 = 10\u00b2 m\u00b2\" with the footnote \"This unit and its symbol were adopted by the International Committee in 1879 (Proces-Verbaux C.I.P.M., 1879, p. 41).\"\n\n- The International System of Units (SI), 1st ed. (1970) categorizes the unit as \"units in use temporarily\".\n- The International System of Units (SI), 5th ed. (1985) adds the clarification that the unit is \"used to express agrarian areas.\"\n- The International System of Units (SI), 7th ed. (1998) changes the categorization to \"Other non-SI units currently accepted for use with the International System.\"\n- The International System of Units (SI), 8th ed. (2006) completely removes the unit (but still defines the hectare).",
    "resources": [
        {
            "relation": "Definition in the International System of Units (SI), 1st Edition",
            "resource-id": "https://www.bipm.org/en/publications/si-brochure"
        },
        {
            "relation": "Wikipedia article describing the unit",
            "resource-id": "https://en.wikipedia.org/wiki/Hectare#Are"
        }
    ],
    "defining-relation": {
        "base-units": [
            {
                "symbol": "m",
                "id": "https://schemas.optimade.org/defs/v1.2/units/si/1960/base/metre"
            }
        ],
        "base-units-expression": "m^2",
        "scale": {
            "exponent": 4
        }
    },
    "x-optimade-definition": {
        "label": "are_si_1970_temporary",
        "kind": "unit",
        "format": "1.2",
        "version": "1.2.0",
        "name": "are"
    }
}
```
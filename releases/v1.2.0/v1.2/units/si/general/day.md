# day, day (unit)

This page documents an [OPTIMADE](https://www.optimade.org/) [Unit Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/defs/v1.2/units/si/general/day`](https://schemas.optimade.org/defs/v1.2/units/si/general/day.md)**  
**Definition name:** `day`

**Unit name:** day  
**Latin symbol:** day  
**Display symbol:** day  
  
**Description:** A unit of time equal to 86 400 seconds using the current, or one of the historical, definitions of the SI units.

The day appear in the International System of Units (SI), 1th ed. (1970) defined as "1 d = 24 h = 86400 s".

- The International System of Units (SI), 1th ed. (1970) categorizes the unit as "Units in use with the International System."
- The International System of Units (SI), 7th ed. (1998) changes the categorization to "Non-SI units accepted for use with the International System."

This is a generalized definition taken to reference the current, or one of the historical, SI unit definitions.
This definition is intended for situations when it is not possible to be more precise, e.g., in contexts where data have been collected that uses different historical SI definitions.

**Resources:**

- [Definition in the International System of Units (SI), 1st Edition](https://www.bipm.org/en/publications/si-brochure)
- [Wikipedia article describing the unit](https://en.wikipedia.org/wiki/Day)


**Formats:** [[JSON](day.json)] [[MD](day.md)]

**JSON definition:**

``` json
{
    "$schema": "https://schemas.optimade.org/meta/v1.2/optimade/physical_unit_definition.md",
    "$id": "https://schemas.optimade.org/defs/v1.2/units/si/general/day",
    "title": "day",
    "symbol": "day",
    "display-symbol": "day",
    "alternate-symbols": [
        "d"
    ],
    "description": "A unit of time equal to 86 400 seconds using the current, or one of the historical, definitions of the SI units.\n\nThe day appear in the International System of Units (SI), 1th ed. (1970) defined as \"1 d = 24 h = 86400 s\".\n\n- The International System of Units (SI), 1th ed. (1970) categorizes the unit as \"Units in use with the International System.\"\n- The International System of Units (SI), 7th ed. (1998) changes the categorization to \"Non-SI units accepted for use with the International System.\"\n\nThis is a generalized definition taken to reference the current, or one of the historical, SI unit definitions.\nThis definition is intended for situations when it is not possible to be more precise, e.g., in contexts where data have been collected that uses different historical SI definitions.",
    "compatibility": [
        "https://schemas.optimade.org/units/v1.2/si/1970/accepted/day"
    ],
    "resources": [
        {
            "relation": "Definition in the International System of Units (SI), 1st Edition",
            "resource-id": "https://www.bipm.org/en/publications/si-brochure"
        },
        {
            "relation": "Wikipedia article describing the unit",
            "resource-id": "https://en.wikipedia.org/wiki/Day"
        }
    ],
    "defining-relation": {
        "base-units": [
            {
                "symbol": "s",
                "id": "https://schema.optimade.org/units/si/general/second"
            }
        ],
        "base-units-expression": "s",
        "scale": {
            "numerator": 86400
        }
    },
    "x-optimade-definition": {
        "kind": "unit",
        "format": "1.2",
        "version": "1.2.0",
        "name": "day"
    }
}
```
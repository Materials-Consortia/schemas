# minute, min (unit)

This page documents an [OPTIMADE](https://www.optimade.org/) [Unit Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/defs/v1.2/units/si/1970/accepted/minute`](https://schemas.optimade.org/defs/v1.2/units/si/1970/accepted/minute.md)**  
**Definition name:** `minute`

**Unit name:** minute  
**Latin symbol:** min  
**Display symbol:** min  
  
**Description:** A unit of time that is equal to 60 seconds, using the 1967 base SI units.

The minute appear in the International System of Units (SI), 1th ed. (1970) defined as "1 min = 60 s".

- The International System of Units (SI), 1th ed. (1970) categorizes the unit as "Units in use with the International System."
- The International System of Units (SI), 7th ed. (1998) changes the categorization to "Non-SI units accepted for use with the International System."

**Resources:**

- [Definition in the International System of Units (SI), 1st Edition](https://www.bipm.org/en/publications/si-brochure)
- [Wikipedia article describing the unit](https://en.wikipedia.org/wiki/Minute)


**Formats:** [[JSON](minute.json)] [[MD](minute.md)]

**JSON definition:**

``` json
{
    "$schema": "https://schemas.optimade.org/meta/v1.2/optimade/physical_unit_definition.md",
    "$id": "https://schemas.optimade.org/defs/v1.2/units/si/1970/accepted/minute",
    "title": "minute",
    "symbol": "min",
    "display-symbol": "min",
    "description": "A unit of time that is equal to 60 seconds, using the 1967 base SI units.\n\nThe minute appear in the International System of Units (SI), 1th ed. (1970) defined as \"1 min = 60 s\".\n\n- The International System of Units (SI), 1th ed. (1970) categorizes the unit as \"Units in use with the International System.\"\n- The International System of Units (SI), 7th ed. (1998) changes the categorization to \"Non-SI units accepted for use with the International System.\"",
    "resources": [
        {
            "relation": "Definition in the International System of Units (SI), 1st Edition",
            "resource-id": "https://www.bipm.org/en/publications/si-brochure"
        },
        {
            "relation": "Wikipedia article describing the unit",
            "resource-id": "https://en.wikipedia.org/wiki/Minute"
        }
    ],
    "defining-relation": {
        "base-units": [
            {
                "symbol": "s",
                "id": "https://schemas.optimade.org/defs/v1.2/units/si/1960/base/second"
            }
        ],
        "base-units-expression": "s",
        "scale": {
            "numerator": 60
        }
    },
    "x-optimade-definition": {
        "label": "minute_si_1970_accepted",
        "kind": "unit",
        "format": "1.2",
        "version": "1.2.0",
        "name": "minute"
    }
}
```
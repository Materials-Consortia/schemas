# astronomical unit, au (unit)

This page documents an [OPTIMADE](https://www.optimade.org/) [Unit Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/defs/v1.2/units/si/2019/accepted/astronomicalunit`](https://schemas.optimade.org/defs/v1.2/units/si/2019/accepted/astronomicalunit.md)**  
**Definition name:** `astronomicalunit`

**Unit name:** astronomical unit  
**Latin symbol:** astronomicalunit  
**Display symbol:** au  
  
**Description:** A unit defined as exactly 149597870700 meters which is meant to represent the mean distance between the Earth and the Sun using the SI 1983 meter.

The International System of Units (SI), 9th ed. (2019) changed the definition of the astronomical unit given in prior editions into: "1 au = 149 597 870 700 m" with the footnote "As decided at the XXVIII General Assembly of the International Astronomical Union (Resolution B2, 2012)."

The International System of Units (SI), 9th ed. (2019) categorizes the astronomical unit as a "non-SI unit accepted for use with the SI units".

**Resources:**

- [Definition in the International System of Units (SI), 9th Edition](https://www.bipm.org/en/publications/si-brochure)
- [Wikipedia article describing the unit](https://en.wikipedia.org/wiki/Astronomical_unit)


**Formats:** [[JSON](astronomicalunit.json)] [[MD](astronomicalunit.md)]

**JSON definition:**

``` json
{
    "$schema": "https://schemas.optimade.org/meta/v1.2/optimade/physical_unit_definition.md",
    "$id": "https://schemas.optimade.org/defs/v1.2/units/si/2019/accepted/astronomicalunit",
    "title": "astronomical unit",
    "symbol": "astronomicalunit",
    "display-symbol": "au",
    "description": "A unit defined as exactly 149597870700 meters which is meant to represent the mean distance between the Earth and the Sun using the SI 1983 meter.\n\nThe International System of Units (SI), 9th ed. (2019) changed the definition of the astronomical unit given in prior editions into: \"1 au = 149 597 870 700 m\" with the footnote \"As decided at the XXVIII General Assembly of the International Astronomical Union (Resolution B2, 2012).\"\n\nThe International System of Units (SI), 9th ed. (2019) categorizes the astronomical unit as a \"non-SI unit accepted for use with the SI units\".",
    "resources": [
        {
            "relation": "Definition in the International System of Units (SI), 9th Edition",
            "resource-id": "https://www.bipm.org/en/publications/si-brochure"
        },
        {
            "relation": "Wikipedia article describing the unit",
            "resource-id": "https://en.wikipedia.org/wiki/Astronomical_unit"
        }
    ],
    "defining-relation": {
        "base-units": [
            {
                "symbol": "m",
                "id": "https://schemas.optimade.org/units/v1.2/si/1983/base/metre"
            }
        ],
        "base-units-expression": "m",
        "scale": {
            "numerator": 149597870700
        }
    },
    "x-optimade-definition": {
        "kind": "unit",
        "format": "1.2",
        "version": "1.2.0",
        "name": "astronomicalunit"
    }
}
```
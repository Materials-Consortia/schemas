# arcminute, ′ (unit)

This page documents an [OPTIMADE](https://www.optimade.org/) [Unit Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/defs/v1.2/units/si/general/arcminute`](https://schemas.optimade.org/defs/v1.2/units/si/general/arcminute.md)**  
**Definition name:** `arcminute`

**Unit name:** arcminute  
**Latin symbol:** arcmin  
**Display symbol:** ′  
  
**Description:** A unit of plane and phase angle equal to 1/60 of a degree representing 1/21600 of a circle, equal to π/10800 rad, using the current, or one of the historical, definitions of the SI units.

This definition uses "arcminute" as the unit name to distingush it from the time unit named minute.
A footnote in The International System of Units, 9th ed. (2019) note that "arcsecond is an alternative name for second of plane angle".
However, "arcminute" and "arcmin" have so far not been mentioned in any of the editions of the International System of Units.
They are defined in the GNU Units 3.15 unit database as 1/60 degree.

The unit appear under the name minute (with symbol ′) in the International System of Units (SI), 1st ed. (1970) defined as "1′ = (1/60)° = (π/10800) rad".

- The International System of Units (SI), 1st ed. (1970) categorizes the unit as "Units in use with the International System."
- The International System of Units (SI), 7th ed. (1998) adds as a footnote: "ISO 31 recommends that the degree be subdivided decimally rather than using the minute and second."
- The International System of Units (SI), 8th ed. (2006) further adds to that footnote: "For navigation and surveying, however, the minute has the advantage that one minute of latitude on the surface of the Earth corresponds (approximately) to one nautical mile."
- The International System of Units (SI), 9th ed. (2019) replaces the footnote with: "For some applications such as in astronomy, small angles are measured in arcseconds (i.e. seconds of plane angle), denoted as or ′′, or milliarcseconds, microarcseconds and picoarcseconds, denoted mas, μas and pas, respectively, where arcsecond is an alternative name for second of plane angle."
  The formulation "denoted as or ″" is reproduced here faithfully from the source and suggests an alternate symbol may have been omitted due to a typographical error.
  It is not clear what alternate symbol was intended to be referenced.

This is a generalized definition taken to reference the current, or one of the historical, SI unit definitions.
This definition is intended for situations when it is not possible to be more precise, e.g., in contexts where data have been collected that uses different historical SI definitions.

**Resources:**

- [Definition in the International System of Units (SI), 1th Edition](https://www.bipm.org/en/publications/si-brochure)
- [Wikipedia article describing the unit](https://en.wikipedia.org/wiki/Minute_and_second_of_arc)


**Formats:** [[JSON](arcminute.json)] [[MD](arcminute.md)]

**JSON definition:**

``` json
{
    "$schema": "https://schemas.optimade.org/meta/v1.2/optimade/physical_unit_definition.md",
    "$id": "https://schemas.optimade.org/defs/v1.2/units/si/general/arcminute",
    "title": "arcminute",
    "symbol": "arcmin",
    "display-symbol": "\u2032",
    "alternate-symbols": [
        "minute of arc",
        "minute of angle",
        "MOA",
        "'"
    ],
    "description": "A unit of plane and phase angle equal to 1/60 of a degree representing 1/21600 of a circle, equal to \u03c0/10800 rad, using the current, or one of the historical, definitions of the SI units.\n\nThis definition uses \"arcminute\" as the unit name to distingush it from the time unit named minute.\nA footnote in The International System of Units, 9th ed. (2019) note that \"arcsecond is an alternative name for second of plane angle\".\nHowever, \"arcminute\" and \"arcmin\" have so far not been mentioned in any of the editions of the International System of Units.\nThey are defined in the GNU Units 3.15 unit database as 1/60 degree.\n\nThe unit appear under the name minute (with symbol \u2032) in the International System of Units (SI), 1st ed. (1970) defined as \"1\u2032 = (1/60)\u00b0 = (\u03c0/10800) rad\".\n\n- The International System of Units (SI), 1st ed. (1970) categorizes the unit as \"Units in use with the International System.\"\n- The International System of Units (SI), 7th ed. (1998) adds as a footnote: \"ISO 31 recommends that the degree be subdivided decimally rather than using the minute and second.\"\n- The International System of Units (SI), 8th ed. (2006) further adds to that footnote: \"For navigation and surveying, however, the minute has the advantage that one minute of latitude on the surface of the Earth corresponds (approximately) to one nautical mile.\"\n- The International System of Units (SI), 9th ed. (2019) replaces the footnote with: \"For some applications such as in astronomy, small angles are measured in arcseconds (i.e. seconds of plane angle), denoted as or \u2032\u2032, or milliarcseconds, microarcseconds and picoarcseconds, denoted mas, \u03bcas and pas, respectively, where arcsecond is an alternative name for second of plane angle.\"\n  The formulation \"denoted as or \u2033\" is reproduced here faithfully from the source and suggests an alternate symbol may have been omitted due to a typographical error.\n  It is not clear what alternate symbol was intended to be referenced.\n\nThis is a generalized definition taken to reference the current, or one of the historical, SI unit definitions.\nThis definition is intended for situations when it is not possible to be more precise, e.g., in contexts where data have been collected that uses different historical SI definitions.",
    "compatibility": [
        "https://schemas.optimade.org/defs/v1.2/units/si/1970/accepted/arcminute"
    ],
    "resources": [
        {
            "relation": "Definition in the International System of Units (SI), 1th Edition",
            "resource-id": "https://www.bipm.org/en/publications/si-brochure"
        },
        {
            "relation": "Wikipedia article describing the unit",
            "resource-id": "https://en.wikipedia.org/wiki/Minute_and_second_of_arc"
        }
    ],
    "defining-relation": {
        "base-units": [
            {
                "symbol": "pi",
                "id": "https://schemas.optimade.org/defs/v1.2/constants/math/basic/pi"
            },
            {
                "symbol": "rad",
                "id": "https://schemas.optimade.org/defs/v1.2/units/si/general/radian"
            }
        ],
        "base-units-expression": "pi*rad",
        "scale": {
            "denominator": 10800
        }
    },
    "x-optimade-definition": {
        "label": "arcminute_si_general",
        "kind": "unit",
        "format": "1.2",
        "version": "1.2.0",
        "name": "arcminute"
    }
}
```
# degree, ° (unit)

This page documents an [OPTIMADE](https://www.optimade.org/) [Unit Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/defs/v1.2/units/si/general/degree`](https://schemas.optimade.org/defs/v1.2/units/si/general/degree.md)**  
**Definition name:** `degree`

**Unit name:** degree  
**Latin symbol:** degree  
**Display symbol:** °  
  
**Description:** A unit of plane and phase angle representing 1/360 of a full circle, equal to π/180 rad using the current, or one of the historical, definitions of the SI units.

With the current definition of raidan in the SI system, the degree is equal to 1/360 of a circle.

The degree appear in the International System of Units (SI), 1th ed. (1970) defined as "1° = (pi/180) rad".

- The International System of Units (SI), 1th ed. (1970) categorizes the unit as "Units in use with the International System."
- The International System of Units (SI), 7th ed. (1998) adds as a footnote: "ISO 31 recommends that the degree be subdivided decimally rather than using the minute and second."
- The International System of Units (SI), 8th ed. (2006) further adds to that footnote: "For navigation and surveying, however, the minute has the advantage that one minute of latitude on the surface of the Earth corresponds (approximately) to one nautical mile."
- The International System of Units (SI), 9th ed. (2019) replaces the footnote with: "For some applications such as in astronomy, small angles are measured in arcseconds (i.e. seconds of plane angle), denoted as or ′′, or milliarcseconds, microarcseconds and picoarcseconds, denoted mas, μas and pas, respectively, where arcsecond is an alternative name for second of plane angle."
  The formulation "denoted as or ″" is reproduced here faithfully from the source and suggests an alternate symbol may have been omitted due to a typographical error.
  It is not clear what alternate symbol was intended to be referenced.

This is a generalized definition taken to reference the current, or one of the historical, SI unit definitions.
This definition is intended for situations when it is not possible to be more precise, e.g., in contexts where data have been collected that uses different historical SI definitions.

**Resources:**

- [Definition in the International System of Units (SI), 9th Edition](https://www.bipm.org/en/publications/si-brochure)
- [Wikipedia article describing the unit](https://en.wikipedia.org/wiki/Degree_(angle))


**Formats:** [[JSON](degree.json)] [[MD](degree.md)]

**JSON definition:**

``` json
{
    "$schema": "https://schemas.optimade.org/meta/v1.2/optimade/physical_unit_definition.md",
    "$id": "https://schemas.optimade.org/defs/v1.2/units/si/general/degree",
    "title": "degree",
    "symbol": "degree",
    "display-symbol": "\u00b0",
    "description": "A unit of plane and phase angle representing 1/360 of a full circle, equal to \u03c0/180 rad using the current, or one of the historical, definitions of the SI units.\n\nWith the current definition of raidan in the SI system, the degree is equal to 1/360 of a circle.\n\nThe degree appear in the International System of Units (SI), 1th ed. (1970) defined as \"1\u00b0 = (pi/180) rad\".\n\n- The International System of Units (SI), 1th ed. (1970) categorizes the unit as \"Units in use with the International System.\"\n- The International System of Units (SI), 7th ed. (1998) adds as a footnote: \"ISO 31 recommends that the degree be subdivided decimally rather than using the minute and second.\"\n- The International System of Units (SI), 8th ed. (2006) further adds to that footnote: \"For navigation and surveying, however, the minute has the advantage that one minute of latitude on the surface of the Earth corresponds (approximately) to one nautical mile.\"\n- The International System of Units (SI), 9th ed. (2019) replaces the footnote with: \"For some applications such as in astronomy, small angles are measured in arcseconds (i.e. seconds of plane angle), denoted as or \u2032\u2032, or milliarcseconds, microarcseconds and picoarcseconds, denoted mas, \u03bcas and pas, respectively, where arcsecond is an alternative name for second of plane angle.\"\n  The formulation \"denoted as or \u2033\" is reproduced here faithfully from the source and suggests an alternate symbol may have been omitted due to a typographical error.\n  It is not clear what alternate symbol was intended to be referenced.\n\nThis is a generalized definition taken to reference the current, or one of the historical, SI unit definitions.\nThis definition is intended for situations when it is not possible to be more precise, e.g., in contexts where data have been collected that uses different historical SI definitions.",
    "compatibility": [
        "https://schemas.optimade.org/units/v1.2/si/1970/accepted/degree"
    ],
    "resources": [
        {
            "relation": "Definition in the International System of Units (SI), 9th Edition",
            "resource-id": "https://www.bipm.org/en/publications/si-brochure"
        },
        {
            "relation": "Wikipedia article describing the unit",
            "resource-id": "https://en.wikipedia.org/wiki/Degree_(angle)"
        }
    ],
    "defining-relation": {
        "base-units": [
            {
                "symbol": "pi",
                "id": "https://schema.optimade.org/units/constants/math/pi"
            },
            {
                "symbol": "rad",
                "id": "https://schema.optimade.org/units/si/general/radian"
            }
        ],
        "base-units-expression": "pi*rad",
        "scale": {
            "denomenator": 180
        }
    },
    "x-optimade-definition": {
        "kind": "unit",
        "format": "1.2",
        "version": "1.2.0",
        "name": "degree"
    }
}
```
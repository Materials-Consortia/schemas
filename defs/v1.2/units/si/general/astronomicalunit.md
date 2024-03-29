# astronomical unit, au (unit)

This page documents an [OPTIMADE](https://www.optimade.org/) [Unit Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/defs/v1.2/units/si/general/astronomicalunit`](https://schemas.optimade.org/defs/v1.2/units/si/general/astronomicalunit.md)**  
**Definition name:** `astronomicalunit`

**Unit name:** astronomical unit  
**Latin symbol:** au  
**Display symbol:** au  
  
**Description:** A unit of length representing the mean distance between the Earth and the Sun, using the current, or one of the historical, definitions given in the editions of the International System of Units (SI).

The current definition in the International System of Units (SI), 9th ed. (2019) is: "1 au = 149 597 870 700 m" with the footnote "As decided at the XXVIII General Assembly of the International Astronomical Union (Resolution B2, 2012)."

The prior definition in the International System of Units (SI), 1st ed. (1970) appears in a footnote: "The astronomical unit of distance is the length of the unperturbed circular orbit about the Sun of a body of infinitesimal mass in motion around the Sun with an angular sidereal velocity of 0.017202098950 radians per ephemeris day of 86,400 seconds. In the System of Astronomical Constants of the International Astronomical Union, the adopted value is: 1 AU = 149,600 x 10⁶ m."

This definition interprets the definition to be the expression in radians and seconds, with the meter value regarded only as an approximation.

- The International System of Units (SI), 1st ed. (1970) categorizes the unit as "Units for use with the SI in specific domains."
- The International System of Units (SI), 2nd ed. (1973) categorizes the unit as "Non-SI units accepted for use with the International System, whose values in SI units are obtained experimentally" and prefixes the footnote with: "This unit does not have an international symbol; abbreviations are used, for example, UA in French, AU in English, AG in German, а.е. in Russian, etc."
- The International System of Units (SI), 4th ed. (1981) omits the unit.
- The International System of Units (SI), 7th ed. (1998) reintroduces the unit in the category "Non-SI units accepted for use with the International System, whose values in SI units are obtained experimentally." with the experimental relationship "1 au = 1.49597870691(30)×10¹¹ m" with the footnote: "The astronomical unit is a unit of length approximatively equal to the mean Earth-Sun distance. Its value is such that, when used to describe the motion of bodies in the Solar System, the heliocentric gravitational constant is (0.01720209895)² ua³⋅d⁻²."
- The International System of Units (SI), 8th ed. (2006) notes the experimental relationship "1 au = 1.49597870691(6)×10¹¹ m" and changes the footnote to: "The astronomical unit is approximately equal to the mean Earth-Sun distance. It is the radius of an unperturbed circular Newtonian orbit about the Sun of a particle having infinitesimal mass, moving with a mean motion of 0.01720209895 radians per day (known as the Gaussian constant). The value given for the astronomical unit is quoted from the IERS Conventions 2003 (D.D. McCarthy and G. Petit eds., IERS Technical Note 32, Frankfurt am Main: Verlag des Bundesamts für Kartographie und Geodäsie, 2004, 12). The value of the astronomical unit in metres comes from the JPL ephemerides DE403 (Standish E.M., Report of the IAU WGAS Sub-Group on Numerical Standards, Highlights of Astronomy, Appenzeller ed., Dordrecht: Kluwer Academic Publishers, 1995, 180-184)."
- The International System of Units (SI), 9th ed. (2019) categorizes the astronomical unit as a "non-SI unit accepted for use with the SI units" and redefines it to have an exact relationship to the meter with the footnote: "As decided at the XXVIII General Assembly of the International Astronomical Union (Resolution B2, 2012)."

This is a generalized definition taken to reference the current, or one of the historical, SI unit definitions.
This definition is intended for situations when it is not possible to be more precise, e.g., in contexts where data have been collected that uses different historical SI definitions.

**Resources:**

- [Definition in the International System of Units (SI), 9th Edition](https://www.bipm.org/en/publications/si-brochure)
- [Wikipedia article describing the unit](https://en.wikipedia.org/wiki/Astronomical_unit)


**Compatibility:** (other definitions that are covered by the above definition)

- [`https://schemas.optimade.org/defs/v1.2/units/si/1970/accepted/astronomicalunit`](https://schemas.optimade.org/defs/v1.2/units/si/1970/accepted/astronomicalunit.md)
- [`https://schemas.optimade.org/defs/v1.2/units/si/2019/accepted/astronomicalunit`](https://schemas.optimade.org/defs/v1.2/units/si/2019/accepted/astronomicalunit.md)


**Formats:** [[JSON](astronomicalunit.json)] [[MD](astronomicalunit.md)]

**JSON definition:**

``` json
{
    "$id": "https://schemas.optimade.org/defs/v1.2/units/si/general/astronomicalunit",
    "$schema": "https://schemas.optimade.org/meta/v1.2/optimade/physical_unit_definition.json",
    "title": "astronomical unit",
    "symbol": "au",
    "display-symbol": "au",
    "description": "A unit of length representing the mean distance between the Earth and the Sun, using the current, or one of the historical, definitions given in the editions of the International System of Units (SI).\n\nThe current definition in the International System of Units (SI), 9th ed. (2019) is: \"1 au = 149 597 870 700 m\" with the footnote \"As decided at the XXVIII General Assembly of the International Astronomical Union (Resolution B2, 2012).\"\n\nThe prior definition in the International System of Units (SI), 1st ed. (1970) appears in a footnote: \"The astronomical unit of distance is the length of the unperturbed circular orbit about the Sun of a body of infinitesimal mass in motion around the Sun with an angular sidereal velocity of 0.017202098950 radians per ephemeris day of 86,400 seconds. In the System of Astronomical Constants of the International Astronomical Union, the adopted value is: 1 AU = 149,600 x 10\u2076 m.\"\n\nThis definition interprets the definition to be the expression in radians and seconds, with the meter value regarded only as an approximation.\n\n- The International System of Units (SI), 1st ed. (1970) categorizes the unit as \"Units for use with the SI in specific domains.\"\n- The International System of Units (SI), 2nd ed. (1973) categorizes the unit as \"Non-SI units accepted for use with the International System, whose values in SI units are obtained experimentally\" and prefixes the footnote with: \"This unit does not have an international symbol; abbreviations are used, for example, UA in French, AU in English, AG in German, \u0430.\u0435. in Russian, etc.\"\n- The International System of Units (SI), 4th ed. (1981) omits the unit.\n- The International System of Units (SI), 7th ed. (1998) reintroduces the unit in the category \"Non-SI units accepted for use with the International System, whose values in SI units are obtained experimentally.\" with the experimental relationship \"1 au = 1.49597870691(30)\u00d710\u00b9\u00b9 m\" with the footnote: \"The astronomical unit is a unit of length approximatively equal to the mean Earth-Sun distance. Its value is such that, when used to describe the motion of bodies in the Solar System, the heliocentric gravitational constant is (0.01720209895)\u00b2 ua\u00b3\u22c5d\u207b\u00b2.\"\n- The International System of Units (SI), 8th ed. (2006) notes the experimental relationship \"1 au = 1.49597870691(6)\u00d710\u00b9\u00b9 m\" and changes the footnote to: \"The astronomical unit is approximately equal to the mean Earth-Sun distance. It is the radius of an unperturbed circular Newtonian orbit about the Sun of a particle having infinitesimal mass, moving with a mean motion of 0.01720209895 radians per day (known as the Gaussian constant). The value given for the astronomical unit is quoted from the IERS Conventions 2003 (D.D. McCarthy and G. Petit eds., IERS Technical Note 32, Frankfurt am Main: Verlag des Bundesamts f\u00fcr Kartographie und Geod\u00e4sie, 2004, 12). The value of the astronomical unit in metres comes from the JPL ephemerides DE403 (Standish E.M., Report of the IAU WGAS Sub-Group on Numerical Standards, Highlights of Astronomy, Appenzeller ed., Dordrecht: Kluwer Academic Publishers, 1995, 180-184).\"\n- The International System of Units (SI), 9th ed. (2019) categorizes the astronomical unit as a \"non-SI unit accepted for use with the SI units\" and redefines it to have an exact relationship to the meter with the footnote: \"As decided at the XXVIII General Assembly of the International Astronomical Union (Resolution B2, 2012).\"\n\nThis is a generalized definition taken to reference the current, or one of the historical, SI unit definitions.\nThis definition is intended for situations when it is not possible to be more precise, e.g., in contexts where data have been collected that uses different historical SI definitions.",
    "compatibility": [
        "https://schemas.optimade.org/defs/v1.2/units/si/1970/accepted/astronomicalunit",
        "https://schemas.optimade.org/defs/v1.2/units/si/2019/accepted/astronomicalunit"
    ],
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
    "$comment": "While the approximate relation given is exact in the current definition of the SI system, this unit definition is a generalized definition that may also reference prior definitions of the astronomical unit, for which this relationship is only approximate.",
    "approximate-relations": [
        {
            "base-units": [
                {
                    "symbol": "m",
                    "id": "https://schemas.optimade.org/defs/v1.2/units/si/1960/base/metre"
                }
            ],
            "base-units-expression": "m",
            "scale": {
                "value": 149597870700
            }
        }
    ],
    "x-optimade-definition": {
        "label": "astronomicalunit_si_general",
        "kind": "unit",
        "format": "1.2",
        "version": "1.2.0",
        "name": "astronomicalunit"
    }
}
```
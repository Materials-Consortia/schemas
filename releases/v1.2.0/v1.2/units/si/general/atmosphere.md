# standard atmosphere, atm (unit)

This page documents an [OPTIMADE](https://www.optimade.org/) [Unit Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/defs/v1.2/units/si/general/atmosphere`](https://schemas.optimade.org/defs/v1.2/units/si/general/atmosphere.md)**  
**Definition name:** `atmosphere`

**Unit name:** standard atmosphere  
**Latin symbol:** atm  
**Display symbol:** atm  
  
**Description:** A unit for pressure approximately equal to the average atmospheric pressure at sea level on Earth using the current, or one of the historical, definitions of the SI units.

The standard atmosphere appear in the International System of Units (SI), 1th ed. (1970) defined as "1 atm = 101325 Pa" with the footnote "Resolution 4 at the 10th C.G.P.M. (1954)."
(While the pascal appear in the 1st ed. as a symbol for N·s/m², it was adopted into SI at the 14th CGPM meeting in 1971.)

- In the International System of Units (SI), 1th ed. (1970) it is categorized as "temporarily admitted" for use with the SI units.
- The International System of Units (SI), 4th ed. (1981) changes the categorization to "Other units generally deprecated" and adds to the footnote that: "The designation "standard atmosphere" for a reference pressure of 101 325 Pa is still acceptable."
- The International System of Units (SI), 7th ed. (1998) changes the categorization to "Examples of other non-SI units."
- The International System of Units (SI), 8th ed. (2006) omits the unit, but uses the term in a footnote to the definition of the unit bar to clarify that prior to 1982 the standard pressure used to tabulate thermodynamical data was the standard atmosphere.
- The International System of Units (SI), 9th ed. (2006) no longer references the unit or the designation "standard atomsphere".

This is a generalized definition taken to reference the current, or one of the historical, SI unit definitions.
This definition is intended for situations when it is not possible to be more precise, e.g., in contexts where data have been collected that uses different historical SI definitions.

**Resources:**

- [Definition in the International System of Units (SI), 9th Edition](https://www.bipm.org/en/publications/si-brochure)
- [Definition of pascal at the 14th CGPM Meeting (1971)](https://www.bipm.org/en/committees/cg/cgpm/14-1971)
- [Wikipedia article describing the unit](https://en.wikipedia.org/wiki/Standard_atmosphere_(unit))


**Formats:** [[JSON](atmosphere.json)] [[MD](atmosphere.md)]

**JSON definition:**

``` json
{
    "$schema": "https://schemas.optimade.org/meta/v1.2/optimade/physical_unit_definition.md",
    "$id": "https://schemas.optimade.org/defs/v1.2/units/si/general/atmosphere",
    "title": "standard atmosphere",
    "symbol": "atm",
    "display-symbol": "atm",
    "description": "A unit for pressure approximately equal to the average atmospheric pressure at sea level on Earth using the current, or one of the historical, definitions of the SI units.\n\nThe standard atmosphere appear in the International System of Units (SI), 1th ed. (1970) defined as \"1 atm = 101325 Pa\" with the footnote \"Resolution 4 at the 10th C.G.P.M. (1954).\"\n(While the pascal appear in the 1st ed. as a symbol for N\u00b7s/m\u00b2, it was adopted into SI at the 14th CGPM meeting in 1971.)\n\n- In the International System of Units (SI), 1th ed. (1970) it is categorized as \"temporarily admitted\" for use with the SI units.\n- The International System of Units (SI), 4th ed. (1981) changes the categorization to \"Other units generally deprecated\" and adds to the footnote that: \"The designation \"standard atmosphere\" for a reference pressure of 101 325 Pa is still acceptable.\"\n- The International System of Units (SI), 7th ed. (1998) changes the categorization to \"Examples of other non-SI units.\"\n- The International System of Units (SI), 8th ed. (2006) omits the unit, but uses the term in a footnote to the definition of the unit bar to clarify that prior to 1982 the standard pressure used to tabulate thermodynamical data was the standard atmosphere.\n- The International System of Units (SI), 9th ed. (2006) no longer references the unit or the designation \"standard atomsphere\".\n\nThis is a generalized definition taken to reference the current, or one of the historical, SI unit definitions.\nThis definition is intended for situations when it is not possible to be more precise, e.g., in contexts where data have been collected that uses different historical SI definitions.",
    "compatibility": [
        "https://schemas.optimade.org/units/v1.2/si/1970/accepted/atmosphere"
    ],
    "resources": [
        {
            "relation": "Definition in the International System of Units (SI), 9th Edition",
            "resource-id": "https://www.bipm.org/en/publications/si-brochure"
        },
        {
            "relation": "Definition of pascal at the 14th CGPM Meeting (1971)",
            "resource-id": "https://www.bipm.org/en/committees/cg/cgpm/14-1971"
        },
        {
            "relation": "Wikipedia article describing the unit",
            "resource-id": "https://en.wikipedia.org/wiki/Standard_atmosphere_(unit)"
        }
    ],
    "defining-relation": {
        "base-units": [
            {
                "symbol": "kg",
                "id": "https://schemas.optimade.org/units/v1.2/si/general/kilogram"
            },
            {
                "symbol": "m",
                "id": "https://schemas.optimade.org/units/v1.2/si/general/metre"
            },
            {
                "symbol": "s",
                "id": "https://schemas.optimade.org/units/v1.2/si/general/second"
            }
        ],
        "base-units-expression": "kg*m^-1*s^-2",
        "scale": {
            "numerator": 101325
        }
    },
    "x-optimade-definition": {
        "kind": "unit",
        "format": "1.2",
        "version": "1.2.0",
        "name": "atmosphere"
    }
}
```
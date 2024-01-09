# gal, Gal (unit)

This page documents an [OPTIMADE](https://www.optimade.org/) [Unit Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/defs/v1.2/units/si/1983/temporary/gal`](https://schemas.optimade.org/defs/v1.2/units/si/1983/temporary/gal.md)**  
**Definition name:** `gal`

**Unit name:** gal  
**Latin symbol:** Gal  
**Display symbol:** Gal  
  
**Description:** A unit of acceleration equal to 1 centimeter per second squared (1 cm/s²), defined according to the 1983 SI units.

The gal appear in the International System of Units (SI), 1st ed. (1970) defined as "1 Gal = 1 cm/s² = 10⁻² m/s²" with the footnote "The gal is a special unit of acceleration employed in geodesy and geophysics to express acceleration due to gravity."

- The International System of Units (SI), 1st ed. (1970) categorizes the unit as "units in use temporarily".
- The International System of Units (SI), 7th ed. (1998) changes the categorisation to "derived CGS units with special names".
- The International System of Units (SI), 9th ed. (2019) moves the unit definition to the margin aside the table for Non-SI units accepted for use with the SI units.
  It is not clear how to interprete the categorization intended with this placement of the unit.

The gal was implicitly redefined via the redefinition of the metre at the 17th CGPM meeting (1983), resolution 1.

**Resources:**

- [Definition in the International System of Units (SI), 1st Edition](https://www.bipm.org/en/publications/si-brochure)
- [Redefinition of the metre at the 17th CGPM meeting (1983), resolution 1](https://www.bipm.org/en/committees/cg/cgpm/17-1983/resolution-1)
- [Wikipedia article describing the unit](https://en.wikipedia.org/wiki/Gal_(unit))


**Formats:** [[JSON](gal.json)] [[MD](gal.md)]

**JSON definition:**

``` json
{
    "$id": "https://schemas.optimade.org/defs/v1.2/units/si/1983/temporary/gal",
    "$schema": "https://schemas.optimade.org/meta/v1.2/optimade/physical_unit_definition.json",
    "title": "gal",
    "symbol": "Gal",
    "display-symbol": "Gal",
    "description": "A unit of acceleration equal to 1 centimeter per second squared (1 cm/s\u00b2), defined according to the 1983 SI units.\n\nThe gal appear in the International System of Units (SI), 1st ed. (1970) defined as \"1 Gal = 1 cm/s\u00b2 = 10\u207b\u00b2 m/s\u00b2\" with the footnote \"The gal is a special unit of acceleration employed in geodesy and geophysics to express acceleration due to gravity.\"\n\n- The International System of Units (SI), 1st ed. (1970) categorizes the unit as \"units in use temporarily\".\n- The International System of Units (SI), 7th ed. (1998) changes the categorisation to \"derived CGS units with special names\".\n- The International System of Units (SI), 9th ed. (2019) moves the unit definition to the margin aside the table for Non-SI units accepted for use with the SI units.\n  It is not clear how to interprete the categorization intended with this placement of the unit.\n\nThe gal was implicitly redefined via the redefinition of the metre at the 17th CGPM meeting (1983), resolution 1.",
    "resources": [
        {
            "relation": "Definition in the International System of Units (SI), 1st Edition",
            "resource-id": "https://www.bipm.org/en/publications/si-brochure"
        },
        {
            "relation": "Redefinition of the metre at the 17th CGPM meeting (1983), resolution 1",
            "resource-id": "https://www.bipm.org/en/committees/cg/cgpm/17-1983/resolution-1"
        },
        {
            "relation": "Wikipedia article describing the unit",
            "resource-id": "https://en.wikipedia.org/wiki/Gal_(unit)"
        }
    ],
    "defining-relation": {
        "base-units": [
            {
                "symbol": "m",
                "id": "https://schemas.optimade.org/defs/v1.2/units/si/1983/base/metre"
            },
            {
                "symbol": "s",
                "id": "https://schemas.optimade.org/defs/v1.2/units/si/1967/base/second"
            }
        ],
        "base-units-expression": "m*s^-2",
        "scale": {
            "exponent": -2
        }
    },
    "x-optimade-definition": {
        "label": "gal_si_1983_temporary",
        "kind": "unit",
        "format": "1.2",
        "version": "1.2.0",
        "name": "gal"
    }
}
```
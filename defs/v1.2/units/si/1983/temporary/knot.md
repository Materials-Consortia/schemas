# knot, knot (unit)

This page documents an [OPTIMADE](https://www.optimade.org/) [Unit Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/defs/v1.2/units/si/1983/temporary/knot`](https://schemas.optimade.org/defs/v1.2/units/si/1983/temporary/knot.md)**  
**Definition name:** `knot`

**Unit name:** knot  
**Latin symbol:** knot  
**Display symbol:** knot  
  
**Description:** A unit of speed primarily used in navigation defined as 1 nautical mile per hour which is equal to (1852/3600) m/s using the 1983 SI units.

The knot appear in the International System of Units (SI), 1st ed. (1970) defined as "1 nautical mile per hour = (1852/3600) m/s."

- The International System of Units (SI), 1st ed. (1970) categorizes the unit as "Units in use temporarily with the International System."
- The International System of Units (SI), 7th ed. (1998) changes the categorization to "Other non-SI units currently accepted for use with the International System."
- The International System of Units (SI), 8th ed. (2006) changes the categorization to "Other non-SI units."
- The knot is omitted in the International System of Units (SI), 9th Edition (2019).

The knot was implicitly redefined via the redefinition of the metre at the 17th CGPM meeting (1983), resolution 1.

**Resources:**

- [Definition in the International System of Units (SI), 1st Edition](https://www.bipm.org/en/publications/si-brochure)
- [Redefinition of the metre at the 17th CGPM meeting (1983), resolution 1](https://www.bipm.org/en/committees/cg/cgpm/17-1983/resolution-1)
- [Wikipedia article describing the unit](https://en.wikipedia.org/wiki/Knot_(unit))


**Formats:** [[JSON](knot.json)] [[MD](knot.md)]

**JSON definition:**

``` json
{
    "$schema": "https://schemas.optimade.org/meta/v1.2/optimade/physical_unit_definition.md",
    "$id": "https://schemas.optimade.org/defs/v1.2/units/si/1983/temporary/knot",
    "title": "knot",
    "symbol": "knot",
    "display-symbol": "knot",
    "description": "A unit of speed primarily used in navigation defined as 1 nautical mile per hour which is equal to (1852/3600) m/s using the 1983 SI units.\n\nThe knot appear in the International System of Units (SI), 1st ed. (1970) defined as \"1 nautical mile per hour = (1852/3600) m/s.\"\n\n- The International System of Units (SI), 1st ed. (1970) categorizes the unit as \"Units in use temporarily with the International System.\"\n- The International System of Units (SI), 7th ed. (1998) changes the categorization to \"Other non-SI units currently accepted for use with the International System.\"\n- The International System of Units (SI), 8th ed. (2006) changes the categorization to \"Other non-SI units.\"\n- The knot is omitted in the International System of Units (SI), 9th Edition (2019).\n\nThe knot was implicitly redefined via the redefinition of the metre at the 17th CGPM meeting (1983), resolution 1.",
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
            "resource-id": "https://en.wikipedia.org/wiki/Knot_(unit)"
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
        "base-units-expression": "ms^-1",
        "scale": {
            "numerator": 1852,
            "denominator": 3600
        }
    },
    "x-optimade-definition": {
        "label": "knot_si_1983_temporary",
        "kind": "unit",
        "format": "1.2",
        "version": "1.2.0",
        "name": "knot"
    }
}
```
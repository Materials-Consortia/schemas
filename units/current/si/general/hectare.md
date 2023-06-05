# hectare, he (unit)
This page documents an [OPTIMADE](https://www.optimade.org/) [Unit Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/units/v1.2.0/si/general/hectare`](https://schemas.optimade.org/units/v1.2.0/si/general/hectare)**  
**Definition name:** `hectare`

**Unit name:** hectare  
**Latin symbol:** he  
**Display symbol:** he  
  
**Description:** A unit of area equal to 1000 square meters (1 hm²), using the current, or one of the historical, definitions of the SI units.

The hectare appear in the International System of Units (SI), 1th ed. (1970) defined as "1 ha = 1 hm² = 10⁴ m²" with the footnote "This unit and its symbol were adopted by the International Committee in 1879 (Proces-Verbaux C.I.P.M., 1879, p. 41).

The International System of Units (SI), 1th ed. (1970) categorizes the unit as "units in use temporarily".
The International System of Units (SI), 5th ed. (1985) add the clarification that the unit is "used to express agricultural areas."
The International System of Units (SI), 7th ed. (1998) changes the categorisation to "Other non-SI units currently accepted for use with the International System."

The hectare was implicitly redefined via the redefinition of the metre at the 17th CGPM meeting (1983), resolution 1.

This is a generalized definition taken to reference the current, or one of the historical, SI unit definitions.
This definition is intended for situations when it is not possible to be more precise, e.g., in contexts where data have been collected that uses different historical SI definitions.

**Resources:**

- [Definition in the International System of Units (SI), 9th Edition](https://www.bipm.org/en/publications/si-brochure)
- [Redefinition of the metre at the 17th CGPM meeting (1983), resolution 1](https://www.bipm.org/en/committees/cg/cgpm/17-1983/resolution-1)
- [Wikipedia article describing the unit](https://en.wikipedia.org/wiki/Hectare)


**Formats:** [[JSON](hectare.json)] [[MD](hectare.md)]

**JSON definition:**

``` json
{
    "$id": "https://schemas.optimade.org/units/v1.2.0/si/general/hectare",
    "title": "hectare",
    "symbol": "he",
    "display-symbol": "he",
    "description": "A unit of area equal to 1000 square meters (1 hm\u00b2), using the current, or one of the historical, definitions of the SI units.\n\nThe hectare appear in the International System of Units (SI), 1th ed. (1970) defined as \"1 ha = 1 hm\u00b2 = 10\u2074 m\u00b2\" with the footnote \"This unit and its symbol were adopted by the International Committee in 1879 (Proces-Verbaux C.I.P.M., 1879, p. 41).\n\nThe International System of Units (SI), 1th ed. (1970) categorizes the unit as \"units in use temporarily\".\nThe International System of Units (SI), 5th ed. (1985) add the clarification that the unit is \"used to express agricultural areas.\"\nThe International System of Units (SI), 7th ed. (1998) changes the categorisation to \"Other non-SI units currently accepted for use with the International System.\"\n\nThe hectare was implicitly redefined via the redefinition of the metre at the 17th CGPM meeting (1983), resolution 1.\n\nThis is a generalized definition taken to reference the current, or one of the historical, SI unit definitions.\nThis definition is intended for situations when it is not possible to be more precise, e.g., in contexts where data have been collected that uses different historical SI definitions.",
    "compatibility": [
        "https://schemas.optimade.org/units/v1.2.0/si/1970/temporary/hectare",
        "https://schemas.optimade.org/units/v1.2.0/si/1983/temporary/hectare"
    ],
    "standard": {
        "name": "gnu units",
        "version": "3.15",
        "symbol": "hectare"
    },
    "resources": [
        {
            "relation": "Definition in the International System of Units (SI), 9th Edition",
            "resource-id": "https://www.bipm.org/en/publications/si-brochure"
        },
        {
            "relation": "Redefinition of the metre at the 17th CGPM meeting (1983), resolution 1",
            "resource-id": "https://www.bipm.org/en/committees/cg/cgpm/17-1983/resolution-1"
        },
        {
            "relation": "Wikipedia article describing the unit",
            "resource-id": "https://en.wikipedia.org/wiki/Hectare"
        }
    ],
    "defining-relation": {
        "base-units": [
            {
                "symbol": "m",
                "id": "https://schema.optimade.org/units/v1.2.0/si/general/metre"
            }
        ],
        "base-units-expression": "m^2",
        "scale": {
            "exponent": 4
        }
    },
    "x-optimade-definition": {
        "kind": "unit",
        "format": "1.2",
        "version": "1.2.0",
        "name": "hectare"
    },
    "$schema": "https://schemas.optimade.org/meta/v1.2.0/optimade/physical_unit_definition.md"
}
```
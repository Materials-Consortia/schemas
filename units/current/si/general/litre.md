# litre, l (unit)
This page documents an [OPTIMADE](https://www.optimade.org/) [Unit Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/units/v1.2.0/si/general/litre`](https://schemas.optimade.org/units/v1.2.0/si/general/litre)**  
**Definition name:** `litre`

**Unit name:** litre  
**Latin symbol:** litre  
**Display symbol:** l  
  
**Description:** The litre, or liter is a unit of volume equal to a cubic decimetre (1 dm³) using the current, or one of the historical, definitions of the SI units.

"The 12th Conférence Générale des Poids et Mesures (CGPM) [...] declares that the word 'litre' may be employed as a special name for the cubic decimetre" [12th CGPM meeting (1964), resolution 6].

The litre was defined at the 12th CGPM meeting in 1964, resolution 6, and implicitly redefined with the redefinition of the metre at the 17th CGPM Meeting in 1983, resolution 1.

This is a generalized definition taken to reference the current, or one of the historical, SI unit definitions.
This definition is intended for situations when it is not possible to be more precise, e.g., in contexts where data have been collected that uses different historical SI definitions.

**Resources:**

- [Definition at the 12th CGPM meeting (1964), resolution 6](https://www.bipm.org/en/committees/cg/cgpm/12-1964/resolution-6)
- [Redefinition of the metre at the 17th CGPM meeting (1983), resolution 1](https://www.bipm.org/en/committees/cg/cgpm/17-1983/resolution-1)
- [Wikipedia article describing the unit](https://en.wikipedia.org/wiki/Litre)


**Formats:** [[JSON](litre.json)] [[MD](litre.md)]

**JSON definition:**

``` json
{
    "$id": "https://schemas.optimade.org/units/v1.2.0/si/general/litre",
    "title": "litre",
    "symbol": "litre",
    "display-symbol": "l",
    "alternate-symbols": [
        "L",
        "liter"
    ],
    "description": "The litre, or liter is a unit of volume equal to a cubic decimetre (1 dm\u00b3) using the current, or one of the historical, definitions of the SI units.\n\n\"The 12th Conf\u00e9rence G\u00e9n\u00e9rale des Poids et Mesures (CGPM) [...] declares that the word 'litre' may be employed as a special name for the cubic decimetre\" [12th CGPM meeting (1964), resolution 6].\n\nThe litre was defined at the 12th CGPM meeting in 1964, resolution 6, and implicitly redefined with the redefinition of the metre at the 17th CGPM Meeting in 1983, resolution 1.\n\nThis is a generalized definition taken to reference the current, or one of the historical, SI unit definitions.\nThis definition is intended for situations when it is not possible to be more precise, e.g., in contexts where data have been collected that uses different historical SI definitions.",
    "compatibility": [
        "https://schemas.optimade.org/units/v1.2.0/si/1964/accepted/litre",
        "https://schemas.optimade.org/units/v1.2.0/si/1983/accepted/litre"
    ],
    "standard": {
        "name": "gnu units",
        "version": "3.15",
        "symbol": "litre"
    },
    "resources": [
        {
            "relation": "Definition at the 12th CGPM meeting (1964), resolution 6",
            "resource-id": "https://www.bipm.org/en/committees/cg/cgpm/12-1964/resolution-6"
        },
        {
            "relation": "Redefinition of the metre at the 17th CGPM meeting (1983), resolution 1",
            "resource-id": "https://www.bipm.org/en/committees/cg/cgpm/17-1983/resolution-1"
        },
        {
            "relation": "Wikipedia article describing the unit",
            "resource-id": "https://en.wikipedia.org/wiki/Litre"
        }
    ],
    "defining-relation": {
        "base-units": [
            {
                "symbol": "m",
                "id": "https://schema.optimade.org/units/v1.2.0/si/general/metre"
            }
        ],
        "base-units-expression": "m^3",
        "scale": {
            "exponent": -3
        }
    },
    "x-optimade-definition": {
        "kind": "unit",
        "format": "1.2",
        "version": "1.2.0",
        "name": "litre"
    },
    "$schema": "https://schemas.optimade.org/meta/v1.2.0/optimade/physical_unit_definition.md"
}
```
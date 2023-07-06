# litre, l (unit)

This page documents an [OPTIMADE](https://www.optimade.org/) [Unit Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/defs/v1.2/units/si/1964/accepted/litre`](https://schemas.optimade.org/defs/v1.2/units/si/1964/accepted/litre)**  
**Definition name:** `litre`

**Unit name:** litre  
**Latin symbol:** litre  
**Display symbol:** l  
  
**Description:** The litre, or liter is a unit of volume equal to a cubic decimetre (1 dm³), with meter defined according to the 1960 SI units.

"The 12th Conférence Générale des Poids et Mesures (CGPM) [...] declares that the word 'litre' may be employed as a special name for the cubic decimetre" [12th CGPM meeting (1964), resolution 6].

**Resources:**

- [Definition at the 12th CGPM meeting (1964), resolution 6](https://www.bipm.org/en/committees/cg/cgpm/12-1964/resolution-6)
- [Wikipedia article describing the unit](https://en.wikipedia.org/wiki/Litre)


**Formats:** [[JSON](litre.json)] [[MD](litre.md)]

**JSON definition:**

``` json
{
    "$schema": "https://schemas.optimade.org/meta/v1.2/optimade/physical_unit_definition.md",
    "$id": "https://schemas.optimade.org/defs/v1.2/units/si/1964/accepted/litre",
    "title": "litre",
    "symbol": "litre",
    "display-symbol": "l",
    "alternate-symbols": [
        "L",
        "liter"
    ],
    "description": "The litre, or liter is a unit of volume equal to a cubic decimetre (1 dm\u00b3), with meter defined according to the 1960 SI units.\n\n\"The 12th Conf\u00e9rence G\u00e9n\u00e9rale des Poids et Mesures (CGPM) [...] declares that the word 'litre' may be employed as a special name for the cubic decimetre\" [12th CGPM meeting (1964), resolution 6].",
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
            "relation": "Wikipedia article describing the unit",
            "resource-id": "https://en.wikipedia.org/wiki/Litre"
        }
    ],
    "defining-relation": {
        "base-units": [
            {
                "symbol": "m",
                "id": "https://schema.optimade.org/units/si/1960/base/metre"
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
    }
}
```
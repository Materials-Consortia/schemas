# becquerel, Bq (unit)

This page documents an [OPTIMADE](https://www.optimade.org/) [Unit Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/defs/v1.2/units/si/general/becquerel`](https://schemas.optimade.org/defs/v1.2/units/si/general/becquerel.md)**  
**Definition name:** `becquerel`

**Unit name:** becquerel  
**Latin symbol:** Bq  
**Display symbol:** Bq  
  
**Description:** A unit for radioactivity, defined as s⁻¹ using the current, or one of the historical, definitions of the SI units.

"The 15th Conférence Générale des Poids et Mesures, [...] adopts the following special name for the SI unit of activity: becquerel, symbol Bq, equal to one reciprocal second." [15th CGPM Meeting (1975)]

This is a generalized definition taken to reference the current, or one of the historical, SI unit definitions.
This definition is intended for situations when it is not possible to be more precise, e.g., in contexts where data have been collected that uses different historical SI definitions.

**Resources:**

- [Definition at the 15th CGPM Meeting (1975)](https://www.bipm.org/en/committees/cg/cgpm/15-1975)
- [Wikipedia article describing the unit](https://en.wikipedia.org/wiki/Becquerel)


**Compatibility:** (other definitions that are covered by the above definition)

- [`https://schemas.optimade.org/defs/v1.2/units/si/1975/named/becquerel`](https://schemas.optimade.org/defs/v1.2/units/si/1975/named/becquerel.md)


**Formats:** [[JSON](becquerel.json)] [[MD](becquerel.md)]

**JSON definition:**

``` json
{
    "$id": "https://schemas.optimade.org/defs/v1.2/units/si/general/becquerel",
    "$schema": "https://schemas.optimade.org/meta/v1.2/optimade/physical_unit_definition.json",
    "title": "becquerel",
    "symbol": "Bq",
    "display-symbol": "Bq",
    "description": "A unit for radioactivity, defined as s\u207b\u00b9 using the current, or one of the historical, definitions of the SI units.\n\n\"The 15th Conf\u00e9rence G\u00e9n\u00e9rale des Poids et Mesures, [...] adopts the following special name for the SI unit of activity: becquerel, symbol Bq, equal to one reciprocal second.\" [15th CGPM Meeting (1975)]\n\nThis is a generalized definition taken to reference the current, or one of the historical, SI unit definitions.\nThis definition is intended for situations when it is not possible to be more precise, e.g., in contexts where data have been collected that uses different historical SI definitions.",
    "compatibility": [
        "https://schemas.optimade.org/defs/v1.2/units/si/1975/named/becquerel"
    ],
    "resources": [
        {
            "relation": "Definition at the 15th CGPM Meeting (1975)",
            "resource-id": "https://www.bipm.org/en/committees/cg/cgpm/15-1975"
        },
        {
            "relation": "Wikipedia article describing the unit",
            "resource-id": "https://en.wikipedia.org/wiki/Becquerel"
        }
    ],
    "defining-relation": {
        "base-units": [
            {
                "symbol": "s",
                "id": "https://schemas.optimade.org/defs/v1.2/units/si/general/second"
            }
        ],
        "base-units-expression": "s^-1"
    },
    "x-optimade-definition": {
        "label": "becquerel_si_general",
        "kind": "unit",
        "format": "1.2",
        "version": "1.2.0",
        "name": "becquerel"
    }
}
```
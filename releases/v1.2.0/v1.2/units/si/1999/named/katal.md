# katal, kat (unit)

This page documents an [OPTIMADE](https://www.optimade.org/) [Unit Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/defs/v1.2/units/si/1999/named/katal`](https://schemas.optimade.org/defs/v1.2/units/si/1999/named/katal.md)**  
**Definition name:** `katal`

**Unit name:** katal  
**Latin symbol:** kat  
**Display symbol:** kat  
  
**Description:** A derived SI unit for catalytic activity, defined as mol·s⁻¹ defined at the 21th CGPM meeting in 1999.

"The 21st Conférence Générale des Poids et Mesures, [...] decides to adopt the special name katal, symbol kat, for the SI unit mole per second to express catalytic activity, especially in the fields of medicine and biochemistry, and recommends that when the katal is used, the measurand be specified by reference to the measurement procedure; the measurement procedure must identify the indicator reaction." [21th CGPM meeting (1999), resolution 12]

**Resources:**

- [Definition of the unit at the 21st CGPM (1999)](https://www.bipm.org/en/committees/cg/cgpm/21-1999/resolution-12)
- [Wikipedia article describing the unit](https://en.wikipedia.org/wiki/Katal)


**Formats:** [[JSON](katal.json)] [[MD](katal.md)]

**JSON definition:**

``` json
{
    "$schema": "https://schemas.optimade.org/meta/v1.2/optimade/physical_unit_definition.md",
    "$id": "https://schemas.optimade.org/defs/v1.2/units/si/1999/named/katal",
    "title": "katal",
    "symbol": "kat",
    "display-symbol": "kat",
    "description": "A derived SI unit for catalytic activity, defined as mol\u00b7s\u207b\u00b9 defined at the 21th CGPM meeting in 1999.\n\n\"The 21st Conf\u00e9rence G\u00e9n\u00e9rale des Poids et Mesures, [...] decides to adopt the special name katal, symbol kat, for the SI unit mole per second to express catalytic activity, especially in the fields of medicine and biochemistry, and recommends that when the katal is used, the measurand be specified by reference to the measurement procedure; the measurement procedure must identify the indicator reaction.\" [21th CGPM meeting (1999), resolution 12]",
    "resources": [
        {
            "relation": "Definition of the unit at the 21st CGPM (1999)",
            "resource-id": "https://www.bipm.org/en/committees/cg/cgpm/21-1999/resolution-12"
        },
        {
            "relation": "Wikipedia article describing the unit",
            "resource-id": "https://en.wikipedia.org/wiki/Katal"
        }
    ],
    "defining-relation": {
        "base-units": [
            {
                "symbol": "mol",
                "id": "https://schemas.optimade.org/units/v1.2/si/1971/base/mole"
            },
            {
                "symbol": "s",
                "id": "https://schemas.optimade.org/units/v1.2/si/1967/base/second"
            }
        ],
        "base-units-expression": "mol*s^-1"
    },
    "x-optimade-definition": {
        "kind": "unit",
        "format": "1.2",
        "version": "1.2.0",
        "name": "katal"
    }
}
```
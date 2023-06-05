# katal, kat (unit)
This page documents an [OPTIMADE](https://www.optimade.org/) [Unit Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/units/v1.2.0/si/general/katal`](https://schemas.optimade.org/units/v1.2.0/si/general/katal)**  
**Definition name:** `katal`

**Unit name:** katal  
**Latin symbol:** kat  
**Display symbol:** kat  
  
**Description:** A derived SI unit for catalytic activity, defined as mol·s⁻¹ using the current, or one of the historical, definitions of the SI units.

"The 21st Conférence Générale des Poids et Mesures, [...] decides to adopt the special name katal, symbol kat, for the SI unit mole per second to express catalytic activity, especially in the fields of medicine and biochemistry, and recommends that when the katal is used, the measurand be specified by reference to the measurement procedure; the measurement procedure must identify the indicator reaction." [21th CGPM meeting (1999), resolution 12]

The katal was implicitly redefined via the redefinition of the mole at the 26th CGPM Meeting (2018), resolution 1.

This is a generalized definition taken to reference the current, or one of the historical, SI unit definitions.
This definition is intended for situations when it is not possible to be more precise, e.g., in contexts where data have been collected that uses different historical SI definitions.

**Resources:**

- [Wikipedia article describing the unit](https://en.wikipedia.org/wiki/Katal)


**Formats:** [[JSON](katal.json)] [[MD](katal.md)]

**JSON definition:**

``` json
{
    "$id": "https://schemas.optimade.org/units/v1.2.0/si/general/katal",
    "title": "katal",
    "symbol": "kat",
    "display-symbol": "kat",
    "description": "A derived SI unit for catalytic activity, defined as mol\u00b7s\u207b\u00b9 using the current, or one of the historical, definitions of the SI units.\n\n\"The 21st Conf\u00e9rence G\u00e9n\u00e9rale des Poids et Mesures, [...] decides to adopt the special name katal, symbol kat, for the SI unit mole per second to express catalytic activity, especially in the fields of medicine and biochemistry, and recommends that when the katal is used, the measurand be specified by reference to the measurement procedure; the measurement procedure must identify the indicator reaction.\" [21th CGPM meeting (1999), resolution 12]\n\nThe katal was implicitly redefined via the redefinition of the mole at the 26th CGPM Meeting (2018), resolution 1.\n\nThis is a generalized definition taken to reference the current, or one of the historical, SI unit definitions.\nThis definition is intended for situations when it is not possible to be more precise, e.g., in contexts where data have been collected that uses different historical SI definitions.",
    "compatibility": [
        "https://schemas.optimade.org/units/v1.2.0/si/1999/named/katal",
        "https://schemas.optimade.org/units/v1.2.0/si/2019/named/katal"
    ],
    "standard": {
        "name": "gnu units",
        "version": "3.15",
        "symbol": "katal"
    },
    "resources": [
        {
            "relation": "Wikipedia article describing the unit",
            "resource-id": "https://en.wikipedia.org/wiki/Katal"
        }
    ],
    "defining-relation": {
        "base-units": [
            {
                "symbol": "mol",
                "id": "https://schemas.optimade.org/units/v1.2.0/si/general/mole"
            },
            {
                "symbol": "s",
                "id": "https://schemas.optimade.org/units/v1.2.0/si/general/second"
            }
        ],
        "base-units-expression": "mol*s^-1"
    },
    "x-optimade-definition": {
        "kind": "unit",
        "format": "1.2",
        "version": "1.2.0",
        "name": "katal"
    },
    "$schema": "https://schemas.optimade.org/meta/v1.2.0/optimade/physical_unit_definition.md"
}
```
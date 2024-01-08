# sievert, Sv (unit)

This page documents an [OPTIMADE](https://www.optimade.org/) [Unit Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/defs/v1.2/units/si/1983/named/sievert`](https://schemas.optimade.org/defs/v1.2/units/si/1983/named/sievert.md)**  
**Definition name:** `sievert`

**Unit name:** sievert  
**Latin symbol:** Sv  
**Display symbol:** Sv  
  
**Description:** A derived SI unit for equivalent dose of ionizing radiation equal to m²·s⁻² using the 1983 SI base units.

"The 16th Conférence Générale des Poids et Mesures, [...] adopts the special name sievert, symbol Sv, for the SI unit of dose equivalent in the field of radioprotection. The sievert is equal to the joule per kilogram." [16th CGPM meeting (1979), resolution 5]

The sievert was defined at the 16th CGPM meeting in 1979 and implicitly redefined via the redefinition of the meter at the 17th CGPM Meeting in 1983, resolution 1.

**Resources:**

- [Definition at the 16th CGPM meeting (1979), resolution 5](https://www.bipm.org/en/committees/cg/cgpm/16-1979/resolution-5)
- [Redefinition of the metre at the 17th CGPM meeting (1983), resolution 1](https://www.bipm.org/en/committees/cg/cgpm/17-1983/resolution-1)
- [Wikipedia article describing the unit](https://en.wikipedia.org/wiki/Sievert)


**Formats:** [[JSON](sievert.json)] [[MD](sievert.md)]

**JSON definition:**

``` json
{
    "$schema": "https://schemas.optimade.org/meta/v1.2/optimade/physical_unit_definition.md",
    "$id": "https://schemas.optimade.org/defs/v1.2/units/si/1983/named/sievert",
    "title": "sievert",
    "symbol": "Sv",
    "display-symbol": "Sv",
    "description": "A derived SI unit for equivalent dose of ionizing radiation equal to m\u00b2\u00b7s\u207b\u00b2 using the 1983 SI base units.\n\n\"The 16th Conf\u00e9rence G\u00e9n\u00e9rale des Poids et Mesures, [...] adopts the special name sievert, symbol Sv, for the SI unit of dose equivalent in the field of radioprotection. The sievert is equal to the joule per kilogram.\" [16th CGPM meeting (1979), resolution 5]\n\nThe sievert was defined at the 16th CGPM meeting in 1979 and implicitly redefined via the redefinition of the meter at the 17th CGPM Meeting in 1983, resolution 1.",
    "resources": [
        {
            "relation": "Definition at the 16th CGPM meeting (1979), resolution 5",
            "resource-id": "https://www.bipm.org/en/committees/cg/cgpm/16-1979/resolution-5"
        },
        {
            "relation": "Redefinition of the metre at the 17th CGPM meeting (1983), resolution 1",
            "resource-id": "https://www.bipm.org/en/committees/cg/cgpm/17-1983/resolution-1"
        },
        {
            "relation": "Wikipedia article describing the unit",
            "resource-id": "https://en.wikipedia.org/wiki/Sievert"
        }
    ],
    "defining-relation": {
        "base-units": [
            {
                "symbol": "m",
                "id": "https://schemas.optimade.org/defs/v1.2/units/si/1960/base/metre"
            },
            {
                "symbol": "s",
                "id": "https://schemas.optimade.org/defs/v1.2/units/si/1967/base/second"
            }
        ],
        "base-units-expression": "m^2*s^-2"
    },
    "standard": {
        "name": "si",
        "year": 1983,
        "category": "named",
        "symbol": "Sv"
    },
    "x-optimade-definition": {
        "label": "sievert_si_1983_named",
        "kind": "unit",
        "format": "1.2",
        "version": "1.2.0",
        "name": "sievert"
    }
}
```
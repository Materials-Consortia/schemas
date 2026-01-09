# candela, cd (unit)

This page documents an [OPTIMADE](https://www.optimade.org/) [Unit Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/defs/v1.2/units/si/1979/base/candela`](https://schemas.optimade.org/defs/v1.2/units/si/1979/base/candela.md)**  
**Definition name:** `candela`

**Unit name:** candela  
**Latin symbol:** cd  
**Display symbol:** cd  
  
**Description:** The SI base unit of luminous intensity in a given direction defined from the luminous intensity of monochromatic radiation at a specific frequency and radiant intensity at the 16th CGPM Meeting in 1979.

"The candela is the luminous intensity, in a given direction, of a source that emits monochromatic radiation of frequency 540×10¹² hertz and that has a radiant intensity in that direction of 1/683 watt per steradian." [16th CGPM Meeting (1979), resolution 3].

The hertz, watt, and steradian units referenced in this definition are:

- the SI 1967 derived hertz unit (https://schemas.optimade.org/defs/v1.2/units/si/1967/named/hertz) equal to second⁻¹, referencing the SI 1967 base unit second (https://schemas.optimade.org/defs/v1.2/units/si/1967/base/second).
- the SI 1967 derived watt unit (https://schemas.optimade.org/defs/v1.2/units/si/1967/named/watt) equal to kilogram·meter²·second⁻³, referencing the SI 1960 base unit kilogram (https://schemas.optimade.org/defs/v1.2/units/si/1960/base/kilogram) and metre (https://schemas.optimade.org/defs/v1.2/units/si/1960/base/metre); and the 1967 base unit second (https://schemas.optimade.org/defs/v1.2/units/si/1967/base/second).
- the SI 1960 supplementary unit steradian (https://schemas.optimade.org/defs/v1.2/units/si/1960/supplementary/steradian).

**Resources:**

- [Redefinition of the candela at the 16th CGPM Meeting in 1979, resolution 3.](https://www.bipm.org/en/committees/cg/cgpm/16-1979/resolution-3)
- [Previous definition at the 13th CGPM meeting (1967)](https://www.bipm.org/en/committees/cg/cgpm/13-1967/resolution-5)
- [Wikipedia article describing the unit](https://en.wikipedia.org/wiki/Candela)


**Formats:** [[JSON](candela.json)] [[MD](candela.md)]

**JSON definition:**

``` json
{
    "$id": "https://schemas.optimade.org/defs/v1.2/units/si/1979/base/candela",
    "$schema": "https://schemas.optimade.org/meta/v1.2/optimade/physical_unit_definition.json",
    "title": "candela",
    "symbol": "cd",
    "display-symbol": "cd",
    "description": "The SI base unit of luminous intensity in a given direction defined from the luminous intensity of monochromatic radiation at a specific frequency and radiant intensity at the 16th CGPM Meeting in 1979.\n\n\"The candela is the luminous intensity, in a given direction, of a source that emits monochromatic radiation of frequency 540\u00d710\u00b9\u00b2 hertz and that has a radiant intensity in that direction of 1/683 watt per steradian.\" [16th CGPM Meeting (1979), resolution 3].\n\nThe hertz, watt, and steradian units referenced in this definition are:\n\n- the SI 1967 derived hertz unit (https://schemas.optimade.org/defs/v1.2/units/si/1967/named/hertz) equal to second\u207b\u00b9, referencing the SI 1967 base unit second (https://schemas.optimade.org/defs/v1.2/units/si/1967/base/second).\n- the SI 1967 derived watt unit (https://schemas.optimade.org/defs/v1.2/units/si/1967/named/watt) equal to kilogram\u00b7meter\u00b2\u00b7second\u207b\u00b3, referencing the SI 1960 base unit kilogram (https://schemas.optimade.org/defs/v1.2/units/si/1960/base/kilogram) and metre (https://schemas.optimade.org/defs/v1.2/units/si/1960/base/metre); and the 1967 base unit second (https://schemas.optimade.org/defs/v1.2/units/si/1967/base/second).\n- the SI 1960 supplementary unit steradian (https://schemas.optimade.org/defs/v1.2/units/si/1960/supplementary/steradian).",
    "resources": [
        {
            "relation": "Redefinition of the candela at the 16th CGPM Meeting in 1979, resolution 3.",
            "resource-id": "https://www.bipm.org/en/committees/cg/cgpm/16-1979/resolution-3"
        },
        {
            "relation": "Previous definition at the 13th CGPM meeting (1967)",
            "resource-id": "https://www.bipm.org/en/committees/cg/cgpm/13-1967/resolution-5"
        },
        {
            "relation": "Wikipedia article describing the unit",
            "resource-id": "https://en.wikipedia.org/wiki/Candela"
        }
    ],
    "standard": {
        "name": "si",
        "year": 1979,
        "category": "base",
        "symbol": "cd"
    },
    "x-optimade-definition": {
        "label": "candela_si_1979_base",
        "kind": "unit",
        "format": "1.2",
        "version": "1.2.0",
        "name": "candela"
    }
}
```
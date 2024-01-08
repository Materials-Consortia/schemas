# candela, cd (unit)

This page documents an [OPTIMADE](https://www.optimade.org/) [Unit Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/defs/v1.2/units/si/1960/base/candela`](https://schemas.optimade.org/defs/v1.2/units/si/1960/base/candela.md)**  
**Definition name:** `candela`

**Unit name:** candela  
**Latin symbol:** cd  
**Display symbol:** cd  
  
**Description:** The SI base unit of luminous intensity in a given direction defined from the radiation of a black body at the solidification temperature of platinum, which was included into SI at the 11th CGPM Meeting in 1960.

"The candela is the sixtieth of the luminous intensity emitted perpendicularly by one square centimeter of a perfect radiator (black body) at the solidification temperature of platinum." [9th CGPM meeting (1948)].
This was a ratification of a definition of a definition at the 41st CIPM meeting in 1946, resolution 1, with a different phrasing: "The value of the new candle is such that the brightness of the full radiator at the temperature of solidification of platinum is 60 new candles per square centimetre."
The candela was adopted into SI at the 11th CGPM Meeting in 1960, resolution 12.

Furthermore, in the definition SI 1960 definition of the candela the centimeter in the definition references 10⁻² times the SI 1960 metre (https://schemas.optimade.org/units/v1.2/si/1960/base/metre).

**Resources:**

- [Definition at the 9st CGPM meeting (1948)](https://www.bipm.org/en/committees/cg/cgpm/9-1948)
- [Related definition at the 41st CIPM meeting (1946)](https://www.bipm.org/en/committees/ci/cipm/41-1946/resolution-1)
- [Establishment of the SI unit system at the 11th CGPM meeting (1960), resolution 12.](https://www.bipm.org/en/committees/cg/cgpm/11-1960/resolution-12)
- [Wikipedia article describing the unit](https://en.wikipedia.org/wiki/Candela)


**Formats:** [[JSON](candela.json)] [[MD](candela.md)]

**JSON definition:**

``` json
{
    "$schema": "https://schemas.optimade.org/meta/v1.2/optimade/physical_unit_definition.md",
    "$id": "https://schemas.optimade.org/defs/v1.2/units/si/1960/base/candela",
    "title": "candela",
    "symbol": "cd",
    "display-symbol": "cd",
    "description": "The SI base unit of luminous intensity in a given direction defined from the radiation of a black body at the solidification temperature of platinum, which was included into SI at the 11th CGPM Meeting in 1960.\n\n\"The candela is the sixtieth of the luminous intensity emitted perpendicularly by one square centimeter of a perfect radiator (black body) at the solidification temperature of platinum.\" [9th CGPM meeting (1948)].\nThis was a ratification of a definition of a definition at the 41st CIPM meeting in 1946, resolution 1, with a different phrasing: \"The value of the new candle is such that the brightness of the full radiator at the temperature of solidification of platinum is 60 new candles per square centimetre.\"\nThe candela was adopted into SI at the 11th CGPM Meeting in 1960, resolution 12.\n\nFurthermore, in the definition SI 1960 definition of the candela the centimeter in the definition references 10\u207b\u00b2 times the SI 1960 metre (https://schemas.optimade.org/units/v1.2/si/1960/base/metre).",
    "resources": [
        {
            "relation": "Definition at the 9st CGPM meeting (1948)",
            "resource-id": "https://www.bipm.org/en/committees/cg/cgpm/9-1948"
        },
        {
            "relation": "Related definition at the 41st CIPM meeting (1946)",
            "resource-id": "https://www.bipm.org/en/committees/ci/cipm/41-1946/resolution-1"
        },
        {
            "relation": "Establishment of the SI unit system at the 11th CGPM meeting (1960), resolution 12.",
            "resource-id": "https://www.bipm.org/en/committees/cg/cgpm/11-1960/resolution-12"
        },
        {
            "relation": "Wikipedia article describing the unit",
            "resource-id": "https://en.wikipedia.org/wiki/Candela"
        }
    ],
    "standard": {
        "name": "si",
        "year": 1960,
        "category": "base",
        "symbol": "cd"
    },
    "x-optimade-definition": {
        "label": "candela_si_1960_base",
        "kind": "unit",
        "format": "1.2",
        "version": "1.2.0",
        "name": "candela"
    }
}
```
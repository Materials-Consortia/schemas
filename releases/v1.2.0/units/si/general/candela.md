# candela, cd (unit)

This page documents an [OPTIMADE](https://www.optimade.org/) [Unit Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/defs/v1.2/units/si/general/candela`](https://schemas.optimade.org/defs/v1.2/units/si/general/candela)**  
**Definition name:** `candela`

**Unit name:** candela  
**Latin symbol:** cd  
**Display symbol:** cd  
  
**Description:** A unit of luminous intensity in a given direction defined according to the current, or one of the historical, definitions of the SI units.

The current definition in its most recent phrasing at the 26th CGPM Meeting in 2018, resolution 1 is: "The candela, symbol cd, is the SI unit of luminous intensity in a given direction. It is defined by taking the fixed numerical value of the luminous efficacy of monochromatic radiation of frequency 540×10¹² Hz, \(K_\mathrm{cd}\), to be 683 when expressed in the unit lm⋅W⁻¹, which is equal to cd⋅sr⋅W⁻¹, or cd⋅sr⋅kg⁻¹⋅m⁻²⋅s³, where the kilogram, metre and second are defined in terms of \(h\), \(c\) and \(\Delta \nu_\textrm{Cs}\)."

This is a rephrasing of a definition at the 16th CGPM Meeting (1979), resolution 3: "The candela is the luminous intensity, in a given direction, of a source that emits monochromatic radiation of frequency 540×10¹² hertz and that has a radiant intensity in that direction of 1/683 watt per steradian."

Earlier different definitions of the candela were:

- "The candela is the luminous intensity, in a given direction, of a source that emits monochromatic radiation of frequency 540×10¹² hertz and that has a radiant intensity in that direction of 1/683 watt per steradian." [16th CGPM Meeting (1979), resolution 3].
- "The candela is the sixtieth of the luminous intensity emitted perpendicularly by one square centimeter of a perfect radiator (black body) at the solidification temperature of platinum." [9th CGPM meeting (1948)] (this definition was adopted into the SI system at the 11th CGPM Meeting in 1960, resolution 12).

This is a generalized definition taken to reference the current, or one of the historical, SI unit definitions.
This definition is intended for situations when it is not possible to be more precise, e.g., in contexts where data have been collected that uses different historical SI definitions.

**Resources:**

- [Definition in the 26th CGPM Meeting in 2018, resolution 1](https://www.bipm.org/en/committees/cg/cgpm/26-2018/resolution-1)
- [Definition in the International System of Units (SI), 9th Edition](https://www.bipm.org/en/publications/si-brochure)
- [Wikipedia article describing the unit](https://en.wikipedia.org/wiki/Candela)


**Formats:** [[JSON](candela.json)] [[MD](candela.md)]

**JSON definition:**

``` json
{
    "$schema": "https://schemas.optimade.org/meta/v1.2/optimade/physical_unit_definition.md",
    "$id": "https://schemas.optimade.org/defs/v1.2/units/si/general/candela",
    "title": "candela",
    "symbol": "cd",
    "display-symbol": "cd",
    "description": "A unit of luminous intensity in a given direction defined according to the current, or one of the historical, definitions of the SI units.\n\nThe current definition in its most recent phrasing at the 26th CGPM Meeting in 2018, resolution 1 is: \"The candela, symbol cd, is the SI unit of luminous intensity in a given direction. It is defined by taking the fixed numerical value of the luminous efficacy of monochromatic radiation of frequency 540\u00d710\u00b9\u00b2 Hz, \\(K_\\mathrm{cd}\\), to be 683 when expressed in the unit lm\u22c5W\u207b\u00b9, which is equal to cd\u22c5sr\u22c5W\u207b\u00b9, or cd\u22c5sr\u22c5kg\u207b\u00b9\u22c5m\u207b\u00b2\u22c5s\u00b3, where the kilogram, metre and second are defined in terms of \\(h\\), \\(c\\) and \\(\\Delta \\nu_\\textrm{Cs}\\).\"\n\nThis is a rephrasing of a definition at the 16th CGPM Meeting (1979), resolution 3: \"The candela is the luminous intensity, in a given direction, of a source that emits monochromatic radiation of frequency 540\u00d710\u00b9\u00b2 hertz and that has a radiant intensity in that direction of 1/683 watt per steradian.\"\n\nEarlier different definitions of the candela were:\n\n- \"The candela is the luminous intensity, in a given direction, of a source that emits monochromatic radiation of frequency 540\u00d710\u00b9\u00b2 hertz and that has a radiant intensity in that direction of 1/683 watt per steradian.\" [16th CGPM Meeting (1979), resolution 3].\n- \"The candela is the sixtieth of the luminous intensity emitted perpendicularly by one square centimeter of a perfect radiator (black body) at the solidification temperature of platinum.\" [9th CGPM meeting (1948)] (this definition was adopted into the SI system at the 11th CGPM Meeting in 1960, resolution 12).\n\nThis is a generalized definition taken to reference the current, or one of the historical, SI unit definitions.\nThis definition is intended for situations when it is not possible to be more precise, e.g., in contexts where data have been collected that uses different historical SI definitions.",
    "compatibility": [
        "https://schemas.optimade.org/units/v1.2/si/1960/base/candela",
        "https://schemas.optimade.org/units/v1.2/si/1967/base/candela",
        "https://schemas.optimade.org/units/v1.2/si/1979/base/candela",
        "https://schemas.optimade.org/units/v1.2/si/1983/base/candela",
        "https://schemas.optimade.org/units/v1.2/si/2019/base/candela"
    ],
    "standard": {
        "name": "gnu units",
        "version": "3.15",
        "symbol": "candela"
    },
    "resources": [
        {
            "relation": "Definition in the 26th CGPM Meeting in 2018, resolution 1",
            "resource-id": "https://www.bipm.org/en/committees/cg/cgpm/26-2018/resolution-1"
        },
        {
            "relation": "Definition in the International System of Units (SI), 9th Edition",
            "resource-id": "https://www.bipm.org/en/publications/si-brochure"
        },
        {
            "relation": "Wikipedia article describing the unit",
            "resource-id": "https://en.wikipedia.org/wiki/Candela"
        }
    ],
    "x-optimade-definition": {
        "kind": "unit",
        "format": "1.2",
        "version": "1.2.0",
        "name": "candela"
    }
}
```
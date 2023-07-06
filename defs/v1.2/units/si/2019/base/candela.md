# candela, cd (unit)

This page documents an [OPTIMADE](https://www.optimade.org/) [Unit Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/defs/v1.2/units/si/2019/base/candela`](https://schemas.optimade.org/defs/v1.2/units/si/2019/base/candela)**  
**Definition name:** `candela`

**Unit name:** candela  
**Latin symbol:** cd  
**Display symbol:** cd  
  
**Description:** The SI base unit of luminous intensity in a given direction defined by fixing the value of the luminous efficacy of radiation of a specific frequency precisely matching the definition at the 16th CGPM Meeting in 1979 using the 2019 SI units.

"The candela is the luminous intensity, in a given direction, of a source that emits monochromatic radiation of frequency 540×10¹² hertz and that has a radiant intensity in that direction of 1/683 watt per steradian." [16th CGPM Meeting (1979), resolution 3].

At the 26th CGPM Meeting in 2018, resolution 1 the definition was rephrased to: "The candela, symbol cd, is the SI unit of luminous intensity in a given direction. It is defined by taking the fixed numerical value of the luminous efficacy of monochromatic radiation of frequency 540×10¹² Hz, \(K_\mathrm{cd}\), to be 683 when expressed in the unit lm⋅W⁻¹, which is equal to cd⋅sr⋅W⁻¹, or cd⋅sr⋅kg⁻¹⋅m⁻²⋅s³, where the kilogram, metre and second are defined in terms of \(h\), \(c\) and \(\Delta \nu_\textrm{Cs}\)." [26th CGPM Meeting (2018), resolution 1].

Following the redefinition of the metre at the 17th CGPM Meeting in 1983, resolution 1, and the redefinition of the kilogram at the 26th CGPM Meeting (2018), resolution 1, the implicitly redefined candela references:

- the SI 1967 derived hertz unit (https://schemas.optimade.org/units/v1.2/si/1967/named/hertz) equal to second⁻¹, referencing the SI 1967 base unit second (https://schemas.optimade.org/units/v1.2/si/1967/base/second).
- the SI 2019 derived watt unit (https://schemas.optimade.org/units/v1.2/si/2019/named/watt) equal to kilogram·meter²·second⁻³, referencing the SI 2019 base unit kilogram (https://schemas.optimade.org/units/v1.2/si/2019/base/kilogram), the SI 1983 base unit metre (https://schemas.optimade.org/units/v1.2/si/1983/base/metre); and the 1967 base unit second (https://schemas.optimade.org/units/v1.2/si/1967/base/second).
- the SI 1960 supplementary unit steradian (https://schemas.optimade.org/units/v1.2/si/1960/supplementary/steradian).

**Resources:**

- [Definition in the 26th CGPM Meeting in 2018, resolution 1](https://www.bipm.org/en/committees/cg/cgpm/26-2018/resolution-1)
- [Definition in the International System of Units (SI), 9th Edition](https://www.bipm.org/en/publications/si-brochure)
- [Wikipedia article describing the unit](https://en.wikipedia.org/wiki/Candela)


**Formats:** [[JSON](candela.json)] [[MD](candela.md)]

**JSON definition:**

``` json
{
    "$schema": "https://schemas.optimade.org/meta/v1.2/optimade/physical_unit_definition.md",
    "$id": "https://schemas.optimade.org/defs/v1.2/units/si/2019/base/candela",
    "title": "candela",
    "symbol": "cd",
    "display-symbol": "cd",
    "description": "The SI base unit of luminous intensity in a given direction defined by fixing the value of the luminous efficacy of radiation of a specific frequency precisely matching the definition at the 16th CGPM Meeting in 1979 using the 2019 SI units.\n\n\"The candela is the luminous intensity, in a given direction, of a source that emits monochromatic radiation of frequency 540\u00d710\u00b9\u00b2 hertz and that has a radiant intensity in that direction of 1/683 watt per steradian.\" [16th CGPM Meeting (1979), resolution 3].\n\nAt the 26th CGPM Meeting in 2018, resolution 1 the definition was rephrased to: \"The candela, symbol cd, is the SI unit of luminous intensity in a given direction. It is defined by taking the fixed numerical value of the luminous efficacy of monochromatic radiation of frequency 540\u00d710\u00b9\u00b2 Hz, \\(K_\\mathrm{cd}\\), to be 683 when expressed in the unit lm\u22c5W\u207b\u00b9, which is equal to cd\u22c5sr\u22c5W\u207b\u00b9, or cd\u22c5sr\u22c5kg\u207b\u00b9\u22c5m\u207b\u00b2\u22c5s\u00b3, where the kilogram, metre and second are defined in terms of \\(h\\), \\(c\\) and \\(\\Delta \\nu_\\textrm{Cs}\\).\" [26th CGPM Meeting (2018), resolution 1].\n\nFollowing the redefinition of the metre at the 17th CGPM Meeting in 1983, resolution 1, and the redefinition of the kilogram at the 26th CGPM Meeting (2018), resolution 1, the implicitly redefined candela references:\n\n- the SI 1967 derived hertz unit (https://schemas.optimade.org/units/v1.2/si/1967/named/hertz) equal to second\u207b\u00b9, referencing the SI 1967 base unit second (https://schemas.optimade.org/units/v1.2/si/1967/base/second).\n- the SI 2019 derived watt unit (https://schemas.optimade.org/units/v1.2/si/2019/named/watt) equal to kilogram\u00b7meter\u00b2\u00b7second\u207b\u00b3, referencing the SI 2019 base unit kilogram (https://schemas.optimade.org/units/v1.2/si/2019/base/kilogram), the SI 1983 base unit metre (https://schemas.optimade.org/units/v1.2/si/1983/base/metre); and the 1967 base unit second (https://schemas.optimade.org/units/v1.2/si/1967/base/second).\n- the SI 1960 supplementary unit steradian (https://schemas.optimade.org/units/v1.2/si/1960/supplementary/steradian).",
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
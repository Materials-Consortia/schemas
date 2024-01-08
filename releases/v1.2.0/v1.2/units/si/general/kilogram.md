# kilogram, kg (unit)

This page documents an [OPTIMADE](https://www.optimade.org/) [Unit Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/defs/v1.2/units/si/general/kilogram`](https://schemas.optimade.org/defs/v1.2/units/si/general/kilogram.md)**  
**Definition name:** `kilogram`

**Unit name:** kilogram  
**Latin symbol:** kg  
**Display symbol:** kg  
  
**Description:** A unit of mass using the current, or one of the historical, definitions of the SI units.

The current definition at the 26th CGPM Meeting in 2018, resolution 1 is: "The kilogram, symbol kg, is the SI unit of mass. It is defined by taking the fixed numerical value of the Planck constant \(h\) to be 6.62607015×10⁻³⁴ when expressed in the unit J⋅s, which is equal to kg⋅m²⋅s⁻¹, where the metre and the second are defined in terms of \(c\) and \(\Delta \nu_\textrm{Cs}\)."

The prior definition at the 1st CGPM Meeting (1889) was: "The prototype of the kilogram adopted by the International Committee; This prototype will henceforth be considered as the unit of mass;", referring to the international prototype of the kilogram made of platinum-iridium.

This is a generalized definition taken to reference the current, or one of the historical, SI unit definitions.
This definition is intended for situations when it is not possible to be more precise, e.g., in contexts where data have been collected that uses different historical SI definitions.

**Resources:**

- [Definition in the 26th CGPM Meeting in 2018, resolution 1](https://www.bipm.org/en/committees/cg/cgpm/26-2018/resolution-1)
- [Definition in the International System of Units (SI), 9th Edition](https://www.bipm.org/en/publications/si-brochure)
- [Wikipedia article describing the unit](https://en.wikipedia.org/wiki/Kilogram)


**Formats:** [[JSON](kilogram.json)] [[MD](kilogram.md)]

**JSON definition:**

``` json
{
    "$schema": "https://schemas.optimade.org/meta/v1.2/optimade/physical_unit_definition.md",
    "$id": "https://schemas.optimade.org/defs/v1.2/units/si/general/kilogram",
    "title": "kilogram",
    "symbol": "kg",
    "display-symbol": "kg",
    "description": "A unit of mass using the current, or one of the historical, definitions of the SI units.\n\nThe current definition at the 26th CGPM Meeting in 2018, resolution 1 is: \"The kilogram, symbol kg, is the SI unit of mass. It is defined by taking the fixed numerical value of the Planck constant \\(h\\) to be 6.62607015\u00d710\u207b\u00b3\u2074 when expressed in the unit J\u22c5s, which is equal to kg\u22c5m\u00b2\u22c5s\u207b\u00b9, where the metre and the second are defined in terms of \\(c\\) and \\(\\Delta \\nu_\\textrm{Cs}\\).\"\n\nThe prior definition at the 1st CGPM Meeting (1889) was: \"The prototype of the kilogram adopted by the International Committee; This prototype will henceforth be considered as the unit of mass;\", referring to the international prototype of the kilogram made of platinum-iridium.\n\nThis is a generalized definition taken to reference the current, or one of the historical, SI unit definitions.\nThis definition is intended for situations when it is not possible to be more precise, e.g., in contexts where data have been collected that uses different historical SI definitions.",
    "compatibility": [
        "https://schemas.optimade.org/defs/v1.2/units/si/1960/base/kilogram",
        "https://schemas.optimade.org/defs/v1.2/units/si/2019/base/kilogram"
    ],
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
            "resource-id": "https://en.wikipedia.org/wiki/Kilogram"
        }
    ],
    "x-optimade-definition": {
        "label": "kilogram_si_general",
        "kind": "unit",
        "format": "1.2",
        "version": "1.2.0",
        "name": "kilogram"
    }
}
```
# ampere, A (unit)

This page documents an [OPTIMADE](https://www.optimade.org/) [Unit Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/defs/v1.2/units/si/general/ampere`](https://schemas.optimade.org/defs/v1.2/units/si/general/ampere.md)**  
**Definition name:** `ampere`

**Unit name:** ampere  
**Latin symbol:** A  
**Display symbol:** A  
  
**Description:** A unit of electric current defined according to the current, or one of the historical, definitions of the SI units.

The current definition at the 26th CGPM Meeting (2018), resolution 1 is: "The ampere, symbol A, is the SI unit of electric current. It is defined by taking the fixed numerical value of the elementary charge \(e\) to be 1.602176634×10⁻¹⁹ when expressed in the unit C, which is equal to A⋅s, where the second is defined in terms of \(\Delta \nu_\textrm{Cs}\)."

The earlier definition from the 41st CIPM meeting (1946), Resolution 2: "The ampere is that constant current which, if maintained in two straight parallel conductors of infinite length, of negligible circular cross-section, and placed 1 metre apart in vacuum, would produce between these conductors a force equal to 2×10⁻⁷ MKS unit of force per metre of length."

This is a generalized definition taken to reference the current, or one of the historical, SI unit definitions.
This definition is intended for situations when it is not possible to be more precise, e.g., in contexts where data have been collected that uses different historical SI definitions.

**Resources:**

- [Definition in the 26th CGPM Meeting in 2018, resolution 1](https://www.bipm.org/en/committees/cg/cgpm/26-2018/resolution-1)
- [Definition in the International System of Units (SI), 9th Edition](https://www.bipm.org/en/publications/si-brochure)
- [Wikipedia article describing the unit](https://en.wikipedia.org/wiki/Ampere)


**Formats:** [[JSON](ampere.json)] [[MD](ampere.md)]

**JSON definition:**

``` json
{
    "$schema": "https://schemas.optimade.org/meta/v1.2/optimade/physical_unit_definition.md",
    "$id": "https://schemas.optimade.org/defs/v1.2/units/si/general/ampere",
    "title": "ampere",
    "symbol": "A",
    "display-symbol": "A",
    "description": "A unit of electric current defined according to the current, or one of the historical, definitions of the SI units.\n\nThe current definition at the 26th CGPM Meeting (2018), resolution 1 is: \"The ampere, symbol A, is the SI unit of electric current. It is defined by taking the fixed numerical value of the elementary charge \\(e\\) to be 1.602176634\u00d710\u207b\u00b9\u2079 when expressed in the unit C, which is equal to A\u22c5s, where the second is defined in terms of \\(\\Delta \\nu_\\textrm{Cs}\\).\"\n\nThe earlier definition from the 41st CIPM meeting (1946), Resolution 2: \"The ampere is that constant current which, if maintained in two straight parallel conductors of infinite length, of negligible circular cross-section, and placed 1 metre apart in vacuum, would produce between these conductors a force equal to 2\u00d710\u207b\u2077 MKS unit of force per metre of length.\"\n\nThis is a generalized definition taken to reference the current, or one of the historical, SI unit definitions.\nThis definition is intended for situations when it is not possible to be more precise, e.g., in contexts where data have been collected that uses different historical SI definitions.",
    "compatibility": [
        "https://schemas.optimade.org/units/v1.2/si/1960/base/ampere",
        "https://schemas.optimade.org/units/v1.2/si/1967/base/ampere",
        "https://schemas.optimade.org/units/v1.2/si/1983/base/ampere",
        "https://schemas.optimade.org/units/v1.2/si/2019/base/ampere"
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
            "resource-id": "https://en.wikipedia.org/wiki/Ampere"
        }
    ],
    "x-optimade-definition": {
        "kind": "unit",
        "format": "1.2",
        "version": "1.2.0",
        "name": "ampere"
    }
}
```
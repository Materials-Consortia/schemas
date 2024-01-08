# second, s (unit)

This page documents an [OPTIMADE](https://www.optimade.org/) [Unit Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/defs/v1.2/units/si/1967/base/second`](https://schemas.optimade.org/defs/v1.2/units/si/1967/base/second.md)**  
**Definition name:** `second`

**Unit name:** second  
**Latin symbol:** s  
**Display symbol:** s  
  
**Description:** The SI base unit of time defined via the periods of transitions between levels in the caesium 133 atom after the redefinition at the 13th CGPM Meeting in 1967.

"The second is the duration of 9192631770 periods of the radiation corresponding to the transition between the two hyperfine levels of the ground state of the caesium 133 atom" [13th CGPM Meeting (1967), resolution 1]

At the 26th CGPM Meeting (2018), resolution 1 the definition was rephrased to: "The second, symbol s, is the SI unit of time. It is defined by taking the fixed numerical value of the caesium frequency, \(\Delta \nu_\textrm{Cs}\), the unperturbed ground-state hyperfine transition frequency of the caesium 133 atom, to be 9192631770 when expressed in the unit Hz, which is equal to s⁻¹."

**Resources:**

- [Definition in the 13th CGPM Meeting (1967), resolution 1](https://www.bipm.org/en/committees/cg/cgpm/13-1967/resolution-1)
- [Rephrased definition in the 26th CGPM Meeting (2018), resolution 1](https://www.bipm.org/en/committees/cg/cgpm/26-2018/resolution-1)
- [Wikipedia article describing the unit](https://en.wikipedia.org/wiki/Second)


**Formats:** [[JSON](second.json)] [[MD](second.md)]

**JSON definition:**

``` json
{
    "$schema": "https://schemas.optimade.org/meta/v1.2/optimade/physical_unit_definition.md",
    "$id": "https://schemas.optimade.org/defs/v1.2/units/si/1967/base/second",
    "title": "second",
    "symbol": "s",
    "display-symbol": "s",
    "description": "The SI base unit of time defined via the periods of transitions between levels in the caesium 133 atom after the redefinition at the 13th CGPM Meeting in 1967.\n\n\"The second is the duration of 9192631770 periods of the radiation corresponding to the transition between the two hyperfine levels of the ground state of the caesium 133 atom\" [13th CGPM Meeting (1967), resolution 1]\n\nAt the 26th CGPM Meeting (2018), resolution 1 the definition was rephrased to: \"The second, symbol s, is the SI unit of time. It is defined by taking the fixed numerical value of the caesium frequency, \\(\\Delta \\nu_\\textrm{Cs}\\), the unperturbed ground-state hyperfine transition frequency of the caesium 133 atom, to be 9192631770 when expressed in the unit Hz, which is equal to s\u207b\u00b9.\"",
    "resources": [
        {
            "relation": "Definition in the 13th CGPM Meeting (1967), resolution 1",
            "resource-id": "https://www.bipm.org/en/committees/cg/cgpm/13-1967/resolution-1"
        },
        {
            "relation": "Rephrased definition in the 26th CGPM Meeting (2018), resolution 1",
            "resource-id": "https://www.bipm.org/en/committees/cg/cgpm/26-2018/resolution-1"
        },
        {
            "relation": "Wikipedia article describing the unit",
            "resource-id": "https://en.wikipedia.org/wiki/Second"
        }
    ],
    "standard": {
        "name": "si",
        "year": 1967,
        "category": "base",
        "symbol": "s"
    },
    "x-optimade-definition": {
        "label": "second_si_1967_base",
        "kind": "unit",
        "format": "1.2",
        "version": "1.2.0",
        "name": "second"
    }
}
```
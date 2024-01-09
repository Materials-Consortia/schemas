# mole, mol (unit)

This page documents an [OPTIMADE](https://www.optimade.org/) [Unit Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/defs/v1.2/units/si/general/mole`](https://schemas.optimade.org/defs/v1.2/units/si/general/mole.md)**  
**Definition name:** `mole`

**Unit name:** mole  
**Latin symbol:** mol  
**Display symbol:** mol  
  
**Description:** A unit of amount of substance using the current, or one of the historical, definitions of the SI units.

The current definition at the 26th CGPM Meeting in 2018, resolution 1 is: "The mole, symbol mol, is the SI unit of amount of substance. One mole contains exactly 6.02214076×10²³ elementary entities. This number is the fixed numerical value of the Avogadro constant, \(N_A\), when expressed in the unit mol⁻¹ and is called the Avogadro number. The amount of substance, symbol \(n\), of a system is a measure of the number of specified elementary entities. An elementary entity may be an atom, a molecule, an ion, an electron, any other particle or specified group of particles."

The prior definition at the 14th CGPM Meeting (1971), resolution 3 was: "1. The mole is the amount of substance of a system which contains as many elementary entities as there are atoms in 0.012 kilogram of carbon 12. 2. When the mole is used, the elementary entities must be specified and may be atoms, molecules, ions, electrons, other particles, or specified groups of such particles." This definition was clarifed at the 69th CIPM meeting in 1980 by appending: "In this definition, it is understood that unbound atoms of carbon 12, at rest and in their ground state, are referred to."

This is a generalized definition taken to reference the current, or one of the historical, SI unit definitions.
This definition is intended for situations when it is not possible to be more precise, e.g., in contexts where data have been collected that uses different historical SI definitions.

**Resources:**

- [Definition in the 26th CGPM Meeting in 2018, resolution 1](https://www.bipm.org/en/committees/cg/cgpm/26-2018/resolution-1)
- [Definition in the 14th CGPM Meeting in 1971, resolution 3](https://www.bipm.org/en/committees/cg/cgpm/14-1971/resolution-3)
- [Clarification in the 96th meeting of the CIPM](https://www.bipm.org/en/committees/ci/cipm/69-1980)
- [Definition in the International System of Units (SI), 9th Edition](https://www.bipm.org/en/publications/si-brochure)
- [Wikipedia article describing the unit](https://en.wikipedia.org/wiki/Mole_(unit))


**Compatibility:** (other definitions that are covered by the above definition)

- [`https://schemas.optimade.org/defs/v1.2/units/si/1971/base/mole`](https://schemas.optimade.org/defs/v1.2/units/si/1971/base/mole.md)
- [`https://schemas.optimade.org/defs/v1.2/units/si/2019/base/mole`](https://schemas.optimade.org/defs/v1.2/units/si/2019/base/mole.md)


**Formats:** [[JSON](mole.json)] [[MD](mole.md)]

**JSON definition:**

``` json
{
    "$id": "https://schemas.optimade.org/defs/v1.2/units/si/general/mole",
    "$schema": "https://schemas.optimade.org/meta/v1.2/optimade/physical_unit_definition.json",
    "title": "mole",
    "symbol": "mol",
    "display-symbol": "mol",
    "description": "A unit of amount of substance using the current, or one of the historical, definitions of the SI units.\n\nThe current definition at the 26th CGPM Meeting in 2018, resolution 1 is: \"The mole, symbol mol, is the SI unit of amount of substance. One mole contains exactly 6.02214076\u00d710\u00b2\u00b3 elementary entities. This number is the fixed numerical value of the Avogadro constant, \\(N_A\\), when expressed in the unit mol\u207b\u00b9 and is called the Avogadro number. The amount of substance, symbol \\(n\\), of a system is a measure of the number of specified elementary entities. An elementary entity may be an atom, a molecule, an ion, an electron, any other particle or specified group of particles.\"\n\nThe prior definition at the 14th CGPM Meeting (1971), resolution 3 was: \"1. The mole is the amount of substance of a system which contains as many elementary entities as there are atoms in 0.012 kilogram of carbon 12. 2. When the mole is used, the elementary entities must be specified and may be atoms, molecules, ions, electrons, other particles, or specified groups of such particles.\" This definition was clarifed at the 69th CIPM meeting in 1980 by appending: \"In this definition, it is understood that unbound atoms of carbon 12, at rest and in their ground state, are referred to.\"\n\nThis is a generalized definition taken to reference the current, or one of the historical, SI unit definitions.\nThis definition is intended for situations when it is not possible to be more precise, e.g., in contexts where data have been collected that uses different historical SI definitions.",
    "compatibility": [
        "https://schemas.optimade.org/defs/v1.2/units/si/1971/base/mole",
        "https://schemas.optimade.org/defs/v1.2/units/si/2019/base/mole"
    ],
    "resources": [
        {
            "relation": "Definition in the 26th CGPM Meeting in 2018, resolution 1",
            "resource-id": "https://www.bipm.org/en/committees/cg/cgpm/26-2018/resolution-1"
        },
        {
            "relation": "Definition in the 14th CGPM Meeting in 1971, resolution 3",
            "resource-id": "https://www.bipm.org/en/committees/cg/cgpm/14-1971/resolution-3"
        },
        {
            "relation": "Clarification in the 96th meeting of the CIPM",
            "resource-id": "https://www.bipm.org/en/committees/ci/cipm/69-1980"
        },
        {
            "relation": "Definition in the International System of Units (SI), 9th Edition",
            "resource-id": "https://www.bipm.org/en/publications/si-brochure"
        },
        {
            "relation": "Wikipedia article describing the unit",
            "resource-id": "https://en.wikipedia.org/wiki/Mole_(unit)"
        }
    ],
    "x-optimade-definition": {
        "label": "mole_si_general",
        "kind": "unit",
        "format": "1.2",
        "version": "1.2.0",
        "name": "mole"
    }
}
```
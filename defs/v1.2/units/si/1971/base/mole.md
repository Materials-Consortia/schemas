# mole, mol (unit)

This page documents an [OPTIMADE](https://www.optimade.org/) [Unit Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/defs/v1.2/units/si/1971/base/mole`](https://schemas.optimade.org/defs/v1.2/units/si/1971/base/mole)**  
**Definition name:** `mole`

**Unit name:** mole  
**Latin symbol:** mol  
**Display symbol:** mol  
  
**Description:** The SI base unit of amount of substance defined via the number of atoms in 12 grams of carbon 12 at the 14th CGPM Meeting in 1971 and clarified at the 69th CIPM meeting in 1980.

"1. The mole is the amount of substance of a system which contains as many elementary entities as there are atoms in 0.012 kilogram of carbon 12. 2. When the mole is used, the elementary entities must be specified and may be atoms, molecules, ions, electrons, other particles, or specified groups of such particles." [14th CGPM Meeting (1971), resolution 3].

The 69th CIPM meeting in 1980 approved to append a clarification to the above definition: "In this definition, it is understood that unbound atoms of carbon 12, at rest and in their ground state, are referred to."

**Resources:**

- [Definition in the 14th CGPM Meeting in 1971, resolution 3](https://www.bipm.org/en/committees/cg/cgpm/14-1971/resolution-3)
- [Clarification in the 96th meeting of the CIPM](https://www.bipm.org/en/committees/ci/cipm/69-1980)
- [Wikipedia article describing the unit](https://en.wikipedia.org/wiki/Mole_(unit))


**Formats:** [[JSON](mole.json)] [[MD](mole.md)]

**JSON definition:**

``` json
{
    "$schema": "https://schemas.optimade.org/meta/v1.2/optimade/physical_unit_definition.md",
    "$id": "https://schemas.optimade.org/defs/v1.2/units/si/1971/base/mole",
    "title": "mole",
    "symbol": "mol",
    "display-symbol": "mol",
    "description": "The SI base unit of amount of substance defined via the number of atoms in 12 grams of carbon 12 at the 14th CGPM Meeting in 1971 and clarified at the 69th CIPM meeting in 1980.\n\n\"1. The mole is the amount of substance of a system which contains as many elementary entities as there are atoms in 0.012 kilogram of carbon 12. 2. When the mole is used, the elementary entities must be specified and may be atoms, molecules, ions, electrons, other particles, or specified groups of such particles.\" [14th CGPM Meeting (1971), resolution 3].\n\nThe 69th CIPM meeting in 1980 approved to append a clarification to the above definition: \"In this definition, it is understood that unbound atoms of carbon 12, at rest and in their ground state, are referred to.\"",
    "resources": [
        {
            "relation": "Definition in the 14th CGPM Meeting in 1971, resolution 3",
            "resource-id": "https://www.bipm.org/en/committees/cg/cgpm/14-1971/resolution-3"
        },
        {
            "relation": "Clarification in the 96th meeting of the CIPM",
            "resource-id": "https://www.bipm.org/en/committees/ci/cipm/69-1980"
        },
        {
            "relation": "Wikipedia article describing the unit",
            "resource-id": "https://en.wikipedia.org/wiki/Mole_(unit)"
        }
    ],
    "x-optimade-definition": {
        "kind": "unit",
        "format": "1.2",
        "version": "1.2.0",
        "name": "mole"
    }
}
```
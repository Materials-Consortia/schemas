# mole, mol (unit)

This page documents an [OPTIMADE](https://www.optimade.org/) [Unit Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/defs/v1.2/units/si/2019/base/mole`](https://schemas.optimade.org/defs/v1.2/units/si/2019/base/mole.md)**  
**Definition name:** `mole`

**Unit name:** mole  
**Latin symbol:** mol  
**Display symbol:** mol  
  
**Description:** The SI base unit of amount of substance defined by fixing the value of Avogadro constant as defined at the 26th CGPM Meeting (2018) and adopted into SI in 2019.

"The mole, symbol mol, is the SI unit of amount of substance. One mole contains exactly 6.02214076×10²³ elementary entities. This number is the fixed numerical value of the Avogadro constant, \(N_A\), when expressed in the unit mol⁻¹ and is called the Avogadro number. The amount of substance, symbol \(n\), of a system is a measure of the number of specified elementary entities. An elementary entity may be an atom, a molecule, an ion, an electron, any other particle or specified group of particles." [26th CGPM Meeting (2018), resolution 1].

**Resources:**

- [Definition in the 26th CGPM Meeting in 2018, resolution 1](https://www.bipm.org/en/committees/cg/cgpm/26-2018/resolution-1)
- [Definition in the International System of Units (SI), 9th Edition](https://www.bipm.org/en/publications/si-brochure)
- [Wikipedia article describing the unit](https://en.wikipedia.org/wiki/Mole_(unit))


**Formats:** [[JSON](mole.json)] [[MD](mole.md)]

**JSON definition:**

``` json
{
    "$schema": "https://schemas.optimade.org/meta/v1.2/optimade/physical_unit_definition.md",
    "$id": "https://schemas.optimade.org/defs/v1.2/units/si/2019/base/mole",
    "title": "mole",
    "symbol": "mol",
    "display-symbol": "mol",
    "description": "The SI base unit of amount of substance defined by fixing the value of Avogadro constant as defined at the 26th CGPM Meeting (2018) and adopted into SI in 2019.\n\n\"The mole, symbol mol, is the SI unit of amount of substance. One mole contains exactly 6.02214076\u00d710\u00b2\u00b3 elementary entities. This number is the fixed numerical value of the Avogadro constant, \\(N_A\\), when expressed in the unit mol\u207b\u00b9 and is called the Avogadro number. The amount of substance, symbol \\(n\\), of a system is a measure of the number of specified elementary entities. An elementary entity may be an atom, a molecule, an ion, an electron, any other particle or specified group of particles.\" [26th CGPM Meeting (2018), resolution 1].",
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
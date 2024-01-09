# Chemical symbol or vacancy (property)

This page documents an [OPTIMADE](https://www.optimade.org/) [Property Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/defs/v1.2/properties/optimade/common/chemical_symbol_or_vacancy`](https://schemas.optimade.org/defs/v1.2/properties/optimade/common/chemical_symbol_or_vacancy.md)**  
**Definition name:** `chemical_symbol_or_vacancy`

**Property name:** Chemical symbol or vacancy  
**Description:** A chemical symbol referring to an element, a non-chemical element, or a vacancy.  
**Type:** string  

**Requirements/Conventions:**

- Must be one of the following:

  - a valid chemical-element symbol, or
  - the special value `"X"` to represent a non-chemical element, or
  - the special value `"vacancy"` to represent that this site has a non-zero probability of having a vacancy.

**Examples:**

- `He`
- `X`
- `vacancy`

**Formats:** [[JSON](chemical_symbol_or_vacancy.json)] [[MD](chemical_symbol_or_vacancy.md)]

**JSON definition:**

``` json
{
    "$id": "https://schemas.optimade.org/defs/v1.2/properties/optimade/common/chemical_symbol_or_vacancy",
    "$schema": "https://schemas.optimade.org/meta/v1.2/optimade/property_definition.json",
    "title": "Chemical symbol or vacancy",
    "x-optimade-type": "string",
    "x-optimade-definition": {
        "label": "chemical_symbol_or_vacancy_optimade_common",
        "kind": "property",
        "version": "1.2.0",
        "format": "1.2",
        "name": "chemical_symbol_or_vacancy"
    },
    "description": "A chemical symbol referring to an element, a non-chemical element, or a vacancy.\n\n**Requirements/Conventions:**\n\n- Must be one of the following:\n\n  - a valid chemical-element symbol, or\n  - the special value `\"X\"` to represent a non-chemical element, or\n  - the special value `\"vacancy\"` to represent that this site has a non-zero probability of having a vacancy.",
    "x-optimade-unit": "inapplicable",
    "examples": [
        "He",
        "X",
        "vacancy"
    ],
    "type": [
        "string"
    ],
    "enum": [
        "X",
        "H",
        "He",
        "Li",
        "Be",
        "B",
        "C",
        "N",
        "O",
        "F",
        "Ne",
        "Na",
        "Mg",
        "Al",
        "Si",
        "P",
        "S",
        "Cl",
        "Ar",
        "K",
        "Ca",
        "Sc",
        "Ti",
        "V",
        "Cr",
        "Mn",
        "Fe",
        "Co",
        "Ni",
        "Cu",
        "Zn",
        "Ga",
        "Ge",
        "As",
        "Se",
        "Br",
        "Kr",
        "Rb",
        "Sr",
        "Y",
        "Zr",
        "Nb",
        "Mo",
        "Tc",
        "Ru",
        "Rh",
        "Pd",
        "Ag",
        "Cd",
        "In",
        "Sn",
        "Sb",
        "Te",
        "I",
        "Xe",
        "Cs",
        "Ba",
        "La",
        "Ce",
        "Pr",
        "Nd",
        "Pm",
        "Sm",
        "Eu",
        "Gd",
        "Tb",
        "Dy",
        "Ho",
        "Er",
        "Tm",
        "Yb",
        "Lu",
        "Hf",
        "Ta",
        "W",
        "Re",
        "Os",
        "Ir",
        "Pt",
        "Au",
        "Hg",
        "Tl",
        "Pb",
        "Bi",
        "Po",
        "At",
        "Rn",
        "Fr",
        "Ra",
        "Ac",
        "Th",
        "Pa",
        "U",
        "Np",
        "Pu",
        "Am",
        "Cm",
        "Bk",
        "Cf",
        "Es",
        "Fm",
        "Md",
        "No",
        "Lr",
        "Rf",
        "Db",
        "Sg",
        "Bh",
        "Hs",
        "Mt",
        "Ds",
        "Rg",
        "Cn",
        "Uut",
        "Uuq",
        "Uup",
        "Uuh",
        "Uus",
        "Uuo",
        "Nh",
        "Fl",
        "Mc",
        "Lv",
        "Ts",
        "Og"
    ]
}
```
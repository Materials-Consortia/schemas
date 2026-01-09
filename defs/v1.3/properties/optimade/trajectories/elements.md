# list of elements (property)

This page documents an [OPTIMADE](https://www.optimade.org/) [Property Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/defs/v1.3/properties/optimade/trajectories/elements`](https://schemas.optimade.org/defs/v1.3/properties/optimade/trajectories/elements.md)**  
**Definition name:** `elements`

**Property name:** list of elements  
**Description:** A list of elements items, where an elements item is a list of the chemical symbols of the different elements present in a structure.  
**Type:** list  

For each elements item the following applies:

**Requirements/Conventions**:

- The strings are the chemical symbols, i.e., either a single uppercase letter or an uppercase letter followed by a number of lowercase letters.
- The order MUST be alphabetical.
- MUST refer to the same elements in the same order, and therefore be of the same length, as `elements_ratios`, if the latter is provided.
- Note: This property SHOULD NOT contain the string "X" to indicate non-chemical elements or "vacancy" to indicate vacancies (in contrast to the field `chemical_symbols` for the species property).

**Examples:**

- `[["Al", "Si", "O"], ["Al", "Si", "O"], ["Al", "F"], ["Al", "Si", "O", "He"]]`
- `[["He"]]`

**Formats:** [[JSON](elements.json)] [[MD](elements.md)]

**JSON definition:**

``` json
{
    "$id": "https://schemas.optimade.org/defs/v1.3/properties/optimade/trajectories/elements",
    "$schema": "https://schemas.optimade.org/meta/v1.3/optimade/property_definition.json",
    "title": "list of elements",
    "x-optimade-type": "list",
    "x-optimade-definition": {
        "label": "elements_optimade_trajectories",
        "kind": "property",
        "version": "1.3.0",
        "format": "1.3",
        "name": "elements"
    },
    "x-optimade-dimensions": {
        "names": [
            "dim_frames",
            "dim_elements"
        ],
        "sizes": [
            null,
            null
        ],
        "compactable": [
            "constant",
            "no"
        ]
    },
    "type": [
        "array",
        "null"
    ],
    "description": "A list of elements items, where an elements item is a list of the chemical symbols of the different elements present in a structure.\n\nFor each elements item the following applies:\n\n**Requirements/Conventions**:\n\n- The strings are the chemical symbols, i.e., either a single uppercase letter or an uppercase letter followed by a number of lowercase letters.\n- The order MUST be alphabetical.\n- MUST refer to the same elements in the same order, and therefore be of the same length, as `elements_ratios`, if the latter is provided.\n- Note: This property SHOULD NOT contain the string \"X\" to indicate non-chemical elements or \"vacancy\" to indicate vacancies (in contrast to the field `chemical_symbols` for the species property).",
    "examples": [
        [
            [
                "Al",
                "Si",
                "O"
            ],
            [
                "Al",
                "Si",
                "O"
            ],
            [
                "Al",
                "F"
            ],
            [
                "Al",
                "Si",
                "O",
                "He"
            ]
        ],
        [
            [
                "He"
            ]
        ]
    ],
    "x-optimade-unit": "inapplicable",
    "items": {
        "$id": "https://schemas.optimade.org/defs/v1.2/properties/optimade/structures/elements",
        "title": "elements",
        "x-optimade-type": "list",
        "x-optimade-definition": {
            "label": "elements_optimade_structures",
            "kind": "property",
            "version": "1.2.1",
            "format": "1.2",
            "name": "elements"
        },
        "x-optimade-dimensions": {
            "names": [
                "dim_elements"
            ],
            "sizes": [
                null
            ]
        },
        "type": [
            "array",
            "null"
        ],
        "description": "The chemical symbols of the different elements present in the structure.\n\n**Requirements/Conventions**:\n\n- The strings are the chemical symbols, i.e., either a single uppercase letter or an uppercase letter followed by a number of lowercase letters.\n- The order MUST be alphabetical.\n- MUST refer to the same elements in the same order, and therefore be of the same length, as `elements_ratios`, if the latter is provided.\n- Note: This property SHOULD NOT contain the string \"X\" to indicate non-chemical elements or \"vacancy\" to indicate vacancies (in contrast to the field `chemical_symbols` for the species property).\n\n**Query examples**:\n\n- A filter that matches all records of structures that contain Si, Al **and** O, and possibly other elements: `elements HAS ALL \"Si\", \"Al\", \"O\"`.\n- To match structures with exactly these three elements, use `elements HAS ALL \"Si\", \"Al\", \"O\" AND elements LENGTH 3`.\n- Note: length queries on this property can be equivalently formulated by filtering on the `nelements` property directly.",
        "examples": [
            [
                "Al",
                "Si",
                "O"
            ],
            [
                "He"
            ]
        ],
        "x-optimade-unit": "inapplicable",
        "items": {
            "$id": "https://schemas.optimade.org/defs/v1.2/properties/optimade/common/element",
            "title": "element",
            "x-optimade-type": "string",
            "x-optimade-definition": {
                "label": "element_optimade_common",
                "kind": "property",
                "version": "1.2.0",
                "format": "1.2",
                "name": "element"
            },
            "description": "The chemical symbol of an element\n\n**Requirements/Conventions:**\n\n- The strings are the chemical symbols, i.e., either a single uppercase letter or an uppercase letter followed by a number of lowercase letters.",
            "x-optimade-unit": "inapplicable",
            "type": [
                "string"
            ],
            "maxLength": 3,
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
    }
}
```
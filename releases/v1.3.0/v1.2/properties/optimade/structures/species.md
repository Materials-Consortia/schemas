# species (property)

This page documents an [OPTIMADE](https://www.optimade.org/) [Property Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/defs/v1.2/properties/optimade/structures/species`](https://schemas.optimade.org/defs/v1.2/properties/optimade/structures/species.md)**  
**Definition name:** `species`

**Property name:** species  
**Description:** A list describing the species of the sites of this structure. Species can represent pure chemical elements, virtual-crystal atoms representing a statistical occupation of a given site by multiple chemical elements, and/or a location to which there are attached atoms, i.e., atoms whose precise location are unknown beyond that they are attached to that position (frequently used to indicate hydrogen atoms attached to another element, e.g., a carbon with three attached hydrogens might represent a methyl group, -CH3).  
**Type:** list  

**Requirements/Conventions**:

- Each list member MUST be a dictionary with the following keys:

    - **name**: REQUIRED; gives the name of the species; the **name** value MUST be unique in the `species` list;

    - **chemical\_symbols**: REQUIRED; MUST be a list of strings of all chemical elements composing this species. Each item of the list MUST be one of the following:

        - a valid chemical-element symbol, or
        - the special value `"X"` to represent a non-chemical element, or
        - the special value `"vacancy"` to represent that this site has a non-zero probability of having a vacancy (the respective probability is indicated in the `concentration` list, see below).

      If any one entry in the `species` list has a `chemical_symbols` list that is longer than 1 element, the correct flag MUST be set in the list `structure_features` (see property `structure_features`).

    - **concentration**: REQUIRED; MUST be a list of floats, with same length as `chemical_symbols`. The numbers represent the relative concentration of the corresponding chemical symbol in this species.
      The numbers SHOULD sum to one. Cases in which the numbers do not sum to one typically fall only in the following two categories:

        - Numerical errors when representing float numbers in fixed precision, e.g. for two chemical symbols with concentrations `1/3` and `2/3`, the concentration might look something like `[0.33333333333, 0.66666666666]`. If the client is aware that the sum is not one because of numerical precision, it can renormalize the values so that the sum is exactly one.
        - Experimental errors in the data present in the database. In this case, it is the responsibility of the client to decide how to process the data.

      Note that concentrations are uncorrelated between different sites (even of the same species).

    - **attached**: OPTIONAL; if provided MUST be a list of length 1 or more of strings of chemical symbols for the elements attached to this site, or "X" for a non-chemical element.
    - **nattached**: OPTIONAL; if provided MUST be a list of length 1 or more of integers indicating the number of attached atoms of the kind specified in the value of the `attached` key.

      The implementation MUST include either both or none of the `attached` and `nattached` keys, and if they are provided, they MUST be of the same length.
      Furthermore, if they are provided, the `structure_features` property MUST include the string `site_attachments`.

    - **mass**: OPTIONAL. If present MUST be a list of floats, with the same length as `chemical_symbols`, providing element masses expressed in a.m.u.
      Elements denoting vacancies MUST have masses equal to 0.
    - **original\_name**: OPTIONAL. Can be any valid Unicode string, and SHOULD contain (if specified) the name of the species that is used internally in the source database.

          **Note**: With regard to "source database", we refer to the immediate source being queried via the OPTIMADE API implementation.
          The main use of this field is for source databases that use species names, containing characters that are not allowed (see description of the list property `species_at_sites`).

- For systems that have only species formed by a single chemical symbol, and that have at most one species per chemical symbol, SHOULD use the chemical symbol as species name (e.g., `"Ti"` for titanium, `"O"` for oxygen, etc.)
  However, note that this is OPTIONAL, and client implementations MUST NOT assume that the key corresponds to a chemical symbol, nor assume that if the species name is a valid chemical symbol, that it represents a species with that chemical symbol.
  This means that a species `{"name": "C", "chemical_symbols": ["Ti"], "concentration": [1.0]}` is valid and represents a titanium species (and *not* a carbon species).
- It is NOT RECOMMENDED that a structure includes species that do not have at least one corresponding site.

**Explained examples**:

- `[ {"name": "Ti", "chemical_symbols": ["Ti"], "concentration": [1.0]} ]`: any site with this species is occupied by a Ti atom.
- `[ {"name": "Ti", "chemical_symbols": ["Ti", "vacancy"], "concentration": [0.9, 0.1]} ]`: any site with this species is occupied by a Ti atom with 90 % probability, and has a vacancy with 10 % probability.
- `[ {"name": "BaCa", "chemical_symbols": ["vacancy", "Ba", "Ca"], "concentration": [0.05, 0.45, 0.5], "mass": [0.0, 137.327, 40.078]} ]`: any site with this species is occupied by a Ba atom with 45 % probability, a Ca atom with 50 % probability, and by a vacancy with 5 % probability.
- `[ {"name": "C12", "chemical_symbols": ["C"], "concentration": [1.0], "mass": [12.0]} ]`: any site with this species is occupied by a carbon isotope with mass 12.
- `[ {"name": "C13", "chemical_symbols": ["C"], "concentration": [1.0], "mass": [13.0]} ]`: any site with this species is occupied by a carbon isotope with mass 13.
- `[ {"name": "CH3", "chemical_symbols": ["C"], "concentration": [1.0], "attached": ["H"], "nattached": [3]} ]`: any site with this species is occupied by a methyl group, -CH3, which is represented without specifying precise positions of the hydrogen atoms.

**Examples:**

- `[{"name": "Ti", "chemical_symbols": ["Ti"], "concentration": [1.0]}]`
- `[{"name": "Ti", "chemical_symbols": ["Ti", "vacancy"], "concentration": [0.9, 0.1]}]`
- `[{"name": "BaCa", "chemical_symbols": ["vacancy", "Ba", "Ca"], "concentration": [0.05, 0.45, 0.5], "mass": [0.0, 137.327, 40.078]}]`
- `[{"name": "C12", "chemical_symbols": ["C"], "concentration": [1.0], "mass": [12.0]}]`
- `[{"name": "C13", "chemical_symbols": ["C"], "concentration": [1.0], "mass": [13.0]}]`
- `[{"name": "CH3", "chemical_symbols": ["C"], "concentration": [1.0], "attached": ["H"], "nattached": [3]}]`

**Formats:** [[JSON](species.json)] [[MD](species.md)]

**JSON definition:**

``` json
{
    "$id": "https://schemas.optimade.org/defs/v1.2/properties/optimade/structures/species",
    "$schema": "https://schemas.optimade.org/meta/v1.2/optimade/property_definition.json",
    "title": "species",
    "x-optimade-type": "list",
    "x-optimade-definition": {
        "label": "species_optimade_structures",
        "kind": "property",
        "version": "1.2.1",
        "format": "1.2",
        "name": "species"
    },
    "x-optimade-dimensions": {
        "names": [
            "dim_species"
        ],
        "sizes": [
            null
        ]
    },
    "x-optimade-unit-definitions": [
        {
            "$id": "https://schemas.optimade.org/defs/v1.2/units/si/general/atomicmassunit",
            "title": "atomic mass unit",
            "symbol": "u",
            "display-symbol": "u",
            "alternate-symbols": [
                "dalton",
                "Da"
            ],
            "description": "A unit of mass representing 1/12 of the mass of a free carbon 12 atom (i.e., a typical value of the mass of a nucleon in an atom) using the current, or one of the historical, definitions given in the editions of the International System of Units (SI).\n\nThe International System of Units (SI), 1st ed. (1970) defines the atomic mass unit in the section \"Units used with the International System\" (known as \"Non-SI units accepted for use with the SI units\" in later editions).\nThe unit is defined in a footnote as: \"The atomic mass unit (unified) is equal to 1/12 of the mass of an atom of the nuclide \u00b9\u00b2C; 1 u = 1.66053 x 10\u207b\u00b2\u2077 kg approximately.\"\n\nThe definition is retained in the International System of Units up to the 7th edition (1998), where the conditions are slightly clarified and dalton (Da) is introduced as an alternative name: \"The unified atomic mass unit is equal to 1/12 of the mass of an unbound atom of the nuclide \u00b9\u00b2C, at rest, and in its ground state. In the field of biochemistry, the unified atomic mass unit is also called the dalton, symbol Da.\"\nIn the 8th ed. (2006) the definition is slightly adjusted, replacing \"unbound\" with \"free\": \"The dalton (Da) and the unified atomic mass unit (u) are alternative names (and symbols) for the same unit, equal to 1/12 times the mass of a free carbon 12 atom, at rest and in its ground state.\"\n\nAll editions of the International System of Units note approximate relationships to the kilogram.\nThe 9th ed. states \"1 Da = 1.660 539 066 60(50)\u00d710\u207b\u00b2\u2077 kg\", where the 2018 CODATA value has been used and the 2019 SI kilogram is referenced (https://schemas.optimade.org/defs/v1.2/units/si/2019/base/kilogram).\n\nIn the 2019 redefinition of the SI units, the atomic mass unit is the only unit listed as accepted for use with SI that has a value in SI units which is determined experimentally.\n\nThis is a generalized definition taken to reference the current, or one of the historical, SI unit definitions.\nThis definition is intended for situations when it is not possible to be more precise, e.g., in contexts where data have been collected that uses different historical SI definitions.",
            "compatibility": [
                "https://schemas.optimade.org/defs/v1.2/units/si/1970/accepted/atomicmassunit",
                "https://schemas.optimade.org/defs/v1.2/units/si/1998/accepted/dalton",
                "https://schemas.optimade.org/defs/v1.2/units/si/general/dalton"
            ],
            "resources": [
                {
                    "relation": "Definition in the International System of Units (SI), 9th Edition",
                    "resource-id": "https://www.bipm.org/en/publications/si-brochure"
                },
                {
                    "relation": "Wikipedia article describing the unit",
                    "resource-id": "https://en.wikipedia.org/wiki/Dalton_(unit)"
                },
                {
                    "relation": "CODATA unified atomic mass unit fundamental physical constant: source for relationship to kg",
                    "resource-id": "https://physics.nist.gov/cgi-bin/cuu/Value?ukg"
                }
            ],
            "approximate-relations": [
                {
                    "base-units": [
                        {
                            "symbol": "kg",
                            "id": "https://schemas.optimade.org/defs/v1.2/units/si/general/kilogram"
                        }
                    ],
                    "base-units-expression": "kg",
                    "scale": {
                        "value": 1.6605390666e-27,
                        "standard_uncertainty": 5e-37
                    }
                }
            ],
            "x-optimade-definition": {
                "label": "atomicmassunit_si_general",
                "kind": "unit",
                "format": "1.2",
                "version": "1.2.0",
                "name": "atomicmassunit"
            }
        }
    ],
    "type": [
        "array",
        "null"
    ],
    "description": "A list describing the species of the sites of this structure. Species can represent pure chemical elements, virtual-crystal atoms representing a statistical occupation of a given site by multiple chemical elements, and/or a location to which there are attached atoms, i.e., atoms whose precise location are unknown beyond that they are attached to that position (frequently used to indicate hydrogen atoms attached to another element, e.g., a carbon with three attached hydrogens might represent a methyl group, -CH3).\n\n**Requirements/Conventions**:\n\n- Each list member MUST be a dictionary with the following keys:\n\n    - **name**: REQUIRED; gives the name of the species; the **name** value MUST be unique in the `species` list;\n\n    - **chemical\\_symbols**: REQUIRED; MUST be a list of strings of all chemical elements composing this species. Each item of the list MUST be one of the following:\n\n        - a valid chemical-element symbol, or\n        - the special value `\"X\"` to represent a non-chemical element, or\n        - the special value `\"vacancy\"` to represent that this site has a non-zero probability of having a vacancy (the respective probability is indicated in the `concentration` list, see below).\n\n      If any one entry in the `species` list has a `chemical_symbols` list that is longer than 1 element, the correct flag MUST be set in the list `structure_features` (see property `structure_features`).\n\n    - **concentration**: REQUIRED; MUST be a list of floats, with same length as `chemical_symbols`. The numbers represent the relative concentration of the corresponding chemical symbol in this species.\n      The numbers SHOULD sum to one. Cases in which the numbers do not sum to one typically fall only in the following two categories:\n\n        - Numerical errors when representing float numbers in fixed precision, e.g. for two chemical symbols with concentrations `1/3` and `2/3`, the concentration might look something like `[0.33333333333, 0.66666666666]`. If the client is aware that the sum is not one because of numerical precision, it can renormalize the values so that the sum is exactly one.\n        - Experimental errors in the data present in the database. In this case, it is the responsibility of the client to decide how to process the data.\n\n      Note that concentrations are uncorrelated between different sites (even of the same species).\n\n    - **attached**: OPTIONAL; if provided MUST be a list of length 1 or more of strings of chemical symbols for the elements attached to this site, or \"X\" for a non-chemical element.\n    - **nattached**: OPTIONAL; if provided MUST be a list of length 1 or more of integers indicating the number of attached atoms of the kind specified in the value of the `attached` key.\n\n      The implementation MUST include either both or none of the `attached` and `nattached` keys, and if they are provided, they MUST be of the same length.\n      Furthermore, if they are provided, the `structure_features` property MUST include the string `site_attachments`.\n\n    - **mass**: OPTIONAL. If present MUST be a list of floats, with the same length as `chemical_symbols`, providing element masses expressed in a.m.u.\n      Elements denoting vacancies MUST have masses equal to 0.\n    - **original\\_name**: OPTIONAL. Can be any valid Unicode string, and SHOULD contain (if specified) the name of the species that is used internally in the source database.\n\n          **Note**: With regard to \"source database\", we refer to the immediate source being queried via the OPTIMADE API implementation.\n          The main use of this field is for source databases that use species names, containing characters that are not allowed (see description of the list property `species_at_sites`).\n\n- For systems that have only species formed by a single chemical symbol, and that have at most one species per chemical symbol, SHOULD use the chemical symbol as species name (e.g., `\"Ti\"` for titanium, `\"O\"` for oxygen, etc.)\n  However, note that this is OPTIONAL, and client implementations MUST NOT assume that the key corresponds to a chemical symbol, nor assume that if the species name is a valid chemical symbol, that it represents a species with that chemical symbol.\n  This means that a species `{\"name\": \"C\", \"chemical_symbols\": [\"Ti\"], \"concentration\": [1.0]}` is valid and represents a titanium species (and *not* a carbon species).\n- It is NOT RECOMMENDED that a structure includes species that do not have at least one corresponding site.\n\n**Explained examples**:\n\n- `[ {\"name\": \"Ti\", \"chemical_symbols\": [\"Ti\"], \"concentration\": [1.0]} ]`: any site with this species is occupied by a Ti atom.\n- `[ {\"name\": \"Ti\", \"chemical_symbols\": [\"Ti\", \"vacancy\"], \"concentration\": [0.9, 0.1]} ]`: any site with this species is occupied by a Ti atom with 90 % probability, and has a vacancy with 10 % probability.\n- `[ {\"name\": \"BaCa\", \"chemical_symbols\": [\"vacancy\", \"Ba\", \"Ca\"], \"concentration\": [0.05, 0.45, 0.5], \"mass\": [0.0, 137.327, 40.078]} ]`: any site with this species is occupied by a Ba atom with 45 % probability, a Ca atom with 50 % probability, and by a vacancy with 5 % probability.\n- `[ {\"name\": \"C12\", \"chemical_symbols\": [\"C\"], \"concentration\": [1.0], \"mass\": [12.0]} ]`: any site with this species is occupied by a carbon isotope with mass 12.\n- `[ {\"name\": \"C13\", \"chemical_symbols\": [\"C\"], \"concentration\": [1.0], \"mass\": [13.0]} ]`: any site with this species is occupied by a carbon isotope with mass 13.\n- `[ {\"name\": \"CH3\", \"chemical_symbols\": [\"C\"], \"concentration\": [1.0], \"attached\": [\"H\"], \"nattached\": [3]} ]`: any site with this species is occupied by a methyl group, -CH3, which is represented without specifying precise positions of the hydrogen atoms.",
    "examples": [
        [
            {
                "name": "Ti",
                "chemical_symbols": [
                    "Ti"
                ],
                "concentration": [
                    1.0
                ]
            }
        ],
        [
            {
                "name": "Ti",
                "chemical_symbols": [
                    "Ti",
                    "vacancy"
                ],
                "concentration": [
                    0.9,
                    0.1
                ]
            }
        ],
        [
            {
                "name": "BaCa",
                "chemical_symbols": [
                    "vacancy",
                    "Ba",
                    "Ca"
                ],
                "concentration": [
                    0.05,
                    0.45,
                    0.5
                ],
                "mass": [
                    0.0,
                    137.327,
                    40.078
                ]
            }
        ],
        [
            {
                "name": "C12",
                "chemical_symbols": [
                    "C"
                ],
                "concentration": [
                    1.0
                ],
                "mass": [
                    12.0
                ]
            }
        ],
        [
            {
                "name": "C13",
                "chemical_symbols": [
                    "C"
                ],
                "concentration": [
                    1.0
                ],
                "mass": [
                    13.0
                ]
            }
        ],
        [
            {
                "name": "CH3",
                "chemical_symbols": [
                    "C"
                ],
                "concentration": [
                    1.0
                ],
                "attached": [
                    "H"
                ],
                "nattached": [
                    3
                ]
            }
        ]
    ],
    "x-optimade-unit": "inapplicable",
    "items": {
        "title": "species declaration",
        "x-optimade-type": "dictionary",
        "description": "A declaration of a species of the sites of this structure. Species can represent pure chemical elements, virtual-crystal atoms representing a statistical occupation of a given site by multiple chemical elements, and/or a location to which there are attached atoms, i.e., atoms whose precise location are unknown beyond that they are attached to that position (frequently used to indicate hydrogen atoms attached to another element, e.g., a carbon with three attached hydrogens might represent a methyl group, -CH3).",
        "x-optimade-unit": "inapplicable",
        "type": [
            "object"
        ],
        "properties": {
            "name": {
                "$id": "https://schemas.optimade.org/defs/v1.2/properties/optimade/common/species_name",
                "title": "name of the species",
                "x-optimade-type": "string",
                "x-optimade-definition": {
                    "label": "species_name_optimade_common",
                    "kind": "property",
                    "version": "1.2.0",
                    "format": "1.2",
                    "name": "species_name"
                },
                "type": [
                    "string"
                ],
                "description": "The name of the species.",
                "examples": [
                    "Na",
                    "Si[32982]",
                    "quop"
                ],
                "x-optimade-unit": "inapplicable"
            },
            "chemical_symbols": {
                "title": "chemical symbols",
                "x-optimade-type": "list",
                "x-optimade-dimensions": {
                    "names": [
                        "dim_species_chemical_symbols"
                    ],
                    "sizes": [
                        null
                    ]
                },
                "type": [
                    "array"
                ],
                "description": "The chemical symbols for the elements composing this species.\n\n**Requirements/Conventions**:\n\n- MUST be a list of strings of all chemical elements composing this species.\n  Each item of the list MUST be one of the following:\n\n    - a valid chemical-element symbol, or\n    - the special value `\"X\"` to represent a non-chemical element, or\n    - the special value `\"vacancy\"` to represent that this site has a non-zero probability of having a vacancy (the respective probability is indicated in the `concentration` list, see below).\n\nIf any one entry in the `species` list has a `chemical_symbols` list that is longer than 1 element, the correct flag MUST be set in the list `structure_features` (see property `structure_features`).",
                "examples": [
                    [
                        "Na",
                        "Cl"
                    ],
                    [
                        "Si",
                        "Mn",
                        "X",
                        "vacancy"
                    ]
                ],
                "x-optimade-unit": "inapplicable",
                "items": {
                    "$id": "https://schemas.optimade.org/defs/v1.2/properties/optimade/common/chemical_symbol_or_vacancy",
                    "title": "chemical symbol or vacancy",
                    "x-optimade-type": "string",
                    "x-optimade-definition": {
                        "label": "chemical_symbol_or_vacancy_optimade_common",
                        "kind": "property",
                        "version": "1.2.0",
                        "format": "1.2",
                        "name": "chemical_symbol_or_vacancy"
                    },
                    "description": "A chemical symbol referring to an element, a non-chemical element, or a vacancy.\n\n**Requirements/Conventions:**\n\n- Must be one of the following:\n\n    - a valid chemical-element symbol, or\n    - the special value `\"X\"` to represent a non-chemical element, or\n    - the special value `\"vacancy\"` to represent that this site has a non-zero probability of having a vacancy.",
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
            },
            "concentration": {
                "title": "concentration",
                "x-optimade-type": "list",
                "x-optimade-dimensions": {
                    "names": [
                        "dim_species_chemical_symbols"
                    ],
                    "sizes": [
                        null
                    ]
                },
                "type": [
                    "array"
                ],
                "description": "A list of the relative concentrations of the elements composing this species.\n\n**Requirements/Conventions**:\n\n- MUST be a list of floats, with same length as `chemical_symbols`. The numbers represent the relative concentration of the corresponding chemical symbol in this species.\n- The numbers SHOULD sum to one. Cases in which the numbers do not sum to one typically fall only in the following two categories:\n\n    - Numerical errors when representing float numbers in fixed precision, e.g. for two chemical symbols with concentrations `1/3` and `2/3`, the concentration might look something like `[0.33333333333, 0.66666666666]`. If the client is aware that the sum is not one because of numerical precision, it can renormalize the values so that the sum is exactly one.\n    - Experimental errors in the data present in the database. In this case, it is the responsibility of the client to decide how to process the data.\n\nNote that concentrations are uncorrelated between different sites (even of the same species).",
                "examples": [
                    [
                        1.0
                    ],
                    [
                        0.3333333333333333,
                        0.2222222222222222,
                        0.4444444444444444
                    ]
                ],
                "x-optimade-unit": "inapplicable",
                "items": {
                    "x-optimade-type": "float",
                    "type": [
                        "number"
                    ],
                    "x-optimade-unit": "dimensionless",
                    "minimum": 0.0,
                    "maximum": 1.0
                }
            },
            "attached": {
                "title": "attached chemical symbols",
                "x-optimade-type": "list",
                "x-optimade-dimensions": {
                    "names": [
                        "dim_species_attached"
                    ],
                    "sizes": [
                        null
                    ]
                },
                "type": [
                    "array"
                ],
                "description": "The chemical symbols of the elements or non-chemical elements attached to a site that has been assinged this species.\n\n**Requirements/Conventions**:\n\n- MUST be a list of strings of all chemical elements composing this species.\n  Each item of the list MUST be one of the following:\n\n    - a valid chemical-element symbol.\n    - the special value `\"X\"` to represent a non-chemical element.\n\nIf any one entry in the `species` list has a `attached` list that is longer than 1 element, the correct flag MUST be set in the list `structure_features` (see property `structure_features`).",
                "examples": [
                    [
                        "Na",
                        "Cl"
                    ],
                    [
                        "Si",
                        "Mn",
                        "X"
                    ]
                ],
                "x-optimade-unit": "inapplicable",
                "items": {
                    "$id": "https://schemas.optimade.org/defs/v1.2/properties/optimade/common/chemical_symbol",
                    "title": "chemical symbol",
                    "x-optimade-type": "string",
                    "x-optimade-definition": {
                        "label": "chemical_symbol_optimade_common",
                        "kind": "property",
                        "version": "1.2.0",
                        "format": "1.2",
                        "name": "chemical_symbol"
                    },
                    "description": "A chemical symbol referring to an element or a non-chemical element.\n\n**Requirements/Conventions:**\n\n- Must be one of the following:\n\n    - a valid chemical-element symbol, or\n    - the special value `\"X\"` to represent a non-chemical element.",
                    "x-optimade-unit": "inapplicable",
                    "examples": [
                        "He",
                        "X"
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
            },
            "nattached": {
                "title": "number of attached entities",
                "x-optimade-type": "list",
                "x-optimade-dimensions": {
                    "names": [
                        "dim_species_attached"
                    ],
                    "sizes": [
                        null
                    ]
                },
                "type": [
                    "array"
                ],
                "description": "MUST be a list of length 1 or more of integers indicating the number of attached atoms of the kind specified in the value of the `attached` key.\n\n**Requirements/Conventions**:\n\n- The implementation MUST include either both or none of the `attached` and `nattached` keys, and if they are provided, they MUST be of the same length.\n  Furthermore, if they are provided, the `structure_features` property MUST include the string `site_attachments`.",
                "examples": [
                    [
                        1,
                        2,
                        5,
                        7
                    ]
                ],
                "x-optimade-unit": "inapplicable",
                "items": {
                    "x-optimade-type": "integer",
                    "type": [
                        "integer"
                    ],
                    "x-optimade-unit": "dimensionless",
                    "minimum": 0
                }
            },
            "mass": {
                "title": "masses of the entities composing the species",
                "x-optimade-type": "list",
                "x-optimade-dimensions": {
                    "names": [
                        "dim_species_chemical_symbols"
                    ],
                    "sizes": [
                        null
                    ]
                },
                "type": [
                    "array"
                ],
                "description": "MUST be a list of floats, with the same length as `chemical_symbols`, providing element masses expressed in a.m.u.\n\n**Requirements/Conventions**:\n\n- Elements denoting vacancies MUST have masses equal to 0.",
                "examples": [
                    [
                        58.933195,
                        28.0855
                    ]
                ],
                "x-optimade-unit": "inapplicable",
                "items": {
                    "x-optimade-type": "float",
                    "type": [
                        "number"
                    ],
                    "x-optimade-unit": "dalton",
                    "minimum": 0.0
                }
            },
            "original_name": {
                "title": "original name",
                "x-optimade-type": "string",
                "type": [
                    "string"
                ],
                "description": "A name for the species that derives from the source database.\n\n**Requirements/Conventions**:\n\n- Can be any valid Unicode string, and SHOULD contain (if specified) the name of the species that is used internally in the source database.\n\n  **Note**: With regard to \"source database\", we refer to the immediate source being queried via the OPTIMADE API implementation.\n  The main use of this field is for source databases that use species names, containing characters that are not allowed (see description of the list property `species_at_sites`).",
                "examples": [
                    "Na[49385]"
                ],
                "x-optimade-unit": "inapplicable"
            }
        },
        "required": [
            "name",
            "chemical_symbols",
            "concentration"
        ]
    }
}
```
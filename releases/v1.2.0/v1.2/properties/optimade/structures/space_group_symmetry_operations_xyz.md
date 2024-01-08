# Space group symmetry operations (property)

This page documents an [OPTIMADE](https://www.optimade.org/) [Property Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/defs/v1.2/properties/optimade/structures/space_group_symmetry_operations_xyz`](https://schemas.optimade.org/defs/v1.2/properties/optimade/structures/space_group_symmetry_operations_xyz.md)**  
**Definition name:** `space_group_symmetry_operations_xyz`

**Property name:** Space group symmetry operations  
**Description:** A list of symmetry operations given as general position x, y and z coordinates in algebraic form.  
**Type:** list  

**Requirements/Conventions**:

- MUST be `null` if the property `nperiodic_dimensions` is equal to 0.
- Each symmetry operation is described by a string that gives that symmetry operation in Jones' faithful representation (Bradley & Cracknell, 1972: pp. 35-37), adapted for computer string notation.
- The letters `x`, `y` and `z` that are typesetted with overbars in printed text represent coordinate values multiplied by -1 and are encoded as `-x`, `-y` and `-z`, respectively.
- The syntax of the strings representing symmetry operations MUST conform to regular expressions given in OPTIMADE specification appendix The Symmetry Operation String Regular Expressions.
- The interpretation of the strings MUST follow the conventions of the IUCr CIF core dictionary (IUCr, 2023).
- In particular, this property MUST explicitly provide all symmetry operations needed to generate all the atoms in the unit cell from the atoms in the asymmetric unit, for the setting used.
- This symmetry operation set MUST always include the `x,y,z` identity operation.
- The symmetry operations are to be applied to fractional atom coordinates.
- In case only Cartesian coordinates are available, these Cartesian coordinates must be converted to fractional coordinates before the application of the provided symmetry operations.
- If the symmetry operation list is present, it MUST be compatible with other space group specifications (e.g. the ITC space group number, the Hall symbol, the Hermann-Mauguin symbol) if these are present.

**Notes**:

- The list of space group symmetry operations applies to the whole periodic array of atoms and together with the lattice translations given in the :property:`lattice\_vectors` property provides the necessary information to reconstruct all atom site positions of the periodic material.
- Thus, the symmetry operations described in this property are only applicable to material models with at least one periodic dimension.
- This property is not meant to represent arbitrary symmetries of molecules, non-periodic (finite) collections of atoms or non-crystallographic symmetry.

**Explained examples**:

- Space group operations for the space group with ITC number 3 (H-M symbol `P 2`, extended H-M symbol `P 1 2 1`, Hall symbol `P 2y`): `["x,y,z", "-x,y,-z"]`
- Space group operations for the space group with ITC number 5 (H-M symbol `C 2`, extended H-M symbol `C 1 2 1`, Hall symbol `C 2y`): `["x,y,z", "-x,y,-z", "x+1/2,y+1/2,z", "-x+1/2,y+1/2,-z"]`

**Bibliographic References**

- Bradley, C. J. and Cracknell, A. P. (1972) The Mathematical Theory of Symmetry in Solids. Oxford, Clarendon Press (paperback edition 2010) 745 p. ISBN `978-0-19-958258-7 <https://isbnsearch.org/isbn/9780199582587>`__.
- IUCr (2023) Core dictionary (coreCIF) version 2.4.5; data name `\_space\_group\_symop\_operation\_xyz`. Available from: https://www.iucr.org/__data/iucr/cifdic_html/1/cif_core.dic/Ispace_group_symop_operation_xyz.html [Accessed 2023-06-18T16:46+03:00].

**Examples:**

- `['x,y,z', '-x,y,-z']`
- `['x,y,z', '-x,y,-z', 'x+1/2,y+1/2,z', '-x+1/2,y+1/2,-z']`

**Formats:** [[JSON](space_group_symmetry_operations_xyz.json)] [[MD](space_group_symmetry_operations_xyz.md)]

**JSON definition:**

``` json
{
    "$schema": "https://schemas.optimade.org/meta/v1.2/optimade/property_definition.md",
    "$id": "https://schemas.optimade.org/defs/v1.2/properties/optimade/structures/space_group_symmetry_operations_xyz",
    "title": "Space group symmetry operations",
    "x-optimade-type": "list",
    "x-optimade-definition": {
        "label": "space_group_symmetry_operations_xyz_optimade_structures",
        "kind": "property",
        "version": "1.2.0",
        "format": "1.2",
        "name": "space_group_symmetry_operations_xyz"
    },
    "type": [
        "array",
        "null"
    ],
    "description": "A list of symmetry operations given as general position x, y and z coordinates in algebraic form.\n\n**Requirements/Conventions**:\n\n- MUST be `null` if the property `nperiodic_dimensions` is equal to 0.\n- Each symmetry operation is described by a string that gives that symmetry operation in Jones' faithful representation (Bradley & Cracknell, 1972: pp. 35-37), adapted for computer string notation.\n- The letters `x`, `y` and `z` that are typesetted with overbars in printed text represent coordinate values multiplied by -1 and are encoded as `-x`, `-y` and `-z`, respectively.\n- The syntax of the strings representing symmetry operations MUST conform to regular expressions given in OPTIMADE specification appendix The Symmetry Operation String Regular Expressions.\n- The interpretation of the strings MUST follow the conventions of the IUCr CIF core dictionary (IUCr, 2023).\n- In particular, this property MUST explicitly provide all symmetry operations needed to generate all the atoms in the unit cell from the atoms in the asymmetric unit, for the setting used.\n- This symmetry operation set MUST always include the `x,y,z` identity operation.\n- The symmetry operations are to be applied to fractional atom coordinates.\n- In case only Cartesian coordinates are available, these Cartesian coordinates must be converted to fractional coordinates before the application of the provided symmetry operations.\n- If the symmetry operation list is present, it MUST be compatible with other space group specifications (e.g. the ITC space group number, the Hall symbol, the Hermann-Mauguin symbol) if these are present.\n\n**Notes**:\n\n- The list of space group symmetry operations applies to the whole periodic array of atoms and together with the lattice translations given in the :property:`lattice\\_vectors` property provides the necessary information to reconstruct all atom site positions of the periodic material.\n- Thus, the symmetry operations described in this property are only applicable to material models with at least one periodic dimension.\n- This property is not meant to represent arbitrary symmetries of molecules, non-periodic (finite) collections of atoms or non-crystallographic symmetry.\n\n**Explained examples**:\n\n- Space group operations for the space group with ITC number 3 (H-M symbol `P 2`, extended H-M symbol `P 1 2 1`, Hall symbol `P 2y`): `[\"x,y,z\", \"-x,y,-z\"]`\n- Space group operations for the space group with ITC number 5 (H-M symbol `C 2`, extended H-M symbol `C 1 2 1`, Hall symbol `C 2y`): `[\"x,y,z\", \"-x,y,-z\", \"x+1/2,y+1/2,z\", \"-x+1/2,y+1/2,-z\"]`\n\n**Bibliographic References**\n\n- Bradley, C. J. and Cracknell, A. P. (1972) The Mathematical Theory of Symmetry in Solids. Oxford, Clarendon Press (paperback edition 2010) 745 p. ISBN `978-0-19-958258-7 <https://isbnsearch.org/isbn/9780199582587>`__.\n- IUCr (2023) Core dictionary (coreCIF) version 2.4.5; data name `\\_space\\_group\\_symop\\_operation\\_xyz`. Available from: https://www.iucr.org/__data/iucr/cifdic_html/1/cif_core.dic/Ispace_group_symop_operation_xyz.html [Accessed 2023-06-18T16:46+03:00].",
    "examples": [
        [
            "x,y,z",
            "-x,y,-z"
        ],
        [
            "x,y,z",
            "-x,y,-z",
            "x+1/2,y+1/2,z",
            "-x+1/2,y+1/2,-z"
        ]
    ],
    "x-optimade-unit": "unapplicable",
    "items": {
        "$id": "https://schemas.optimade.org/defs/v1.2/properties/optimade/common/space_group_symmetry_operation_xyz",
        "title": "Space group symmetry operation",
        "x-optimade-type": "string",
        "x-optimade-definition": {
            "label": "space_group_symmetry_operation_xyz_optimade_common",
            "kind": "property",
            "version": "1.2.0",
            "format": "1.2",
            "name": "space_group_symmetry_operation_xyz"
        },
        "type": [
            "string"
        ],
        "description": "A single symmetry operation.\n\n**Requirements/Conventions**:\n\n- The symmetry operation is described in Jones' faithful representation (Bradley & Cracknell, 1972: pp. 35-37), adapted for computer string notation.\n\n- The letters `x`, `y` and `z` that are typesetted with overbars in printed text represent coordinate values multiplied by -1 and are encoded as `-x`, `-y` and `-z`, respectively.\n- The syntax of the string representing a symmetry operation MUST conform to regular expressions given in appendix `The Symmetry Operation String Regular Expressions`_.\n\n**Bibliographic References**\n\n- Bradley, C. J. and Cracknell, A. P. (1972) The Mathematical Theory of Symmetry in Solids. Oxford, Clarendon Press (paperback edition 2010) 745 p. ISBN `978-0-19-958258-7 <https://isbnsearch.org/isbn/9780199582587>`__.\n- IUCr (2023) Core dictionary (coreCIF) version 2.4.5; data name `\\_space\\_group\\_symop\\_operation\\_xyz`. Available from: https://www.iucr.org/__data/iucr/cifdic_html/1/cif_core.dic/Ispace_group_symop_operation_xyz.html [Accessed 2023-06-18T16:46+03:00].",
        "examples": [
            "x,y,z",
            "-x,y,-z"
        ],
        "x-optimade-unit": "inapplicable"
    }
}
```
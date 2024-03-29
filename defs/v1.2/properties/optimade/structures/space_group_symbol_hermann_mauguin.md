# Hermann-Mauguin space group symbol (property)

This page documents an [OPTIMADE](https://www.optimade.org/) [Property Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/defs/v1.2/properties/optimade/structures/space_group_symbol_hermann_mauguin`](https://schemas.optimade.org/defs/v1.2/properties/optimade/structures/space_group_symbol_hermann_mauguin.md)**  
**Definition name:** `space_group_symbol_hermann_mauguin`

**Property name:** Hermann-Mauguin space group symbol  
**Description:** A human- and machine-readable string containing the short Hermann-Mauguin (H-M) symbol which specifies the space group of the structure in the response.  
**Type:** string  

**Requirements/Conventions**:

- The H-M symbol SHOULD aim to convey the closest representation of the symmetry information that can be specified using the short format used in the International Tables for Crystallography vol. A (IUCr, 2005), Table 4.3.2.1 as described in the accompanying text.
- The symbol MAY be a non-standard short H-M symbol.
- The H-M symbol does not unambiguously communicate the axis, cell, and origin choice, and the given symbol SHOULD NOT be amended to convey this information.
- To encode as character strings, the following adaptations MUST be made when representing H-M symbols given in their typesetted form:

    - the overbar above the numbers MUST be changed to the minus sign in front of the digit (e.g. `-2`);
    - subscripts that denote screw axes are written as digits immediately after the axis designator without a space (e.g. `P 32`);
    - the space group generators MUST be separated by a single space (e.g. `P 21 21 2`);
    - there MUST be no spaces in the space group generator designation (i.e. use `P 21/m`, not the `P 21 / m`);

**Bibliographic References**

- IUCr (2005). International Tables for Crystallography vol. A. Space-Group Symmetry. Ed. Theo Hahn. 5-th edition. Dordrecht, Springer.

**Examples:**

- `"C 2"`
- `"P 21 21 21"`

**Formats:** [[JSON](space_group_symbol_hermann_mauguin.json)] [[MD](space_group_symbol_hermann_mauguin.md)]

**JSON definition:**

``` json
{
    "$id": "https://schemas.optimade.org/defs/v1.2/properties/optimade/structures/space_group_symbol_hermann_mauguin",
    "$schema": "https://schemas.optimade.org/meta/v1.2/optimade/property_definition.json",
    "title": "Hermann-Mauguin space group symbol",
    "x-optimade-type": "string",
    "x-optimade-definition": {
        "label": "space_group_symbol_hermann_mauguin_optimade_structures",
        "kind": "property",
        "version": "1.2.0",
        "format": "1.2",
        "name": "space_group_symbol_hermann_mauguin"
    },
    "type": [
        "string",
        "null"
    ],
    "description": "A human- and machine-readable string containing the short Hermann-Mauguin (H-M) symbol which specifies the space group of the structure in the response.\n\n**Requirements/Conventions**:\n\n- The H-M symbol SHOULD aim to convey the closest representation of the symmetry information that can be specified using the short format used in the International Tables for Crystallography vol. A (IUCr, 2005), Table 4.3.2.1 as described in the accompanying text.\n- The symbol MAY be a non-standard short H-M symbol.\n- The H-M symbol does not unambiguously communicate the axis, cell, and origin choice, and the given symbol SHOULD NOT be amended to convey this information.\n- To encode as character strings, the following adaptations MUST be made when representing H-M symbols given in their typesetted form:\n\n    - the overbar above the numbers MUST be changed to the minus sign in front of the digit (e.g. `-2`);\n    - subscripts that denote screw axes are written as digits immediately after the axis designator without a space (e.g. `P 32`);\n    - the space group generators MUST be separated by a single space (e.g. `P 21 21 2`);\n    - there MUST be no spaces in the space group generator designation (i.e. use `P 21/m`, not the `P 21 / m`);\n\n**Bibliographic References**\n\n- IUCr (2005). International Tables for Crystallography vol. A. Space-Group Symmetry. Ed. Theo Hahn. 5-th edition. Dordrecht, Springer.",
    "examples": [
        "C 2",
        "P 21 21 21"
    ],
    "x-optimade-unit": "unapplicable"
}
```
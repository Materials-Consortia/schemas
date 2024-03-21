# extended Hermann-Mauguin space group symbol (property)

This page documents an [OPTIMADE](https://www.optimade.org/) [Property Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/defs/v1.2/properties/optimade/structures/space_group_symbol_hermann_mauguin_extended`](https://schemas.optimade.org/defs/v1.2/properties/optimade/structures/space_group_symbol_hermann_mauguin_extended.md)**  
**Definition name:** `space_group_symbol_hermann_mauguin_extended`

**Property name:** extended Hermann-Mauguin space group symbol  
**Description:** A human- and machine-readable string containing the extended Hermann-Mauguin (H-M) symbol which specifies the space group of the structure in the response.  
**Type:** string  

**Requirements/Conventions**:

- The H-M symbols SHOULD be given as specified in the International Tables for Crystallography vol. A (IUCr, 2005), Table 4.3.2.1.
- The change-of-basis operation SHOULD be provided for the non-standard axis and cell choices.
- The extended H-M symbol does not unambiguously communicate the origin choice, and the given symbol SHOULD NOT be amended to convey this information.
- The description of the change-of-basis SHOULD follow conventions of the ITC Vol. B, Sect. 1.4, Appendix A1.4.2 (IUCr, 2001).
- The same character string encoding conventions MUST be used as for the specification of the `space_group_symbol_hermann_mauguin` property.

**Bibliographic References**

- IUCr (2001). International Tables for Crystallography vol. B. Reciprocal Space. Ed. U. Shmueli. 2-nd edition. Dordrecht/Boston/London, Kluwer Academic Publishers.
- IUCr (2005). International Tables for Crystallography vol. A. Space-Group Symmetry. Ed. Theo Hahn. 5-th edition. Dordrecht, Springer.

**Examples:**

- `"C 1 2 1"`

**Formats:** [[JSON](space_group_symbol_hermann_mauguin_extended.json)] [[MD](space_group_symbol_hermann_mauguin_extended.md)]

**JSON definition:**

``` json
{
    "$id": "https://schemas.optimade.org/defs/v1.2/properties/optimade/structures/space_group_symbol_hermann_mauguin_extended",
    "$schema": "https://schemas.optimade.org/meta/v1.2/optimade/property_definition.json",
    "title": "extended Hermann-Mauguin space group symbol",
    "x-optimade-type": "string",
    "x-optimade-definition": {
        "label": "space_group_symbol_hermann_mauguin_extended_optimade_structures",
        "kind": "property",
        "version": "1.2.0",
        "format": "1.2",
        "name": "space_group_symbol_hermann_mauguin_extended"
    },
    "type": [
        "string",
        "null"
    ],
    "description": "A human- and machine-readable string containing the extended Hermann-Mauguin (H-M) symbol which specifies the space group of the structure in the response.\n\n**Requirements/Conventions**:\n\n- The H-M symbols SHOULD be given as specified in the International Tables for Crystallography vol. A (IUCr, 2005), Table 4.3.2.1.\n- The change-of-basis operation SHOULD be provided for the non-standard axis and cell choices.\n- The extended H-M symbol does not unambiguously communicate the origin choice, and the given symbol SHOULD NOT be amended to convey this information.\n- The description of the change-of-basis SHOULD follow conventions of the ITC Vol. B, Sect. 1.4, Appendix A1.4.2 (IUCr, 2001).\n- The same character string encoding conventions MUST be used as for the specification of the `space_group_symbol_hermann_mauguin` property.\n\n**Bibliographic References**\n\n- IUCr (2001). International Tables for Crystallography vol. B. Reciprocal Space. Ed. U. Shmueli. 2-nd edition. Dordrecht/Boston/London, Kluwer Academic Publishers.\n- IUCr (2005). International Tables for Crystallography vol. A. Space-Group Symmetry. Ed. Theo Hahn. 5-th edition. Dordrecht, Springer.",
    "examples": [
        "C 1 2 1"
    ],
    "x-optimade-unit": "unapplicable"
}
```
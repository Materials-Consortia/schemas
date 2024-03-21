# Hall space group symbol (property)

This page documents an [OPTIMADE](https://www.optimade.org/) [Property Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/defs/v1.2/properties/optimade/structures/space_group_symbol_hall`](https://schemas.optimade.org/defs/v1.2/properties/optimade/structures/space_group_symbol_hall.md)**  
**Definition name:** `space_group_symbol_hall`

**Property name:** Hall space group symbol  
**Description:** A Hall space group symbol representing the symmetry of the structure as defined in Hall, S. R. (1981), Acta Cryst. A37, 517-525 and erratum (1981), A37, 921.  
**Type:** string  

**Requirements/Conventions**:

- The change-of-basis operations are used as defined in the International Tables of Crystallography (ITC) Vol. B, Sect. 1.4, Appendix A1.4.2 (IUCr, 2001).
- Each component of the Hall symbol MUST be separated by a single space symbol.
- If there exists a standard Hall symbol which represents the symmetry it SHOULD be used.
- MUST be `null` if `nperiodic_dimensions` is not equal to 3.

**Explained examples**:

- Space group symbols with explicit origin (the Hall symbols):

    - `P 2c -2ac`
    - `-I 4bd 2ab 3`

- Space group symbols with change-of-basis operations:

    - `P 2yb (-1/2*x+z,1/2*x,y)`
    - `-I 4 2 (1/2*x+1/2*y,-1/2*x+1/2*y,z)`

**Bibliographic References**

- Hall, S. R. (1981) Space-group notation with an explicit origin. Acta Crystallographica Section A, 37, 517-525, International Union of Crystallography (IUCr), DOI: https://doi.org/10.1107/s0567739481001228
- Hall, S. R. (1981a) Space-group notation with an explicit origin; erratum. Acta Crystallographica Section A, 37, 921-921, International Union of Crystallography (IUCr), DOI: https://doi.org/10.1107/s0567739481001976
- IUCr (2001). International Tables for Crystallography vol. B. Reciprocal Space. Ed. U. Shmueli. 2-nd edition. Dordrecht/Boston/London, Kluwer Academic Publishers.

**Examples:**

- `"P 2c -2ac"`
- `"-I 4db 2ab 3"`
- `"P 2yb (-1/2*x+z,1/2*x,y)"`
- `"-I 4 2 (1/2*x+1/2*y,-1/2*x+1/2*y,z)"`

**Formats:** [[JSON](space_group_symbol_hall.json)] [[MD](space_group_symbol_hall.md)]

**JSON definition:**

``` json
{
    "$id": "https://schemas.optimade.org/defs/v1.2/properties/optimade/structures/space_group_symbol_hall",
    "$schema": "https://schemas.optimade.org/meta/v1.2/optimade/property_definition.json",
    "title": "Hall space group symbol",
    "x-optimade-type": "string",
    "x-optimade-definition": {
        "label": "space_group_symbol_hall_optimade_structures",
        "kind": "property",
        "version": "1.2.0",
        "format": "1.2",
        "name": "space_group_symbol_hall"
    },
    "type": [
        "string",
        "null"
    ],
    "description": "A Hall space group symbol representing the symmetry of the structure as defined in Hall, S. R. (1981), Acta Cryst. A37, 517-525 and erratum (1981), A37, 921.\n\n**Requirements/Conventions**:\n\n- The change-of-basis operations are used as defined in the International Tables of Crystallography (ITC) Vol. B, Sect. 1.4, Appendix A1.4.2 (IUCr, 2001).\n- Each component of the Hall symbol MUST be separated by a single space symbol.\n- If there exists a standard Hall symbol which represents the symmetry it SHOULD be used.\n- MUST be `null` if `nperiodic_dimensions` is not equal to 3.\n\n**Explained examples**:\n\n- Space group symbols with explicit origin (the Hall symbols):\n\n    - `P 2c -2ac`\n    - `-I 4bd 2ab 3`\n\n- Space group symbols with change-of-basis operations:\n\n    - `P 2yb (-1/2*x+z,1/2*x,y)`\n    - `-I 4 2 (1/2*x+1/2*y,-1/2*x+1/2*y,z)`\n\n**Bibliographic References**\n\n- Hall, S. R. (1981) Space-group notation with an explicit origin. Acta Crystallographica Section A, 37, 517-525, International Union of Crystallography (IUCr), DOI: https://doi.org/10.1107/s0567739481001228\n- Hall, S. R. (1981a) Space-group notation with an explicit origin; erratum. Acta Crystallographica Section A, 37, 921-921, International Union of Crystallography (IUCr), DOI: https://doi.org/10.1107/s0567739481001976\n- IUCr (2001). International Tables for Crystallography vol. B. Reciprocal Space. Ed. U. Shmueli. 2-nd edition. Dordrecht/Boston/London, Kluwer Academic Publishers.",
    "examples": [
        "P 2c -2ac",
        "-I 4db 2ab 3",
        "P 2yb (-1/2*x+z,1/2*x,y)",
        "-I 4 2 (1/2*x+1/2*y,-1/2*x+1/2*y,z)"
    ],
    "x-optimade-unit": "unapplicable"
}
```
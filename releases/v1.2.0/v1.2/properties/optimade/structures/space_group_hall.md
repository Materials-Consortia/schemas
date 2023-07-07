# Hall space group (property)

This page documents an [OPTIMADE](https://www.optimade.org/) [Property Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/defs/v1.2/properties/optimade/structures/space_group_hall`](https://schemas.optimade.org/defs/v1.2/properties/optimade/structures/space_group_hall.md)**  
**Definition name:** `space_group_hall`

**Property name:** Hall space group  
**Description:** A Hall space group symbol representing the symmetry of the structure as defined in Hall, S. R. (1981), Acta Cryst. A37, 517-525 and erratum (1981), A37, 921.  
**Type:** string  

**Requirements/Conventions**:

- Each component of the Hall symbol MUST be separated by a single space symbol.
- If there exists a standard Hall symbol which represents the symmetry it SHOULD be used.
- MUST be null if n`periodic_dimensions` is not equal to 3.

**Examples:**

- `P 2c -2ac`
- `-I 4db 2ab 3`

**Formats:** [[JSON](space_group_hall.json)] [[MD](space_group_hall.md)]

**JSON definition:**

``` json
{
    "$schema": "https://schemas.optimade.org/meta/v1.2/optimade/property_definition.md",
    "$id": "https://schemas.optimade.org/defs/v1.2/properties/optimade/structures/space_group_hall",
    "title": "Hall space group",
    "x-optimade-type": "string",
    "x-optimade-definition": {
        "kind": "property",
        "version": "1.2.0",
        "format": "1.2",
        "name": "space_group_hall"
    },
    "type": [
        "string",
        "null"
    ],
    "description": "A Hall space group symbol representing the symmetry of the structure as defined in Hall, S. R. (1981), Acta Cryst. A37, 517-525 and erratum (1981), A37, 921.\n\n**Requirements/Conventions**:\n\n- Each component of the Hall symbol MUST be separated by a single space symbol.\n- If there exists a standard Hall symbol which represents the symmetry it SHOULD be used.\n- MUST be null if n`periodic_dimensions` is not equal to 3.",
    "examples": [
        "P 2c -2ac",
        "-I 4db 2ab 3"
    ],
    "x-optimade-unit": "unapplicable"
}
```
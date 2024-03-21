# space group IT number (property)

This page documents an [OPTIMADE](https://www.optimade.org/) [Property Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/defs/v1.2/properties/optimade/structures/space_group_it_number`](https://schemas.optimade.org/defs/v1.2/properties/optimade/structures/space_group_it_number.md)**  
**Definition name:** `space_group_it_number`

**Property name:** space group IT number  
**Description:** Space group number for the structure assigned by the International Tables for Crystallography Vol. A.  
**Type:** integer  

**Requirements/Conventions**:

- The integer value MUST be between 1 and 230.
- MUST be `null` if `nperiodic_dimensions` is not equal to 3.

**Examples:**

- `42`

**Formats:** [[JSON](space_group_it_number.json)] [[MD](space_group_it_number.md)]

**JSON definition:**

``` json
{
    "$id": "https://schemas.optimade.org/defs/v1.2/properties/optimade/structures/space_group_it_number",
    "$schema": "https://schemas.optimade.org/meta/v1.2/optimade/property_definition.json",
    "title": "space group IT number",
    "x-optimade-type": "integer",
    "x-optimade-definition": {
        "label": "space_group_it_number_optimade_structures",
        "kind": "property",
        "version": "1.2.0",
        "format": "1.2",
        "name": "space_group_it_number"
    },
    "type": [
        "integer",
        "null"
    ],
    "description": "Space group number for the structure assigned by the International Tables for Crystallography Vol. A.\n\n**Requirements/Conventions**:\n\n- The integer value MUST be between 1 and 230.\n- MUST be `null` if `nperiodic_dimensions` is not equal to 3.",
    "examples": [
        42
    ],
    "x-optimade-unit": "unapplicable"
}
```
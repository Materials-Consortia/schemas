# number of periodic dimensions (property)

This page documents an [OPTIMADE](https://www.optimade.org/) [Property Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/defs/v1.2/properties/optimade/structures/nperiodic_dimensions`](https://schemas.optimade.org/defs/v1.2/properties/optimade/structures/nperiodic_dimensions.md)**  
**Definition name:** `nperiodic_dimensions`

**Property name:** number of periodic dimensions  
**Description:** An integer specifying the number of periodic dimensions in the structure, equivalent to the number of non-zero entries in `dimension_types`.  
**Type:** integer  

**Requirements/Conventions**:

- The integer value MUST be between 0 and 3 inclusive and MUST be equal to the sum of the items in the dimension_types property.

- This property only reflects the treatment of the lattice vectors provided for the structure, and not any physical interpretation of the dimensionality of its contents.

**Explained examples**

- `2` should be indicated in cases where dimension_types is any of `[1, 1, 0]`, `[1, 0, 1]`, `[0, 1, 1]`.

**Query examples**:

- Match only structures with exactly 3 periodic dimensions: `nperiodic_dimensions=3`
- Match all structures with 2 or fewer periodic dimensions: `nperiodic_dimensions<=2`

**Examples:**

- `2`

**Formats:** [[JSON](nperiodic_dimensions.json)] [[MD](nperiodic_dimensions.md)]

**JSON definition:**

``` json
{
    "$id": "https://schemas.optimade.org/defs/v1.2/properties/optimade/structures/nperiodic_dimensions",
    "$schema": "https://schemas.optimade.org/meta/v1.2/optimade/property_definition.json",
    "title": "number of periodic dimensions",
    "x-optimade-type": "integer",
    "x-optimade-definition": {
        "label": "nperiodic_dimensions_optimade_structures",
        "kind": "property",
        "version": "1.2.0",
        "format": "1.2",
        "name": "nperiodic_dimensions"
    },
    "type": [
        "integer",
        "null"
    ],
    "description": "An integer specifying the number of periodic dimensions in the structure, equivalent to the number of non-zero entries in `dimension_types`.\n\n**Requirements/Conventions**:\n\n- The integer value MUST be between 0 and 3 inclusive and MUST be equal to the sum of the items in the dimension_types property.\n\n- This property only reflects the treatment of the lattice vectors provided for the structure, and not any physical interpretation of the dimensionality of its contents.\n\n**Explained examples**\n\n- `2` should be indicated in cases where dimension_types is any of `[1, 1, 0]`, `[1, 0, 1]`, `[0, 1, 1]`.\n\n**Query examples**:\n\n- Match only structures with exactly 3 periodic dimensions: `nperiodic_dimensions=3`\n- Match all structures with 2 or fewer periodic dimensions: `nperiodic_dimensions<=2`",
    "examples": [
        2
    ],
    "x-optimade-unit": "dimensionless"
}
```
# list of number of elements (property)

This page documents an [OPTIMADE](https://www.optimade.org/) [Property Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/defs/v1.3/properties/optimade/trajectories/nelements`](https://schemas.optimade.org/defs/v1.3/properties/optimade/trajectories/nelements.md)**  
**Definition name:** `nelements`

**Property name:** list of number of elements  
**Description:** A list of nelment items.
An nelement item is the number of different elements in a structure as an integer.  
**Type:** list  

For each nelement item the following applies:

**Requirements/Conventions**:

- MUST be equal to the lengths of the list properties elements and elements_ratios, if they are provided.

**Examples:**

- `[4, 5, 7, 2]`
- `[3]`

**Formats:** [[JSON](nelements.json)] [[MD](nelements.md)]

**JSON definition:**

``` json
{
    "$id": "https://schemas.optimade.org/defs/v1.3/properties/optimade/trajectories/nelements",
    "$schema": "https://schemas.optimade.org/meta/v1.3/optimade/property_definition.json",
    "title": "list of number of elements",
    "x-optimade-type": "list",
    "x-optimade-definition": {
        "label": "nelements_optimade_trajectories",
        "kind": "property",
        "version": "1.3.0",
        "format": "1.3",
        "name": "nelements"
    },
    "x-optimade-dimensions": {
        "names": [
            "dim_frames"
        ],
        "sizes": [
            null
        ],
        "compactable": [
            "constant"
        ]
    },
    "type": [
        "array",
        "null"
    ],
    "description": "A list of nelment items.\nAn nelement item is the number of different elements in a structure as an integer.\n\nFor each nelement item the following applies:\n\n**Requirements/Conventions**:\n\n- MUST be equal to the lengths of the list properties elements and elements_ratios, if they are provided.",
    "examples": [
        [
            4,
            5,
            7,
            2
        ],
        [
            3
        ]
    ],
    "x-optimade-unit": "inapplicable",
    "items": {
        "$id": "https://schemas.optimade.org/defs/v1.2/properties/optimade/structures/nelements",
        "title": "number of elements",
        "x-optimade-type": "integer",
        "x-optimade-definition": {
            "label": "nelements_optimade_structures",
            "kind": "property",
            "version": "1.2.1",
            "format": "1.2",
            "name": "nelements"
        },
        "type": [
            "integer",
            "null"
        ],
        "description": "Number of different elements in the structure as an integer.\n\n**Requirements/Conventions**:\n\n- MUST be equal to the lengths of the list properties elements and elements_ratios, if they are provided.\n\n**Querying**:\n\n- Queries on this property can equivalently be formulated using `elements LENGTH`.\n- A filter that matches structures that have exactly 4 elements: `nelements=4`.\n- A filter that matches structures that have between 2 and 7 elements: `nelements>=2 AND nelements<=7`.",
        "examples": [
            3
        ],
        "x-optimade-unit": "dimensionless"
    }
}
```
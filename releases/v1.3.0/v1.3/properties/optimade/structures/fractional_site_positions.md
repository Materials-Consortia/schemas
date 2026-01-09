# fractional site positions (property)

This page documents an [OPTIMADE](https://www.optimade.org/) [Property Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/defs/v1.3/properties/optimade/structures/fractional_site_positions`](https://schemas.optimade.org/defs/v1.3/properties/optimade/structures/fractional_site_positions.md)**  
**Definition name:** `fractional_site_positions`

**Property name:** fractional site positions  
**Description:** Fractional coordinates (positions) of each site in the structure.  
**Type:** list  

A site is usually used to describe positions of atoms; what atoms can be encountered at a given site is conveyed by the `species_at_sites` property, and the species themselves are described in the `species` property.
Site coordinates MAY be given as `cartesian_site_positions`, `fractional_site_positions`, or both.
When symmetry operations given in `space_group_symmetry_operations_xyz` are applied, they MUST be applied to coordinates given in the `fractional_site_positions` array.

**Requirements/Conventions**:

- It MUST be a list of length equal to the number of sites in the structure, where every element is a list of the three fractional coordinates of a site expressed as float values in the fractions of the unit cell vectors given by the `lattice_vectors` property.
- An entry MAY have multiple sites at the same site position (for a relevant use of this, see e.g., the property `assemblies`).
- Since both `cartesian_site_positions` and the `fractional_site_positions` always describe the same sites, they MUST always have the same number of elements, equal to the number of elements in the `species_at_sites` array.

**Explained examples**:

- `[[0,0,0],[0,0,0.2]]` indicates a structure with two sites, one sitting at the origin and one along the third unit cell axis (*c*-axis), 1/5-th (0.2) of the vector *c* in the direction of the vector *c* from the origin.

**Examples:**

- `[[0, 0, 0], [0, 0, 0.2]]`

**Formats:** [[JSON](fractional_site_positions.json)] [[MD](fractional_site_positions.md)]

**JSON definition:**

``` json
{
    "$id": "https://schemas.optimade.org/defs/v1.3/properties/optimade/structures/fractional_site_positions",
    "$schema": "https://schemas.optimade.org/meta/v1.2/optimade/property_definition.json",
    "title": "fractional site positions",
    "x-optimade-type": "list",
    "x-optimade-definition": {
        "label": "fractional_site_positions_optimade_structures",
        "kind": "property",
        "version": "1.3.0",
        "format": "1.2",
        "name": "fractional_site_positions"
    },
    "x-optimade-dimensions": {
        "names": [
            "dim_sites",
            "dim_spatial"
        ],
        "sizes": [
            null,
            3
        ]
    },
    "type": [
        "array",
        "null"
    ],
    "description": "Fractional coordinates (positions) of each site in the structure.\n\nA site is usually used to describe positions of atoms; what atoms can be encountered at a given site is conveyed by the `species_at_sites` property, and the species themselves are described in the `species` property.\nSite coordinates MAY be given as `cartesian_site_positions`, `fractional_site_positions`, or both.\nWhen symmetry operations given in `space_group_symmetry_operations_xyz` are applied, they MUST be applied to coordinates given in the `fractional_site_positions` array.\n\n**Requirements/Conventions**:\n\n- It MUST be a list of length equal to the number of sites in the structure, where every element is a list of the three fractional coordinates of a site expressed as float values in the fractions of the unit cell vectors given by the `lattice_vectors` property.\n- An entry MAY have multiple sites at the same site position (for a relevant use of this, see e.g., the property `assemblies`).\n- Since both `cartesian_site_positions` and the `fractional_site_positions` always describe the same sites, they MUST always have the same number of elements, equal to the number of elements in the `species_at_sites` array.\n\n**Explained examples**:\n\n- `[[0,0,0],[0,0,0.2]]` indicates a structure with two sites, one sitting at the origin and one along the third unit cell axis (*c*-axis), 1/5-th (0.2) of the vector *c* in the direction of the vector *c* from the origin.",
    "examples": [
        [
            [
                0,
                0,
                0
            ],
            [
                0,
                0,
                0.2
            ]
        ]
    ],
    "x-optimade-unit": "inapplicable",
    "items": {
        "x-optimade-type": "list",
        "x-optimade-dimensions": {
            "names": [
                "dim_spatial"
            ],
            "sizes": [
                3
            ]
        },
        "type": [
            "array"
        ],
        "x-optimade-unit": "inapplicable",
        "items": {
            "x-optimade-type": "float",
            "type": [
                "number"
            ],
            "x-optimade-unit": "dimensionless"
        }
    }
}
```
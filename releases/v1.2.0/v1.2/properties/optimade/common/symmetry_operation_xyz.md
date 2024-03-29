# symmetry operation (property)

This page documents an [OPTIMADE](https://www.optimade.org/) [Property Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/defs/v1.2/properties/optimade/common/symmetry_operation_xyz`](https://schemas.optimade.org/defs/v1.2/properties/optimade/common/symmetry_operation_xyz.md)**  
**Definition name:** `symmetry_operation_xyz`

**Property name:** symmetry operation  
**Description:** A symmetry operation given as general position x, y, z coordinates in algebraic form.  
**Type:** string  

**Requirements/Conventions:**

- The symmetry operation is described by a string that gives that symmetry operation in Jones' faithful representation (Bradley & Cracknell, 1972: pp. 35-37), adapted for computer string notation.
- The letters `x`, `y` and `z` that are typesetted with overbars in printed text represent coordinate values multiplied by -1 and are encoded as `-x`, `-y` and `-z`, respectively.
- The syntax of the strings representing symmetry operations MUST conform to regular expressions given in appendix `The Symmetry Operation String Regular Expressions`_.

**Examples:**



**Formats:** [[JSON](symmetry_operation_xyz.json)] [[MD](symmetry_operation_xyz.md)]

**JSON definition:**

``` json
{
    "$id": "https://schemas.optimade.org/defs/v1.2/properties/optimade/common/symmetry_operation_xyz",
    "$schema": "https://schemas.optimade.org/meta/v1.2/optimade/property_definition.json",
    "title": "symmetry operation",
    "x-optimade-type": "string",
    "x-optimade-definition": {
        "label": "symmetry_operation_xyz_optimade_common",
        "kind": "property",
        "version": "1.2.0",
        "format": "1.2",
        "name": "symmetry_operation_xyz"
    },
    "description": "A symmetry operation given as general position x, y, z coordinates in algebraic form.\n\n**Requirements/Conventions:**\n\n- The symmetry operation is described by a string that gives that symmetry operation in Jones' faithful representation (Bradley & Cracknell, 1972: pp. 35-37), adapted for computer string notation.\n- The letters `x`, `y` and `z` that are typesetted with overbars in printed text represent coordinate values multiplied by -1 and are encoded as `-x`, `-y` and `-z`, respectively.\n- The syntax of the strings representing symmetry operations MUST conform to regular expressions given in appendix `The Symmetry Operation String Regular Expressions`_.",
    "x-optimade-unit": "inapplicable",
    "type": [
        "string"
    ],
    "maxLength": 3
}
```
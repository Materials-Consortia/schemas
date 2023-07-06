# Elements ratios (property)

This page documents an [OPTIMADE](https://www.optimade.org/) [Property Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/defs/v1.2/properties/optimade/structures/elements_ratios`](https://schemas.optimade.org/defs/v1.2/properties/optimade/structures/elements_ratios)**  
**Definition name:** `element_ratios`

**Property name:** Elements ratios  
**Description:** Relative proportions of different elements in the structure.  
**Type:** list  

**Requirements/Conventions**:

- Composed by the proportions of elements in the structure as a list of floating point numbers.
- The sum of the numbers MUST be 1.0 (within floating point accuracy)
- MUST refer to the same elements in the same order, and therefore be of the same length, as `elements`, if the latter is provided.

**Query examples**:

- Note: Useful filters can be formulated using the set operator syntax for correlated values.
  However, since the values are floating point values, the use of equality comparisons is generally inadvisable.
- OPTIONAL: a filter that matches structures where approximately 1/3 of the atoms in the structure are the element Al is: `elements:elements_ratios HAS ALL "Al":>0.3333, "Al":<0.3334`.

**Examples:**

- `[1.0]`
- `[0.3333333333333333, 0.2222222222222222, 0.4444444444444444]`

**Formats:** [[JSON](elements_ratios.json)] [[MD](elements_ratios.md)]

**JSON definition:**

``` json
{
    "$schema": "https://schemas.optimade.org/meta/v1.2/optimade/property_definition.md",
    "$id": "https://schemas.optimade.org/defs/v1.2/properties/optimade/structures/elements_ratios",
    "title": "Elements ratios",
    "x-optimade-type": "list",
    "x-optimade-definition": {
        "kind": "property",
        "version": "1.2.0",
        "format": "1.2",
        "name": "element_ratios"
    },
    "type": [
        "array",
        "null"
    ],
    "description": "Relative proportions of different elements in the structure.\n\n**Requirements/Conventions**:\n\n- Composed by the proportions of elements in the structure as a list of floating point numbers.\n- The sum of the numbers MUST be 1.0 (within floating point accuracy)\n- MUST refer to the same elements in the same order, and therefore be of the same length, as `elements`, if the latter is provided.\n\n**Query examples**:\n\n- Note: Useful filters can be formulated using the set operator syntax for correlated values.\n  However, since the values are floating point values, the use of equality comparisons is generally inadvisable.\n- OPTIONAL: a filter that matches structures where approximately 1/3 of the atoms in the structure are the element Al is: `elements:elements_ratios HAS ALL \"Al\":>0.3333, \"Al\":<0.3334`.",
    "examples": [
        [
            1.0
        ],
        [
            0.3333333333333333,
            0.2222222222222222,
            0.4444444444444444
        ]
    ],
    "x-optimade-unit": "inapplicable",
    "items": {
        "x-optimade-type": "float",
        "type": [
            "number"
        ],
        "x-optimade-unit": "dimensionless",
        "minimum": 0.0,
        "maximum": 1.0
    }
}
```
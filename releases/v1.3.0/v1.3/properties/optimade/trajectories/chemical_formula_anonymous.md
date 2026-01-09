# anonymous chemical formula (property)

This page documents an [OPTIMADE](https://www.optimade.org/) [Property Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/defs/v1.3/properties/optimade/trajectories/chemical_formula_anonymous`](https://schemas.optimade.org/defs/v1.3/properties/optimade/trajectories/chemical_formula_anonymous.md)**  
**Definition name:** `chemical_formula_anonymous`

**Property name:** anonymous chemical formula  
**Description:** A list of chemical_formula_anonymous items.
A chemical_formula_anonymous item is a string with element symbols and integer chemical proportion numbers.  
**Type:** list  

For each chemical_formula_anonymous item the following applies:

The anonymous formula is the chemical_formula_reduced, but where the elements are instead first ordered by their chemical proportion number, and then, in order left to right, replaced by anonymous symbols A, B, C, ..., Z, Aa, Ba, ..., Za, Ab, Bb, ... and so on.

**Examples:**

- `["A2B", "A42B42C16D12E10F9G5"]`

**Formats:** [[JSON](chemical_formula_anonymous.json)] [[MD](chemical_formula_anonymous.md)]

**JSON definition:**

``` json
{
    "$id": "https://schemas.optimade.org/defs/v1.3/properties/optimade/trajectories/chemical_formula_anonymous",
    "$schema": "https://schemas.optimade.org/meta/v1.3/optimade/property_definition.json",
    "title": "anonymous chemical formula",
    "x-optimade-type": "list",
    "x-optimade-definition": {
        "label": "chemical_formula_anonymous_optimade_trajectories",
        "kind": "property",
        "version": "1.3.0",
        "format": "1.3",
        "name": "chemical_formula_anonymous"
    },
    "type": [
        "array",
        "null"
    ],
    "description": "A list of chemical_formula_anonymous items.\nA chemical_formula_anonymous item is a string with element symbols and integer chemical proportion numbers.\n\nFor each chemical_formula_anonymous item the following applies:\n\nThe anonymous formula is the chemical_formula_reduced, but where the elements are instead first ordered by their chemical proportion number, and then, in order left to right, replaced by anonymous symbols A, B, C, ..., Z, Aa, Ba, ..., Za, Ab, Bb, ... and so on.",
    "examples": [
        [
            "A2B",
            "A42B42C16D12E10F9G5"
        ]
    ],
    "x-optimade-unit": "inapplicable",
    "items": {
        "$id": "https://schemas.optimade.org/defs/v1.2/properties/optimade/structures/chemical_formula_anonymous",
        "title": "anonymous chemical formula",
        "x-optimade-type": "string",
        "x-optimade-definition": {
            "label": "chemical_formula_anonymous_optimade_structures",
            "kind": "property",
            "version": "1.2.0",
            "format": "1.2",
            "name": "chemical_formula_anonymous"
        },
        "type": [
            "string",
            "null"
        ],
        "description": "The anonymous formula is the chemical_formula_reduced, but where the elements are instead first ordered by their chemical proportion number, and then, in order left to right, replaced by anonymous symbols A, B, C, ..., Z, Aa, Ba, ..., Za, Ab, Bb, ... and so on.",
        "examples": [
            "A2B",
            "A42B42C16D12E10F9G5"
        ],
        "x-optimade-unit": "inapplicable"
    }
}
```
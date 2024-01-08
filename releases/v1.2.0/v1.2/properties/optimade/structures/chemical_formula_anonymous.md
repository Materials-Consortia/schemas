# Anonymous chemical formula (property)

This page documents an [OPTIMADE](https://www.optimade.org/) [Property Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/defs/v1.2/properties/optimade/structures/chemical_formula_anonymous`](https://schemas.optimade.org/defs/v1.2/properties/optimade/structures/chemical_formula_anonymous.md)**  
**Definition name:** `chemical_formula_anonymous`

**Property name:** Anonymous chemical formula  
**Description:** The anonymous formula is the chemical_formula_reduced, but where the elements are instead first ordered by their chemical proportion number, and then, in order left to right, replaced by anonymous symbols A, B, C, ..., Z, Aa, Ba, ..., Za, Ab, Bb, ... and so on.  
**Type:** string  



**Examples:**

- `A2B`
- `A42B42C16D12E10F9G5`

**Formats:** [[JSON](chemical_formula_anonymous.json)] [[MD](chemical_formula_anonymous.md)]

**JSON definition:**

``` json
{
    "$schema": "https://schemas.optimade.org/meta/v1.2/optimade/property_definition.md",
    "$id": "https://schemas.optimade.org/defs/v1.2/properties/optimade/structures/chemical_formula_anonymous",
    "title": "Anonymous chemical formula",
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
```
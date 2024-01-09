# Reduced chemical formula (property)

This page documents an [OPTIMADE](https://www.optimade.org/) [Property Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/defs/v1.2/properties/optimade/structures/chemical_formula_reduced`](https://schemas.optimade.org/defs/v1.2/properties/optimade/structures/chemical_formula_reduced.md)**  
**Definition name:** `chemical_formula_reduced`

**Property name:** Reduced chemical formula  
**Description:** The reduced chemical formula for a structure as a string with element symbols and integer chemical proportion numbers.  
**Type:** string  

**Requirements/Conventions**:

- Intricate queries on formula components are suggested to be formulated using set-type filter operators on the multi valued `elements` and `elements_ratios` properties.
- Element symbols MUST have proper capitalization (e.g., `"Si"`, not `"SI"` for "silicon").
- Elements MUST be placed in alphabetical order, followed by their integer chemical proportion number.
- For structures with no partial occupation, the chemical proportion numbers are the smallest integers for which the chemical proportion is exactly correct.
- For structures with partial occupation, the chemical proportion numbers are integers that within reasonable approximation indicate the correct chemical proportions. The precise details of how to perform the rounding is chosen by the API implementation.
- No spaces or separators are allowed.

**Query examples**:

- A filter that matches an exactly given formula is `chemical_formula_reduced="H2NaO"`.

**Examples:**

- `H2NaO`
- `ClNa`
- `CCaO3`

**Formats:** [[JSON](chemical_formula_reduced.json)] [[MD](chemical_formula_reduced.md)]

**JSON definition:**

``` json
{
    "$id": "https://schemas.optimade.org/defs/v1.2/properties/optimade/structures/chemical_formula_reduced",
    "$schema": "https://schemas.optimade.org/meta/v1.2/optimade/property_definition.json",
    "title": "Reduced chemical formula",
    "x-optimade-type": "string",
    "x-optimade-definition": {
        "label": "chemical_formula_reduced_optimade_structures",
        "kind": "property",
        "version": "1.2.0",
        "format": "1.2",
        "name": "chemical_formula_reduced"
    },
    "type": [
        "string",
        "null"
    ],
    "description": "The reduced chemical formula for a structure as a string with element symbols and integer chemical proportion numbers.\n\n**Requirements/Conventions**:\n\n- Intricate queries on formula components are suggested to be formulated using set-type filter operators on the multi valued `elements` and `elements_ratios` properties.\n- Element symbols MUST have proper capitalization (e.g., `\"Si\"`, not `\"SI\"` for \"silicon\").\n- Elements MUST be placed in alphabetical order, followed by their integer chemical proportion number.\n- For structures with no partial occupation, the chemical proportion numbers are the smallest integers for which the chemical proportion is exactly correct.\n- For structures with partial occupation, the chemical proportion numbers are integers that within reasonable approximation indicate the correct chemical proportions. The precise details of how to perform the rounding is chosen by the API implementation.\n- No spaces or separators are allowed.\n\n**Query examples**:\n\n- A filter that matches an exactly given formula is `chemical_formula_reduced=\"H2NaO\"`.",
    "examples": [
        "H2NaO",
        "ClNa",
        "CCaO3"
    ],
    "x-optimade-unit": "inapplicable"
}
```
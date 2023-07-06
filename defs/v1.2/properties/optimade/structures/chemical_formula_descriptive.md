# Descriptive chemical formula (property)

This page documents an [OPTIMADE](https://www.optimade.org/) [Property Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/defs/v1.2/properties/optimade/structures/chemical_formula_descriptive`](https://schemas.optimade.org/defs/v1.2/properties/optimade/structures/chemical_formula_descriptive)**  
**Definition name:** `chemical_formula_descriptive`

**Property name:** Descriptive chemical formula  
**Description:** The chemical formula for a structure as a string in a form chosen by the API implementation.  
**Type:** string  

**Requirements/Conventions**:

- The chemical formula is given as a string consisting of properly capitalized element symbols followed by integers or decimal numbers, balanced parentheses, square, and curly brackets `(`,\ `)`, `[`,\ `]`, `{`, `}`, commas, the `+`, `-`, `:` and `=` symbols.
  The parentheses are allowed to be followed by a number.
  Spaces are allowed anywhere except within chemical symbols.
  The order of elements and any groupings indicated by parentheses or brackets are chosen freely by the API implementation.
- The string SHOULD be arithmetically consistent with the element ratios in the `chemical_formula_reduced` property.
- It is RECOMMENDED, but not mandatory, that symbols, parentheses and brackets, if used, are used with the meanings prescribed by [IUPAC's Nomenclature of Organic Chemistry](https://www.qmul.ac.uk/sbcs/iupac/bibliog/blue.html).

**Query examples**:

- Note: the free-form nature of this property is likely to make queries on it across different databases inconsistent.
- A filter that matches an exactly given formula: `chemical_formula_descriptive="(H2O)2 Na"`.
- A filter that does a partial match: `chemical_formula_descriptive CONTAINS "H2O"`.

**Examples:**

- `(H2O)2 Na`
- `NaCl`
- `CaCO3`
- `CCaO3`
- `(CH3)3N+ - [CH2]2-OH = Me3N+ - CH2 - CH2OH`

**Formats:** [[JSON](chemical_formula_descriptive.json)] [[MD](chemical_formula_descriptive.md)]

**JSON definition:**

``` json
{
    "$schema": "https://schemas.optimade.org/meta/v1.2/optimade/property_definition.md",
    "$id": "https://schemas.optimade.org/defs/v1.2/properties/optimade/structures/chemical_formula_descriptive",
    "title": "Descriptive chemical formula",
    "x-optimade-type": "string",
    "x-optimade-definition": {
        "kind": "property",
        "version": "1.2.0",
        "format": "1.2",
        "name": "chemical_formula_descriptive"
    },
    "type": [
        "string",
        "null"
    ],
    "description": "The chemical formula for a structure as a string in a form chosen by the API implementation.\n\n**Requirements/Conventions**:\n\n- The chemical formula is given as a string consisting of properly capitalized element symbols followed by integers or decimal numbers, balanced parentheses, square, and curly brackets `(`,\\ `)`, `[`,\\ `]`, `{`, `}`, commas, the `+`, `-`, `:` and `=` symbols.\n  The parentheses are allowed to be followed by a number.\n  Spaces are allowed anywhere except within chemical symbols.\n  The order of elements and any groupings indicated by parentheses or brackets are chosen freely by the API implementation.\n- The string SHOULD be arithmetically consistent with the element ratios in the `chemical_formula_reduced` property.\n- It is RECOMMENDED, but not mandatory, that symbols, parentheses and brackets, if used, are used with the meanings prescribed by [IUPAC's Nomenclature of Organic Chemistry](https://www.qmul.ac.uk/sbcs/iupac/bibliog/blue.html).\n\n**Query examples**:\n\n- Note: the free-form nature of this property is likely to make queries on it across different databases inconsistent.\n- A filter that matches an exactly given formula: `chemical_formula_descriptive=\"(H2O)2 Na\"`.\n- A filter that does a partial match: `chemical_formula_descriptive CONTAINS \"H2O\"`.",
    "examples": [
        "(H2O)2 Na",
        "NaCl",
        "CaCO3",
        "CCaO3",
        "(CH3)3N+ - [CH2]2-OH = Me3N+ - CH2 - CH2OH"
    ],
    "x-optimade-unit": "inapplicable"
}
```
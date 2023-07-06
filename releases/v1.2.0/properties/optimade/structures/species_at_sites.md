# Species at sites (property)

This page documents an [OPTIMADE](https://www.optimade.org/) [Property Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/defs/v1.2/properties/optimade/structures/species_at_sites`](https://schemas.optimade.org/defs/v1.2/properties/optimade/structures/species_at_sites)**  
**Definition name:** `species_at_sites`

**Property name:** Species at sites  
**Description:** Name of the species at each site (where values for sites are specified with the same order of the property `cartesian_site_positions`). The properties of the species are found in the property `species`.  
**Type:** list  

**Requirements/Conventions**:

- MUST have length equal to the number of sites in the structure (first dimension of the list property `cartesian_site_positions`).
- Each species name mentioned in the `species_at_sites` list MUST be described in the list property `species` (i.e. for each value in the `species_at_sites` list there MUST exist exactly one dictionary in the `species` list with the `name` attribute equal to the corresponding `species_at_sites` value).
- Each site MUST be associated only to a single species.
  **Note**: However, species can represent mixtures of atoms, and multiple species MAY be defined for the same chemical element.
  This latter case is useful when different atoms of the same type need to be grouped or distinguished, for instance in simulation codes to assign different initial spin states.

**Explained examples**:

- `["Ti","O2"]` indicates that the first site is hosting a species labeled `"Ti"` and the second a species labeled `"O2"`
- `["Ac", "Ac", "Ag", "Ir"]` indicates that the first two sites contain the `"Ac"` species, while the third and fourth sites contain the `"Ag"` and `"Ir"` species, respectively.

**Examples:**

- `['Ti', 'O2']`
- `['Ac', 'Ac', 'Ag', 'Ir']`

**Formats:** [[JSON](species_at_sites.json)] [[MD](species_at_sites.md)]

**JSON definition:**

``` json
{
    "$schema": "https://schemas.optimade.org/meta/v1.2/optimade/property_definition.md",
    "$id": "https://schemas.optimade.org/defs/v1.2/properties/optimade/structures/species_at_sites",
    "title": "Species at sites",
    "x-optimade-type": "list",
    "x-optimade-definition": {
        "kind": "property",
        "version": "1.2.0",
        "format": "1.2",
        "name": "species_at_sites"
    },
    "type": [
        "array",
        "null"
    ],
    "description": "Name of the species at each site (where values for sites are specified with the same order of the property `cartesian_site_positions`). The properties of the species are found in the property `species`.\n\n**Requirements/Conventions**:\n\n- MUST have length equal to the number of sites in the structure (first dimension of the list property `cartesian_site_positions`).\n- Each species name mentioned in the `species_at_sites` list MUST be described in the list property `species` (i.e. for each value in the `species_at_sites` list there MUST exist exactly one dictionary in the `species` list with the `name` attribute equal to the corresponding `species_at_sites` value).\n- Each site MUST be associated only to a single species.\n  **Note**: However, species can represent mixtures of atoms, and multiple species MAY be defined for the same chemical element.\n  This latter case is useful when different atoms of the same type need to be grouped or distinguished, for instance in simulation codes to assign different initial spin states.\n\n**Explained examples**:\n\n- `[\"Ti\",\"O2\"]` indicates that the first site is hosting a species labeled `\"Ti\"` and the second a species labeled `\"O2\"`\n- `[\"Ac\", \"Ac\", \"Ag\", \"Ir\"]` indicates that the first two sites contain the `\"Ac\"` species, while the third and fourth sites contain the `\"Ag\"` and `\"Ir\"` species, respectively.",
    "examples": [
        [
            "Ti",
            "O2"
        ],
        [
            "Ac",
            "Ac",
            "Ag",
            "Ir"
        ]
    ],
    "x-optimade-unit": "inapplicable",
    "items": {
        "$id": "https://schemas.optimade.org/defs/v1.2/properties/optimade/common/species_name",
        "title": "Name of the species",
        "x-optimade-type": "string",
        "x-optimade-definition": {
            "kind": "property",
            "version": "1.2.0",
            "format": "1.2",
            "name": "species_name"
        },
        "type": [
            "string"
        ],
        "description": "The name of the species.",
        "examples": [
            "Na",
            "Si[32982]",
            "quop"
        ],
        "x-optimade-unit": "inapplicable"
    }
}
```
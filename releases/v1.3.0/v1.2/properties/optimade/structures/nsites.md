# number of sites (property)

This page documents an [OPTIMADE](https://www.optimade.org/) [Property Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/defs/v1.2/properties/optimade/structures/nsites`](https://schemas.optimade.org/defs/v1.2/properties/optimade/structures/nsites.md)**  
**Definition name:** `nsites`

**Property name:** number of sites  
**Description:** An integer specifying the length of the `cartesian_site_positions` property.  
**Type:** integer  

**Requirements/Conventions**:

- MUST be equal to the lengths of the list properties elements and elements_ratios, if they are provided.

**Query examples**:

- Match only structures with exactly 4 sites: `nsites=4`
- Match structures that have between 2 and 7 sites: `nsites>=2 AND nsites<=7`

**Examples:**

- `42`

**Formats:** [[JSON](nsites.json)] [[MD](nsites.md)]

**JSON definition:**

``` json
{
    "$id": "https://schemas.optimade.org/defs/v1.2/properties/optimade/structures/nsites",
    "$schema": "https://schemas.optimade.org/meta/v1.2/optimade/property_definition.json",
    "title": "number of sites",
    "x-optimade-type": "integer",
    "x-optimade-definition": {
        "label": "nsites_optimade_structures",
        "kind": "property",
        "version": "1.2.0",
        "format": "1.2",
        "name": "nsites"
    },
    "type": [
        "integer",
        "null"
    ],
    "description": "An integer specifying the length of the `cartesian_site_positions` property.\n\n**Requirements/Conventions**:\n\n- MUST be equal to the lengths of the list properties elements and elements_ratios, if they are provided.\n\n**Query examples**:\n\n- Match only structures with exactly 4 sites: `nsites=4`\n- Match structures that have between 2 and 7 sites: `nsites>=2 AND nsites<=7`",
    "examples": [
        42
    ],
    "x-optimade-unit": "dimensionless"
}
```
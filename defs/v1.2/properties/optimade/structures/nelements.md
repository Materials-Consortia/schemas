# Number of elements (property)

This page documents an [OPTIMADE](https://www.optimade.org/) [Property Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/defs/v1.2/properties/optimade/structures/nelements`](https://schemas.optimade.org/defs/v1.2/properties/optimade/structures/nelements)**  
**Definition name:** `nelements`

**Property name:** Number of elements  
**Description:** Number of different elements in the structure as an integer.  
**Type:** integer  
**Implementation requirements:**  
- **Support:** SHOULD be supported by all implementations, i.e., SHOULD NOT be `null`.  

- **Query:** MUST be a queryable property with support for all mandatory filter features.  

**Requirements/Conventions**:

- MUST be equal to the lengths of the list properties elements and elements_ratios, if they are provided.

**Querying**:

- Queries on this property can equivalently be formulated using `elements LENGTH`.
- A filter that matches structures that have exactly 4 elements: `nelements=4`.
- A filter that matches structures that have between 2 and 7 elements: `nelements>=2 AND nelements<=7`.

**Examples:**

- `3`

**Formats:** [[JSON](nelements.json)] [[MD](nelements.md)]

**JSON definition:**

``` json
{
    "$schema": "https://schemas.optimade.org/meta/v1.2/optimade/property_definition.md",
    "$id": "https://schemas.optimade.org/defs/v1.2/properties/optimade/structures/nelements",
    "title": "Number of elements",
    "x-optimade-type": "integer",
    "x-optimade-definition": {
        "kind": "property",
        "version": "1.2.0",
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
    "x-optimade-unit": "dimensionless",
    "x-optimade-requirements": {
        "support": "should",
        "sortable": false,
        "query-support": "all mandatory"
    }
}
```
# editors (property)

This page documents an [OPTIMADE](https://www.optimade.org/) [Property Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/defs/v1.2/properties/optimade/references/editors`](https://schemas.optimade.org/defs/v1.2/properties/optimade/references/editors.md)**  
**Definition name:** `editors`

**Property name:** editors  
**Description:** A list of dictionaries with names of the editors.  
**Type:** list  

**Requirements/Conventions**:

- Each list member MUST be a dictionary with the following keys:

  - **name**: Full name of the person, REQUIRED.
  - **firstname**, **lastname**: Parts of the person's name, OPTIONAL.

**Examples:**

- `[OrderedDict([('name', 'John Smith')]), OrderedDict([('name', 'Arthur Dent'), ('firstname', 'Arthur'), ('lastname', 'Dent')])]`

**Formats:** [[JSON](editors.json)] [[MD](editors.md)]

**JSON definition:**

``` json
{
    "$id": "https://schemas.optimade.org/defs/v1.2/properties/optimade/references/editors",
    "$schema": "https://schemas.optimade.org/meta/v1.2/optimade/property_definition.json",
    "title": "editors",
    "x-optimade-type": "list",
    "x-optimade-definition": {
        "label": "editors_optimade_references",
        "kind": "property",
        "version": "1.2.0",
        "format": "1.2",
        "name": "editors"
    },
    "x-optimade-dimensions": {
        "names": [
            "dim_editors"
        ]
    },
    "type": [
        "array",
        "null"
    ],
    "description": "A list of dictionaries with names of the editors.\n\n**Requirements/Conventions**:\n\n- Each list member MUST be a dictionary with the following keys:\n\n  - **name**: Full name of the person, REQUIRED.\n  - **firstname**, **lastname**: Parts of the person's name, OPTIONAL.",
    "items": {
        "$id": "https://schemas.optimade.org/defs/v1.2/properties/optimade/common/person",
        "title": "person",
        "x-optimade-type": "dictionary",
        "x-optimade-definition": {
            "label": "person_optimade_common",
            "kind": "property",
            "version": "1.2.0",
            "format": "1.2",
            "name": "person"
        },
        "type": [
            "object",
            "null"
        ],
        "description": "A dictionary with name information about a person.\n\n**Requirements/Conventions**:\n\n- The dictionary MUST adhere to the following format:\n\n  - **name**: Full name of the person, REQUIRED.\n  - **firstname**, **lastname**: Parts of the person's name, OPTIONAL.",
        "required": [
            "name"
        ],
        "properties": {
            "name": {
                "x-optimade-type": "string",
                "x-optimade-unit": "inapplicable",
                "type": [
                    "string"
                ]
            },
            "firstname": {
                "x-optimade-type": "string",
                "x-optimade-unit": "inapplicable",
                "type": [
                    "string"
                ]
            },
            "lastname": {
                "x-optimade-type": "string",
                "x-optimade-unit": "inapplicable",
                "type": [
                    "string"
                ]
            }
        },
        "examples": [
            {
                "name": "John Smith"
            },
            {
                "name": "Arthur Dent",
                "firstname": "Arthur",
                "lastname": "Dent"
            }
        ],
        "x-optimade-unit": "inapplicable"
    },
    "examples": [
        [
            {
                "name": "John Smith"
            },
            {
                "name": "Arthur Dent",
                "firstname": "Arthur",
                "lastname": "Dent"
            }
        ]
    ],
    "x-optimade-unit": "inapplicable"
}
```
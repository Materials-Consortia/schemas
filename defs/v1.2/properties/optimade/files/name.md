# Name (property)

This page documents an [OPTIMADE](https://www.optimade.org/) [Property Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/defs/v1.2/properties/optimade/files/name`](https://schemas.optimade.org/defs/v1.2/properties/optimade/files/name.md)**  
**Definition name:** `name`

**Property name:** Name  
**Description:** Base name of a file.  
**Type:** string  
**Implementation requirements:**  
- **Support:** MUST be supported by all implementations, MUST NOT be `null`.  

- **Query:** Support for queries on this property is OPTIONAL.  

**Requirements/Conventions:**

- File name extension is an integral part of a file name and, if available, MUST be included.

**Examples:**

- `1000000.cif`

**Formats:** [[JSON](name.json)] [[MD](name.md)]

**JSON definition:**

``` json
{
    "$id": "https://schemas.optimade.org/defs/v1.2/properties/optimade/files/name",
    "$schema": "https://schemas.optimade.org/meta/v1.2/optimade/property_definition.json",
    "title": "Name",
    "x-optimade-type": "string",
    "x-optimade-definition": {
        "label": "name_optimade_files",
        "kind": "property",
        "version": "1.2.0",
        "format": "1.2",
        "name": "name"
    },
    "type": [
        "string"
    ],
    "description": "Base name of a file.\n\n**Requirements/Conventions:**\n\n- File name extension is an integral part of a file name and, if available, MUST be included.",
    "examples": [
        "1000000.cif"
    ],
    "x-optimade-unit": "inapplicable",
    "x-optimade-requirements": {
        "support": "must",
        "sortable": false,
        "query-support": "none"
    }
}
```
# Immutable ID (property)

This page documents an [OPTIMADE](https://www.optimade.org/) [Property Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/defs/v1.2/properties/core/immutable_id`](https://schemas.optimade.org/defs/v1.2/properties/core/immutable_id.md)**  
**Definition name:** `immutable_id`

**Property name:** Immutable ID  
**Description:** The entry's immutable ID (e.g., a UUID).  
**Type:** string  

**Requirements/Conventions:**

- This is important for databases having preferred IDs that point to "the latest version" of a record, but still offer access to older variants.
- This ID maps to the version-specific record, in case it changes in the future.

**Examples:**

- `8bd3e750-b477-41a0-9b11-3a799f21b44f`
- `fjeiwoj,54;@=%<>#32`

**Formats:** [[JSON](immutable_id.json)] [[MD](immutable_id.md)]

**JSON definition:**

``` json
{
    "$id": "https://schemas.optimade.org/defs/v1.2/properties/core/immutable_id",
    "$schema": "https://schemas.optimade.org/meta/v1.2/optimade/property_definition.json",
    "title": "Immutable ID",
    "x-optimade-type": "string",
    "x-optimade-definition": {
        "label": "immutable_id_core",
        "kind": "property",
        "version": "1.2.0",
        "format": "1.2",
        "name": "immutable_id"
    },
    "type": [
        "string",
        "null"
    ],
    "description": "The entry's immutable ID (e.g., a UUID).\n\n**Requirements/Conventions:**\n\n- This is important for databases having preferred IDs that point to \"the latest version\" of a record, but still offer access to older variants.\n- This ID maps to the version-specific record, in case it changes in the future.",
    "examples": [
        "8bd3e750-b477-41a0-9b11-3a799f21b44f",
        "fjeiwoj,54;@=%<>#32"
    ],
    "x-optimade-unit": "inapplicable"
}
```
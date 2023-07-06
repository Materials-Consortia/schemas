# url (property)

This page documents an [OPTIMADE](https://www.optimade.org/) [Property Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/defs/v1.2/properties/optimade/references/url`](https://schemas.optimade.org/defs/v1.2/properties/optimade/references/url)**  
**Definition name:** `url`

**Property name:** url  
**Description:** The URL of the object being referenced.  
**Type:** string  



**Examples:**

- `https://example.com/papers/my_paper`

**Formats:** [[JSON](url.json)] [[MD](url.md)]

**JSON definition:**

``` json
{
    "$schema": "https://schemas.optimade.org/meta/v1.2/optimade/property_definition.md",
    "$id": "https://schemas.optimade.org/defs/v1.2/properties/optimade/references/url",
    "title": "url",
    "x-optimade-type": "string",
    "x-optimade-definition": {
        "kind": "property",
        "version": "1.2.0",
        "format": "1.2",
        "name": "url"
    },
    "type": [
        "string",
        "null"
    ],
    "description": "The URL of the object being referenced.",
    "examples": [
        "https://example.com/papers/my_paper"
    ],
    "x-optimade-unit": "inapplicable"
}
```
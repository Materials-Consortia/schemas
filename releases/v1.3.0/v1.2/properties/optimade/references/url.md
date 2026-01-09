# URL (property)

This page documents an [OPTIMADE](https://www.optimade.org/) [Property Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/defs/v1.2/properties/optimade/references/url`](https://schemas.optimade.org/defs/v1.2/properties/optimade/references/url.md)**  
**Definition name:** `url`

**Property name:** URL  
**Description:** The URL of the object being referenced.  
**Type:** string  



**Examples:**

- `"https://example.com/papers/my_paper"`

**Formats:** [[JSON](url.json)] [[MD](url.md)]

**JSON definition:**

``` json
{
    "$id": "https://schemas.optimade.org/defs/v1.2/properties/optimade/references/url",
    "$schema": "https://schemas.optimade.org/meta/v1.2/optimade/property_definition.json",
    "title": "URL",
    "x-optimade-type": "string",
    "x-optimade-definition": {
        "label": "url_optimade_references",
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
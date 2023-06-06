# URL (property)
This page documents an [OPTIMADE](https://www.optimade.org/) [Property Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/properties/v1.2.0/optimade/files/url`](https://schemas.optimade.org/properties/v1.2.0/optimade/files/url)**  
**Definition name:** `url`

**Property name:** URL  
**Description:** The URL to get the contents of a file.  
**Type:** string  

**Requirements/Conventions:**

- The URL MUST point to the actual contents of a file (i.e. byte stream), not an intermediate (preview) representation. For example, if referring to a file on GitHub, a link should point to raw contents.

**Examples:**

- `https://example.org/files/cifs/1000000.cif`

**Formats:** [[JSON](url.json)] [[MD](url.md)]

**JSON definition:**

``` json
{
    "$id": "https://schemas.optimade.org/properties/v1.2.0/optimade/files/url",
    "title": "URL",
    "x-optimade-type": "string",
    "x-optimade-definition": {
        "kind": "property",
        "version": "1.2.0",
        "format": "1.2",
        "name": "url"
    },
    "type": [
        "string"
    ],
    "description": "The URL to get the contents of a file.\n\n**Requirements/Conventions:**\n\n- The URL MUST point to the actual contents of a file (i.e. byte stream), not an intermediate (preview) representation. For example, if referring to a file on GitHub, a link should point to raw contents.",
    "examples": [
        "https://example.org/files/cifs/1000000.cif"
    ],
    "x-optimade-unit": "inapplicable",
    "$schema": "https://schemas.optimade.org/meta/v1.2.0/optimade/property_definition.md"
}
```
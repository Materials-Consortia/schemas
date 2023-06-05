# URL stable until (property)
This page documents an [OPTIMADE](https://www.optimade.org/) [Property Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/properties/v1.2.0/optimade/file/url_stable_until`](https://schemas.optimade.org/properties/v1.2.0/optimade/file/url_stable_until)**  
**Definition name:** `url_stable_until`

**Property name:** URL stable until  
**Description:** Point in time until which the URL in `url` is guaranteed to stay stable.  
**Type:** timestamp  

**Requirements/Conventions:**

- `null` means that there is no stability guarantee for the URL in url.
  Indefinite support could be communicated by providing a date sufficiently far in the future, for example, 9999-12-31.

**Examples:**

- `2052-04-05T14:30:20Z`

**Formats:** [[JSON](url_stable_until.json)] [[MD](url_stable_until.md)]

**JSON definition:**

``` json
{
    "$id": "https://schemas.optimade.org/properties/v1.2.0/optimade/file/url_stable_until",
    "title": "URL stable until",
    "x-optimade-type": "timestamp",
    "x-optimade-definition": {
        "kind": "property",
        "version": "1.2.0",
        "format": "1.2",
        "name": "url_stable_until"
    },
    "type": [
        "string",
        "null"
    ],
    "description": "Point in time until which the URL in `url` is guaranteed to stay stable.\n\n**Requirements/Conventions:**\n\n- `null` means that there is no stability guarantee for the URL in url.\n  Indefinite support could be communicated by providing a date sufficiently far in the future, for example, 9999-12-31.",
    "examples": [
        "2052-04-05T14:30:20Z"
    ],
    "x-optimade-unit": "inapplicable",
    "format": "date-time",
    "$schema": "https://schemas.optimade.org/meta/v1.2.0/optimade/property_definition.md"
}
```
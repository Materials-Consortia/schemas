# Media type (property)

This page documents an [OPTIMADE](https://www.optimade.org/) [Property Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/defs/v1.2/properties/optimade/files/media_type`](https://schemas.optimade.org/defs/v1.2/properties/optimade/files/media_type.md)**  
**Definition name:** `media_type`

**Property name:** Media type  
**Description:** Media type identifier (also known as MIME type), for a file as per [RFC 6838 Media Type Specifications and Registration Procedures](https://datatracker.ietf.org/doc/html/rfc6838).  
**Type:** string  



**Examples:**

- `chemical/x-cif`

**Formats:** [[JSON](media_type.json)] [[MD](media_type.md)]

**JSON definition:**

``` json
{
    "$schema": "https://schemas.optimade.org/meta/v1.2/optimade/property_definition.md",
    "$id": "https://schemas.optimade.org/defs/v1.2/properties/optimade/files/media_type",
    "title": "Media type",
    "x-optimade-type": "string",
    "x-optimade-definition": {
        "label": "media_type_optimade_files",
        "kind": "property",
        "version": "1.2.0",
        "format": "1.2",
        "name": "media_type"
    },
    "type": [
        "string",
        "null"
    ],
    "description": "Media type identifier (also known as MIME type), for a file as per [RFC 6838 Media Type Specifications and Registration Procedures](https://datatracker.ietf.org/doc/html/rfc6838).",
    "examples": [
        "chemical/x-cif"
    ],
    "x-optimade-unit": "inapplicable"
}
```
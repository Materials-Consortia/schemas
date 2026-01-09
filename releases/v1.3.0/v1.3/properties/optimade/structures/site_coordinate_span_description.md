# site coordinate span description (property)

This page documents an [OPTIMADE](https://www.optimade.org/) [Property Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/defs/v1.3/properties/optimade/structures/site_coordinate_span_description`](https://schemas.optimade.org/defs/v1.3/properties/optimade/structures/site_coordinate_span_description.md)**  
**Definition name:** `site_coordinate_span_description`

**Property name:** site coordinate span description  
**Description:** Human-readable semi-formal characterization of the coordinate span when the `site_coordinate_span` property has value `other`.  
**Type:** string  



**Examples:**

- `"Two fullerene molecules with a VdW contact."`

**Formats:** [[JSON](site_coordinate_span_description.json)] [[MD](site_coordinate_span_description.md)]

**JSON definition:**

``` json
{
    "$id": "https://schemas.optimade.org/defs/v1.3/properties/optimade/structures/site_coordinate_span_description",
    "$schema": "https://schemas.optimade.org/meta/v1.2/optimade/property_definition.json",
    "title": "site coordinate span description",
    "x-optimade-type": "string",
    "x-optimade-definition": {
        "label": "site_coordinate_span_description_optimade_structures",
        "kind": "property",
        "version": "1.3.0",
        "format": "1.2",
        "name": "site_coordinate_span_description"
    },
    "type": [
        "string",
        "null"
    ],
    "description": "Human-readable semi-formal characterization of the coordinate span when the `site_coordinate_span` property has value `other`.",
    "examples": [
        "Two fullerene molecules with a VdW contact."
    ],
    "x-optimade-unit": "inapplicable"
}
```
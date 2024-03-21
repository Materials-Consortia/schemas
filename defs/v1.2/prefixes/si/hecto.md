# hecto, h (prefix)

This page documents an [OPTIMADE](https://www.optimade.org/) [Prefix Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/defs/v1.2/prefixes/si/hecto`](https://schemas.optimade.org/defs/v1.2/prefixes/si/hecto.md)**  
**Definition name:** `hecto`

**Prefix name:** hecto  
**Latin symbol:** h  
**Display symbol:** h  
  
**Description:** The hecto SI prefix defined as a dimensionless multiple of 10², adopted into SI at its creation at the 11th CGPM Meeting in 1960, resolution 12.



**Resources:**

- [Definition in the 11th CGPM Meeting in 1960, resolution 12](https://www.bipm.org/en/committees/cg/cgpm/11-1960/resolution-12)
- [Wikipedia article describing the prefix](https://en.wikipedia.org/wiki/Hecto-)


**Formats:** [[JSON](hecto.json)] [[MD](hecto.md)]

**JSON definition:**

``` json
{
    "$id": "https://schemas.optimade.org/defs/v1.2/prefixes/si/hecto",
    "$schema": "https://schemas.optimade.org/meta/v1.2/optimade/prefix_definition.json",
    "title": "hecto",
    "symbol": "h",
    "display-symbol": "h",
    "description": "The hecto SI prefix defined as a dimensionless multiple of 10\u00b2, adopted into SI at its creation at the 11th CGPM Meeting in 1960, resolution 12.",
    "resources": [
        {
            "relation": "Definition in the 11th CGPM Meeting in 1960, resolution 12",
            "resource-id": "https://www.bipm.org/en/committees/cg/cgpm/11-1960/resolution-12"
        },
        {
            "relation": "Wikipedia article describing the prefix",
            "resource-id": "https://en.wikipedia.org/wiki/Hecto-"
        }
    ],
    "defining-relation": {
        "base-units": [],
        "base-units-expression": "",
        "scale": {
            "exponent": 2
        }
    },
    "x-optimade-definition": {
        "label": "hecto_prefix_si",
        "kind": "prefix",
        "format": "1.2",
        "version": "1.2.0",
        "name": "hecto"
    }
}
```
# deci, d (prefix)

This page documents an [OPTIMADE](https://www.optimade.org/) [Prefix Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/defs/v1.2/prefixes/si/deci`](https://schemas.optimade.org/defs/v1.2/prefixes/si/deci.md)**  
**Definition name:** `deci`

**Prefix name:** deci  
**Latin symbol:** d  
**Display symbol:** d  
  
**Description:** The deci SI prefix defined as a dimensionless multiple of 10⁻¹, adopted into SI at its creation at the 11th CGPM Meeting in 1960, resolution 12.



**Resources:**

- [Definition in the 11th CGPM Meeting in 1960, resolution 12](https://www.bipm.org/en/committees/cg/cgpm/11-1960/resolution-12)
- [Wikipedia article describing the prefix](https://en.wikipedia.org/wiki/Deci-)


**Formats:** [[JSON](deci.json)] [[MD](deci.md)]

**JSON definition:**

``` json
{
    "$id": "https://schemas.optimade.org/defs/v1.2/prefixes/si/deci",
    "$schema": "https://schemas.optimade.org/meta/v1.2/optimade/prefix_definition.json",
    "title": "deci",
    "symbol": "d",
    "display-symbol": "d",
    "description": "The deci SI prefix defined as a dimensionless multiple of 10\u207b\u00b9, adopted into SI at its creation at the 11th CGPM Meeting in 1960, resolution 12.",
    "resources": [
        {
            "relation": "Definition in the 11th CGPM Meeting in 1960, resolution 12",
            "resource-id": "https://www.bipm.org/en/committees/cg/cgpm/11-1960/resolution-12"
        },
        {
            "relation": "Wikipedia article describing the prefix",
            "resource-id": "https://en.wikipedia.org/wiki/Deci-"
        }
    ],
    "defining-relation": {
        "base-units": [],
        "base-units-expression": "",
        "scale": {
            "exponent": -1
        }
    },
    "x-optimade-definition": {
        "label": "deci_prefix_si",
        "kind": "prefix",
        "format": "1.2",
        "version": "1.2.0",
        "name": "deci"
    }
}
```
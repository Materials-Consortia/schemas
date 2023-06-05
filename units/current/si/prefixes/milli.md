# milli, m (prefix)
This page documents an [OPTIMADE](https://www.optimade.org/) [Prefix Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/units/v1.2.0/si/prefixes/milli`](https://schemas.optimade.org/units/v1.2.0/si/prefixes/milli)**  
**Definition name:** `milli`

**Prefix name:** milli  
**Latin symbol:** m  
**Display symbol:** m  
  
**Description:** The milli SI prefix defined as a dimensionless multiple of 10⁻³, adopted into SI at its creation at the 11th CGPM Meeting in 1960, resolution 12.



**Resources:**

- [Definition in the 11:th CGPM Meeting in 1960, resolution 12](https://www.bipm.org/en/committees/cg/cgpm/11-1960/resolution-12)
- [Wikipedia article describing the prefix](https://en.wikipedia.org/wiki/Milli-)


**Formats:** [[JSON](milli.json)] [[MD](milli.md)]

**JSON definition:**

``` json
{
    "title": "milli",
    "symbol": "m",
    "display-symbol": "m",
    "$id": "https://schemas.optimade.org/units/v1.2.0/si/prefixes/milli",
    "description": "The milli SI prefix defined as a dimensionless multiple of 10\u207b\u00b3, adopted into SI at its creation at the 11th CGPM Meeting in 1960, resolution 12.",
    "standard": {
        "name": "gnu units",
        "version": "3.15",
        "symbol": "milli"
    },
    "resources": [
        {
            "relation": "Definition in the 11:th CGPM Meeting in 1960, resolution 12",
            "resource-id": "https://www.bipm.org/en/committees/cg/cgpm/11-1960/resolution-12"
        },
        {
            "relation": "Wikipedia article describing the prefix",
            "resource-id": "https://en.wikipedia.org/wiki/Milli-"
        }
    ],
    "defining-relation": {
        "base-units": [],
        "base-units-expression": "",
        "scale": {
            "exponent": -3
        }
    },
    "x-optimade-definition": {
        "kind": "prefix",
        "format": "1.2",
        "version": "1.2.0",
        "name": "milli"
    },
    "$schema": "https://schemas.optimade.org/meta/v1.2.0/optimade/physical_unit_definition.md"
}
```
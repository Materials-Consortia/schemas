# tera, T (prefix)
This page documents an [OPTIMADE](https://www.optimade.org/) [Prefix Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/units/v1.2.0/si/prefixes/tera`](https://schemas.optimade.org/units/v1.2.0/si/prefixes/tera)**  
**Definition name:** `tera`

**Prefix name:** tera  
**Latin symbol:** T  
**Display symbol:** T  
  
**Description:** The tera SI prefix defined as a dimensionless multiple of 10¹², adopted into SI at its creation at the 11th CGPM Meeting in 1960, resolution 12.



**Resources:**

- [Definition in the 11:th CGPM Meeting in 1960, resolution 12](https://www.bipm.org/en/committees/cg/cgpm/11-1960/resolution-12)
- [Wikipedia article describing the SI prefixes](https://en.wikipedia.org/wiki/Metric_prefix)


**Formats:** [[JSON](tera.json)] [[MD](tera.md)]

**JSON definition:**

``` json
{
    "title": "tera",
    "symbol": "T",
    "display-symbol": "T",
    "$id": "https://schemas.optimade.org/units/v1.2.0/si/prefixes/tera",
    "description": "The tera SI prefix defined as a dimensionless multiple of 10\u00b9\u00b2, adopted into SI at its creation at the 11th CGPM Meeting in 1960, resolution 12.",
    "standard": {
        "name": "gnu units",
        "version": "3.15",
        "symbol": "tera"
    },
    "resources": [
        {
            "relation": "Definition in the 11:th CGPM Meeting in 1960, resolution 12",
            "resource-id": "https://www.bipm.org/en/committees/cg/cgpm/11-1960/resolution-12"
        },
        {
            "relation": "Wikipedia article describing the SI prefixes",
            "resource-id": "https://en.wikipedia.org/wiki/Metric_prefix"
        }
    ],
    "defining-relation": {
        "base-units": [],
        "base-units-expression": "",
        "scale": {
            "exponent": 12
        }
    },
    "x-optimade-definition": {
        "kind": "prefix",
        "format": "1.2",
        "version": "1.2.0",
        "name": "tera"
    },
    "$schema": "https://schemas.optimade.org/meta/v1.2.0/optimade/physical_unit_definition.md"
}
```
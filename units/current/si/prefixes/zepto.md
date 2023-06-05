# zepto, z (prefix)
This page documents an [OPTIMADE](https://www.optimade.org/) [Prefix Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/units/v1.2.0/si/prefixes/zepto`](https://schemas.optimade.org/units/v1.2.0/si/prefixes/zepto)**  
**Definition name:** `zepto`

**Prefix name:** zepto  
**Latin symbol:** z  
**Display symbol:** z  
  
**Description:** The zepto SI prefix defined as a dimensionless multiple of 10⁻²¹, defined at the 19:th CGPM Meeting in 1991, resolution 4.



**Resources:**

- [Definition in the 19:th CGPM Meeting in 1991, resolution 4](https://www.bipm.org/en/committees/cg/cgpm/19-1991/resolution-4)
- [Wikipedia article describing SI prefixes](https://en.wikipedia.org/wiki/Metric_prefix)


**Formats:** [[JSON](zepto.json)] [[MD](zepto.md)]

**JSON definition:**

``` json
{
    "title": "zepto",
    "symbol": "z",
    "display-symbol": "z",
    "$id": "https://schemas.optimade.org/units/v1.2.0/si/prefixes/zepto",
    "description": "The zepto SI prefix defined as a dimensionless multiple of 10\u207b\u00b2\u00b9, defined at the 19:th CGPM Meeting in 1991, resolution 4.",
    "standard": {
        "name": "gnu units",
        "version": "3.15",
        "symbol": "zepto"
    },
    "resources": [
        {
            "relation": "Definition in the 19:th CGPM Meeting in 1991, resolution 4",
            "resource-id": "https://www.bipm.org/en/committees/cg/cgpm/19-1991/resolution-4"
        },
        {
            "relation": "Wikipedia article describing SI prefixes",
            "resource-id": "https://en.wikipedia.org/wiki/Metric_prefix"
        }
    ],
    "defining-relation": {
        "base-units": [],
        "base-units-expression": "",
        "scale": {
            "exponent": -21
        }
    },
    "x-optimade-definition": {
        "kind": "prefix",
        "format": "1.2",
        "version": "1.2.0",
        "name": "zepto"
    },
    "$schema": "https://schemas.optimade.org/meta/v1.2.0/optimade/physical_unit_definition.md"
}
```
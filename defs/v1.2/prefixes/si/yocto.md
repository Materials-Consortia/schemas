# yocto, y (prefix)

This page documents an [OPTIMADE](https://www.optimade.org/) [Prefix Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/defs/v1.2/prefixes/si/yocto`](https://schemas.optimade.org/defs/v1.2/prefixes/si/yocto.md)**  
**Definition name:** `yocto`

**Prefix name:** yocto  
**Latin symbol:** y  
**Display symbol:** y  
  
**Description:** The yocto SI prefix defined as a dimensionless multiple of 10⁻²⁴, defined at the 19:th CGPM Meeting in 1991, resolution 4.



**Resources:**

- [Definition in the 19:th CGPM Meeting in 1991, resolution 4](https://www.bipm.org/en/committees/cg/cgpm/19-1991/resolution-4)
- [Wikipedia article describing SI prefixes](https://en.wikipedia.org/wiki/Metric_prefix)


**Formats:** [[JSON](yocto.json)] [[MD](yocto.md)]

**JSON definition:**

``` json
{
    "$id": "https://schemas.optimade.org/defs/v1.2/prefixes/si/yocto",
    "$schema": "https://schemas.optimade.org/meta/v1.2/optimade/prefix_definition.json",
    "title": "yocto",
    "symbol": "y",
    "display-symbol": "y",
    "description": "The yocto SI prefix defined as a dimensionless multiple of 10\u207b\u00b2\u2074, defined at the 19:th CGPM Meeting in 1991, resolution 4.",
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
            "exponent": -24
        }
    },
    "x-optimade-definition": {
        "label": "yocto_prefix_si",
        "kind": "prefix",
        "format": "1.2",
        "version": "1.2.0",
        "name": "yocto"
    }
}
```
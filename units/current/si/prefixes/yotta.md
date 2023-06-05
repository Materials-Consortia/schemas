# yotta, Y (prefix)
This page documents an [OPTIMADE](https://www.optimade.org/) [Prefix Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/units/v1.2.0/si/prefixes/yotta`](https://schemas.optimade.org/units/v1.2.0/si/prefixes/yotta)**  
**Definition name:** `yotta`

**Prefix name:** yotta  
**Latin symbol:** Y  
**Display symbol:** Y  
  
**Description:** The yotta SI prefix defined as a dimensionless multiple of 10²⁴, defined at the 19:th CGPM Meeting in 1991, resolution 4.



**Resources:**

- [Definition in the 19:th CGPM Meeting in 1991, resolution 4](https://www.bipm.org/en/committees/cg/cgpm/19-1991/resolution-4)
- [Wikipedia article describing SI prefixes](https://en.wikipedia.org/wiki/Metric_prefix)


**Formats:** [[JSON](yotta.json)] [[MD](yotta.md)]

**JSON definition:**

``` json
{
    "title": "yotta",
    "symbol": "Y",
    "display-symbol": "Y",
    "$id": "https://schemas.optimade.org/units/v1.2.0/si/prefixes/yotta",
    "description": "The yotta SI prefix defined as a dimensionless multiple of 10\u00b2\u2074, defined at the 19:th CGPM Meeting in 1991, resolution 4.",
    "standard": {
        "name": "gnu units",
        "version": "3.15",
        "symbol": "yotta"
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
            "exponent": 24
        }
    },
    "x-optimade-definition": {
        "kind": "prefix",
        "format": "1.2",
        "version": "1.2.0",
        "name": "yotta"
    },
    "$schema": "https://schemas.optimade.org/meta/v1.2.0/optimade/physical_unit_definition.md"
}
```
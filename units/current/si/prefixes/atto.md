# atto, a (prefix)
This page documents an [OPTIMADE](https://www.optimade.org/) [Prefix Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/units/v1.2.0/si/prefixes/atto`](https://schemas.optimade.org/units/v1.2.0/si/prefixes/atto)**  
**Definition name:** `atto`

**Prefix name:** atto  
**Latin symbol:** a  
**Display symbol:** a  
  
**Description:** The atto SI prefix defined as a dimensionless multiple of 10⁻¹⁸, defined at the 12:th CGPM Meeting in 1964, resolution 8.



**Resources:**

- [Definition in the 12th CGPM Meeting in 1964, resolution 8](https://www.bipm.org/en/committees/cg/cgpm/12-1964/resolution-8)
- [Wikipedia article describing the SI prefixes](https://en.wikipedia.org/wiki/Metric_prefix)


**Formats:** [[JSON](atto.json)] [[MD](atto.md)]

**JSON definition:**

``` json
{
    "title": "atto",
    "symbol": "a",
    "display-symbol": "a",
    "$id": "https://schemas.optimade.org/units/v1.2.0/si/prefixes/atto",
    "description": "The atto SI prefix defined as a dimensionless multiple of 10\u207b\u00b9\u2078, defined at the 12:th CGPM Meeting in 1964, resolution 8.",
    "standard": {
        "name": "gnu units",
        "version": "3.15",
        "symbol": "atto"
    },
    "resources": [
        {
            "relation": "Definition in the 12th CGPM Meeting in 1964, resolution 8",
            "resource-id": "https://www.bipm.org/en/committees/cg/cgpm/12-1964/resolution-8"
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
            "exponent": -18
        }
    },
    "x-optimade-definition": {
        "kind": "prefix",
        "format": "1.2",
        "version": "1.2.0",
        "name": "atto"
    },
    "$schema": "https://schemas.optimade.org/meta/v1.2.0/optimade/physical_unit_definition.md"
}
```
# pico, p (prefix)
This page documents an [OPTIMADE](https://www.optimade.org/) [Prefix Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/units/v1.2.0/si/prefixes/pico`](https://schemas.optimade.org/units/v1.2.0/si/prefixes/pico)**  
**Definition name:** `pico`

**Prefix name:** pico  
**Latin symbol:** p  
**Display symbol:** p  
  
**Description:** The pico SI prefix defined as a dimensionless multiple of 10⁻¹², adopted into SI at its creation at the 11th CGPM Meeting in 1960, resolution 12.



**Resources:**

- [Definition in the 11:th CGPM Meeting in 1960, resolution 12](https://www.bipm.org/en/committees/cg/cgpm/11-1960/resolution-12)
- [Wikipedia article describing the SI prefixes](https://en.wikipedia.org/wiki/Metric_prefix)


**Formats:** [[JSON](pico.json)] [[MD](pico.md)]

**JSON definition:**

``` json
{
    "title": "pico",
    "symbol": "p",
    "display-symbol": "p",
    "$id": "https://schemas.optimade.org/units/v1.2.0/si/prefixes/pico",
    "description": "The pico SI prefix defined as a dimensionless multiple of 10\u207b\u00b9\u00b2, adopted into SI at its creation at the 11th CGPM Meeting in 1960, resolution 12.",
    "standard": {
        "name": "gnu units",
        "version": "3.15",
        "symbol": "pico"
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
            "exponent": -12
        }
    },
    "x-optimade-definition": {
        "kind": "prefix",
        "format": "1.2",
        "version": "1.2.0",
        "name": "pico"
    },
    "$schema": "https://schemas.optimade.org/meta/v1.2.0/optimade/physical_unit_definition.md"
}
```
# quecto, q (prefix)

This page documents an [OPTIMADE](https://www.optimade.org/) [Prefix Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/defs/v1.2/prefixes/si/quecto`](https://schemas.optimade.org/defs/v1.2/prefixes/si/quecto.md)**  
**Definition name:** `quecto`

**Prefix name:** quecto  
**Latin symbol:** q  
**Display symbol:** q  
  
**Description:** The quecto SI prefix defined as a dimensionless multiple of 10⁻³⁰, defined at the 27th CGPM Meeting in 2022, resolution 3.



**Resources:**

- [Definition in the 27th CGPM Meeting in 2022, resolution 3](https://www.bipm.org/en/cgpm-2022/resolution-3)
- [Wikipedia article describing SI prefixes](https://en.wikipedia.org/wiki/Metric_prefix)


**Formats:** [[JSON](quecto.json)] [[MD](quecto.md)]

**JSON definition:**

``` json
{
    "$id": "https://schemas.optimade.org/defs/v1.2/prefixes/si/quecto",
    "$schema": "https://schemas.optimade.org/meta/v1.2/optimade/prefix_definition.json",
    "title": "quecto",
    "symbol": "q",
    "display-symbol": "q",
    "description": "The quecto SI prefix defined as a dimensionless multiple of 10\u207b\u00b3\u2070, defined at the 27th CGPM Meeting in 2022, resolution 3.",
    "resources": [
        {
            "relation": "Definition in the 27th CGPM Meeting in 2022, resolution 3",
            "resource-id": "https://www.bipm.org/en/cgpm-2022/resolution-3"
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
            "exponent": -30
        }
    },
    "x-optimade-definition": {
        "label": "quecto_prefix_si",
        "kind": "prefix",
        "format": "1.2",
        "version": "1.2.0",
        "name": "quecto"
    }
}
```
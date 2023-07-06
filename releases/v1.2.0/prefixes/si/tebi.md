# tebi, Ti (prefix)

This page documents an [OPTIMADE](https://www.optimade.org/) [Prefix Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/defs/v1.2/prefixes/si/tebi`](https://schemas.optimade.org/defs/v1.2/prefixes/si/tebi)**  
**Definition name:** `tebi`

**Prefix name:** tebi  
**Latin symbol:** Ti  
**Display symbol:** Ti  
  
**Description:** The tebi prefix as a dimensionless multiple of 2⁴⁰ is one of a set of recommended prefixes in the International System of Units (SI), 9th Edition for refering to powers of 2.



**Resources:**

- [Definition in the International System of Units (SI), 9th Edition](https://www.bipm.org/en/publications/si-brochure)
- [Wikipedia article describing SI prefixes](https://en.wikipedia.org/wiki/Metric_prefix)


**Formats:** [[JSON](tebi.json)] [[MD](tebi.md)]

**JSON definition:**

``` json
{
    "$schema": "https://schemas.optimade.org/meta/v1.2/optimade/prefix_definition.md",
    "$id": "https://schemas.optimade.org/defs/v1.2/prefixes/si/tebi",
    "title": "tebi",
    "symbol": "Ti",
    "display-symbol": "Ti",
    "description": "The tebi prefix as a dimensionless multiple of 2\u2074\u2070 is one of a set of recommended prefixes in the International System of Units (SI), 9th Edition for refering to powers of 2.",
    "standard": {
        "name": "gnu units",
        "version": "3.15",
        "symbol": "tebi"
    },
    "resources": [
        {
            "relation": "Definition in the International System of Units (SI), 9th Edition",
            "resource-id": "https://www.bipm.org/en/publications/si-brochure"
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
            "base": 2,
            "nominator": 40
        }
    },
    "x-optimade-definition": {
        "kind": "prefix",
        "format": "1.2",
        "version": "1.2.0",
        "name": "tebi"
    }
}
```
# yobi, Yi (prefix)
This page documents an [OPTIMADE](https://www.optimade.org/) [Prefix Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/units/v1.2.0/si/prefixes/yobi`](https://schemas.optimade.org/units/v1.2.0/si/prefixes/yobi)**  
**Definition name:** `yobi`

**Prefix name:** yobi  
**Latin symbol:** Yi  
**Display symbol:** Yi  
  
**Description:** The yobi prefix as a dimensionless multiple of 2⁸⁰ is one of a set of recommended prefixes in the International System of Units (SI), 9th Edition for refering to powers of 2.



**Resources:**

- [Definition in the International System of Units (SI), 9th Edition](https://www.bipm.org/en/publications/si-brochure)
- [Wikipedia article describing SI prefixes](https://en.wikipedia.org/wiki/Metric_prefix)


**Formats:** [[JSON](yobi.json)] [[MD](yobi.md)]

**JSON definition:**

``` json
{
    "$id": "https://schemas.optimade.org/units/v1.2.0/si/prefixes/yobi",
    "title": "yobi",
    "symbol": "Yi",
    "display-symbol": "Yi",
    "description": "The yobi prefix as a dimensionless multiple of 2\u2078\u2070 is one of a set of recommended prefixes in the International System of Units (SI), 9th Edition for refering to powers of 2.",
    "standard": {
        "name": "gnu units",
        "version": "3.15",
        "symbol": "yobi"
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
            "nominator": 80
        }
    },
    "x-optimade-definition": {
        "kind": "prefix",
        "format": "1.2",
        "version": "1.2.0",
        "name": "yobi"
    },
    "$schema": "https://schemas.optimade.org/meta/v1.2.0/optimade/physical_unit_definition.md"
}
```
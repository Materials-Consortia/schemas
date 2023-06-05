# exbi, Ei (prefix)
This page documents an [OPTIMADE](https://www.optimade.org/) [Prefix Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/units/v1.2.0/si/prefixes/exbi`](https://schemas.optimade.org/units/v1.2.0/si/prefixes/exbi)**  
**Definition name:** `exbi`

**Prefix name:** exbi  
**Latin symbol:** Ei  
**Display symbol:** Ei  
  
**Description:** The exbi prefix as a dimensionless multiple of 2⁶⁰ is one of a set of recommended prefixes in the International System of Units (SI), 9th Edition for refering to powers of 2.



**Resources:**

- [Definition in the International System of Units (SI), 9th Edition](https://www.bipm.org/en/publications/si-brochure)
- [Wikipedia article describing SI prefixes](https://en.wikipedia.org/wiki/Metric_prefix)


**Formats:** [[JSON](exbi.json)] [[MD](exbi.md)]

**JSON definition:**

``` json
{
    "$id": "https://schemas.optimade.org/units/v1.2.0/si/prefixes/exbi",
    "title": "exbi",
    "symbol": "Ei",
    "display-symbol": "Ei",
    "description": "The exbi prefix as a dimensionless multiple of 2\u2076\u2070 is one of a set of recommended prefixes in the International System of Units (SI), 9th Edition for refering to powers of 2.",
    "standard": {
        "name": "gnu units",
        "version": "3.15",
        "symbol": "exbi"
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
            "nominator": 60
        }
    },
    "x-optimade-definition": {
        "kind": "prefix",
        "format": "1.2",
        "version": "1.2.0",
        "name": "exbi"
    },
    "$schema": "https://schemas.optimade.org/meta/v1.2.0/optimade/physical_unit_definition.md"
}
```
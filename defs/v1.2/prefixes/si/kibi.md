# kibi, Ki (prefix)

This page documents an [OPTIMADE](https://www.optimade.org/) [Prefix Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/defs/v1.2/prefixes/si/kibi`](https://schemas.optimade.org/defs/v1.2/prefixes/si/kibi.md)**  
**Definition name:** `kibi`

**Prefix name:** kibi  
**Latin symbol:** Ki  
**Display symbol:** Ki  
  
**Description:** The kibi prefix as a dimensionless multiple of 2¹⁰ = 1024 is one of a set of recommended prefixes in the International System of Units (SI), 9th Edition for referring to powers of 2.



**Resources:**

- [Definition in the International System of Units (SI), 9th Edition](https://www.bipm.org/en/publications/si-brochure)
- [Wikipedia article describing SI prefixes](https://en.wikipedia.org/wiki/Metric_prefix)


**Formats:** [[JSON](kibi.json)] [[MD](kibi.md)]

**JSON definition:**

``` json
{
    "$schema": "https://schemas.optimade.org/meta/v1.2/optimade/prefix_definition.md",
    "$id": "https://schemas.optimade.org/defs/v1.2/prefixes/si/kibi",
    "title": "kibi",
    "symbol": "Ki",
    "display-symbol": "Ki",
    "description": "The kibi prefix as a dimensionless multiple of 2\u00b9\u2070 = 1024 is one of a set of recommended prefixes in the International System of Units (SI), 9th Edition for referring to powers of 2.",
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
            "exponent": 10
        }
    },
    "x-optimade-definition": {
        "label": "kibi_prefix_si",
        "kind": "prefix",
        "format": "1.2",
        "version": "1.2.0",
        "name": "kibi"
    }
}
```
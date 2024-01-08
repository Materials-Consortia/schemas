# pebi, Ei (prefix)

This page documents an [OPTIMADE](https://www.optimade.org/) [Prefix Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/defs/v1.2/prefixes/si/pebi`](https://schemas.optimade.org/defs/v1.2/prefixes/si/pebi.md)**  
**Definition name:** `pebi`

**Prefix name:** pebi  
**Latin symbol:** Ei  
**Display symbol:** Ei  
  
**Description:** The pebi prefix as a dimensionless multiple of 2⁵⁰ is one of a set of recommended prefixes in the International System of Units (SI), 9th Edition for refering to powers of 2.



**Resources:**

- [Definition in the International System of Units (SI), 9th Edition](https://www.bipm.org/en/publications/si-brochure)
- [Wikipedia article describing SI prefixes](https://en.wikipedia.org/wiki/Metric_prefix)


**Formats:** [[JSON](pebi.json)] [[MD](pebi.md)]

**JSON definition:**

``` json
{
    "$schema": "https://schemas.optimade.org/meta/v1.2/optimade/prefix_definition.md",
    "$id": "https://schemas.optimade.org/defs/v1.2/prefixes/si/pebi",
    "title": "pebi",
    "symbol": "Ei",
    "display-symbol": "Ei",
    "description": "The pebi prefix as a dimensionless multiple of 2\u2075\u2070 is one of a set of recommended prefixes in the International System of Units (SI), 9th Edition for refering to powers of 2.",
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
            "numerator": 50
        }
    },
    "x-optimade-definition": {
        "label": "pebi_prefix_si",
        "kind": "prefix",
        "format": "1.2",
        "version": "1.2.0",
        "name": "pebi"
    }
}
```
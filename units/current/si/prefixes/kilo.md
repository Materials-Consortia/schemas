# kilo, k (prefix)
This page documents an [OPTIMADE](https://www.optimade.org/) [Prefix Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/units/v1.2.0/si/prefixes/kilo`](https://schemas.optimade.org/units/v1.2.0/si/prefixes/kilo)**  
**Definition name:** `kilo`

**Prefix name:** kilo  
**Latin symbol:** k  
**Display symbol:** k  
  
**Description:** The kilo SI prefix defined as a dimensionless multiple of 10³, adopted into SI at its creation at the 11th CGPM Meeting in 1960, resolution 12.



**Resources:**

- [Definition in the 11:th CGPM Meeting in 1960, resolution 12](https://www.bipm.org/en/committees/cg/cgpm/11-1960/resolution-12)
- [Wikipedia article describing the prefix](https://en.wikipedia.org/wiki/Kilo-)


**Formats:** [[JSON](kilo.json)] [[MD](kilo.md)]

**JSON definition:**

``` json
{
    "title": "kilo",
    "symbol": "k",
    "display-symbol": "k",
    "$id": "https://schemas.optimade.org/units/v1.2.0/si/prefixes/kilo",
    "description": "The kilo SI prefix defined as a dimensionless multiple of 10\u00b3, adopted into SI at its creation at the 11th CGPM Meeting in 1960, resolution 12.",
    "standard": {
        "name": "gnu units",
        "version": "3.15",
        "symbol": "kilo"
    },
    "resources": [
        {
            "relation": "Definition in the 11:th CGPM Meeting in 1960, resolution 12",
            "resource-id": "https://www.bipm.org/en/committees/cg/cgpm/11-1960/resolution-12"
        },
        {
            "relation": "Wikipedia article describing the prefix",
            "resource-id": "https://en.wikipedia.org/wiki/Kilo-"
        }
    ],
    "defining-relation": {
        "base-units": [],
        "base-units-expression": "",
        "scale": {
            "exponent": 3
        }
    },
    "x-optimade-definition": {
        "kind": "prefix",
        "format": "1.2",
        "version": "1.2.0",
        "name": "kilo"
    },
    "$schema": "https://schemas.optimade.org/meta/v1.2.0/optimade/physical_unit_definition.md"
}
```
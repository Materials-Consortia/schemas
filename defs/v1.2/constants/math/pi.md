# pi, π (constant)

This page documents an [OPTIMADE](https://www.optimade.org/) [Constant Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/defs/v1.2/constants/math/pi`](https://schemas.optimade.org/defs/v1.2/constants/math/pi)**  
**Definition name:** `pi`

**Constant name:** pi  
**Latin symbol:** pi  
**Display symbol:** π  
  
**Description:** The ratio of a circle's circumference to its diameter. Approximately equal to 3.1415926.

An early definition of π as the symbol for the ratio of a circle's circumference to its diameter goes back to William Jones, Synopsis Palmariorum Matheseos (1706), page 263.

**Resources:**

- [Definition in William Jones, Synopsis Palmariorum Matheseos (1706)](https://archive.org/details/SynopsisPalmariorumMatheseosOrANewIntroductionToTheMathematics/page/n283/)
- [Wikipedia article describing the constant](https://en.wikipedia.org/wiki/Pi)


**Formats:** [[JSON](pi.json)] [[MD](pi.md)]

**JSON definition:**

``` json
{
    "$schema": "https://schemas.optimade.org/meta/v1.2/optimade/constant_definition.md",
    "$id": "https://schemas.optimade.org/defs/v1.2/constants/math/pi",
    "title": "pi",
    "symbol": "pi",
    "display-symbol": "\u03c0",
    "description": "The ratio of a circle's circumference to its diameter. Approximately equal to 3.1415926.\n\nAn early definition of \u03c0 as the symbol for the ratio of a circle's circumference to its diameter goes back to William Jones, Synopsis Palmariorum Matheseos (1706), page 263.",
    "standard": {
        "name": "gnu units",
        "version": "3.15",
        "symbol": "pi"
    },
    "resources": [
        {
            "relation": "Definition in William Jones, Synopsis Palmariorum Matheseos (1706)",
            "resource-id": "https://archive.org/details/SynopsisPalmariorumMatheseosOrANewIntroductionToTheMathematics/page/n283/"
        },
        {
            "relation": "Wikipedia article describing the constant",
            "resource-id": "https://en.wikipedia.org/wiki/Pi"
        }
    ],
    "approximate-relations": [
        {
            "value": 3.141592653589793
        }
    ],
    "x-optimade-definition": {
        "kind": "constant",
        "format": "1.2",
        "version": "1.2.0",
        "name": "pi"
    }
}
```
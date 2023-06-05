# bit, bit (unit)
This page documents an [OPTIMADE](https://www.optimade.org/) [Unit Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/units/v1.2.0/independent/1948/information/bit`](https://schemas.optimade.org/units/v1.2.0/independent/1948/information/bit)**  
**Definition name:** `bit`

**Unit name:** bit  
**Latin symbol:** bit  
**Display symbol:** bit  
  
**Description:** A basic unit of digital information representing a single logical state with one of two possible values, defined by Shannon in 1948.

"If the base 2 is used the resulting units may be called binary digits, or more briefly bits, a word suggested by J. W. Tukey. A device with two stable positions, such as a relay or a flip-flop circuit, can store one bit of information." ["A Mathematical Theory of Communication", C. E. Shannon, The Bell System Technical Journal 27, 379 (1948)].

**Resources:**

- [Defining paper: "A Mathematical Theory of Communication" by C. E. Shannon, The Bell System Technical Journal, Vol. 27, pp. 379–423 (1948).](https://doi.org/10.1002/j.1538-7305.1948.tb01338.x)
- [Wikipedia article describing the unit](https://en.wikipedia.org/wiki/Bit)


**Formats:** [[JSON](bit.json)] [[MD](bit.md)]

**JSON definition:**

``` json
{
    "$id": "https://schemas.optimade.org/units/v1.2.0/independent/1948/information/bit",
    "title": "bit",
    "symbol": "bit",
    "display-symbol": "bit",
    "description": "A basic unit of digital information representing a single logical state with one of two possible values, defined by Shannon in 1948.\n\n\"If the base 2 is used the resulting units may be called binary digits, or more briefly bits, a word suggested by J. W. Tukey. A device with two stable positions, such as a relay or a flip-flop circuit, can store one bit of information.\" [\"A Mathematical Theory of Communication\", C. E. Shannon, The Bell System Technical Journal 27, 379 (1948)].",
    "standard": {
        "name": "gnu units",
        "version": "3.15",
        "symbol": "bit"
    },
    "resources": [
        {
            "relation": "Defining paper: \"A Mathematical Theory of Communication\" by C. E. Shannon, The Bell System Technical Journal, Vol. 27, pp. 379\u2013423 (1948).",
            "resource-id": "https://doi.org/10.1002/j.1538-7305.1948.tb01338.x"
        },
        {
            "relation": "Wikipedia article describing the unit",
            "resource-id": "https://en.wikipedia.org/wiki/Bit"
        }
    ],
    "x-optimade-definition": {
        "kind": "unit",
        "format": "1.2",
        "version": "1.2.0",
        "name": "bit"
    },
    "$schema": "https://schemas.optimade.org/meta/v1.2.0/optimade/physical_unit_definition.md"
}
```
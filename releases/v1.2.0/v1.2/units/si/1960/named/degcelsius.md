# degree Celsius, °C (unit)

This page documents an [OPTIMADE](https://www.optimade.org/) [Unit Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/defs/v1.2/units/si/1960/named/degcelsius`](https://schemas.optimade.org/defs/v1.2/units/si/1960/named/degcelsius.md)**  
**Definition name:** `degcelsius`

**Unit name:** degree Celsius  
**Latin symbol:** degC  
**Display symbol:** °C  
  
**Description:** A derived SI unit of temperature, defined as degree kelvin offset with +273.15 in the SI base units adopted at the 11th CGPM Meeting in 1960.

"If we add to the practical international Celsius temperatures defined above T₀ = 273.15 degrees, we obtain the practical international Kelvin temperatures. By subtracting T₀ from the thermodynamic temperatures, we obtain the thermodynamic Celsius temperatures." [11th CGPM meeting (1960)]

**Resources:**

- [Wikipedia article describing the unit](https://en.wikipedia.org/wiki/Celsius)


**Formats:** [[JSON](degcelsius.json)] [[MD](degcelsius.md)]

**JSON definition:**

``` json
{
    "$id": "https://schemas.optimade.org/defs/v1.2/units/si/1960/named/degcelsius",
    "$schema": "https://schemas.optimade.org/meta/v1.2/optimade/physical_unit_definition.json",
    "title": "degree Celsius",
    "symbol": "degC",
    "display-symbol": "\u00b0C",
    "alternate-symbols": [
        "degreecelsius"
    ],
    "description": "A derived SI unit of temperature, defined as degree kelvin offset with +273.15 in the SI base units adopted at the 11th CGPM Meeting in 1960.\n\n\"If we add to the practical international Celsius temperatures defined above T\u2080 = 273.15 degrees, we obtain the practical international Kelvin temperatures. By subtracting T\u2080 from the thermodynamic temperatures, we obtain the thermodynamic Celsius temperatures.\" [11th CGPM meeting (1960)]",
    "resources": [
        {
            "relation": "Wikipedia article describing the unit",
            "resource-id": "https://en.wikipedia.org/wiki/Celsius"
        }
    ],
    "defining-relation": {
        "base-units": [
            {
                "symbol": "degK",
                "id": "https://schemas.optimade.org/defs/v1.2/units/si/1960/base/degreekelvin"
            }
        ],
        "base-units-expression": "degK",
        "offset": {
            "numerator": 27315,
            "denominator": 100
        }
    },
    "standard": {
        "name": "si",
        "year": 1960,
        "category": "named",
        "symbol": "degC"
    },
    "x-optimade-definition": {
        "label": "degcelsius_si_1960_named",
        "kind": "unit",
        "format": "1.2",
        "version": "1.2.0",
        "name": "degcelsius"
    }
}
```
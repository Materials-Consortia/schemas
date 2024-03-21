# degree Celsius, °C (unit)

This page documents an [OPTIMADE](https://www.optimade.org/) [Unit Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/defs/v1.2/units/si/general/degcelsius`](https://schemas.optimade.org/defs/v1.2/units/si/general/degcelsius.md)**  
**Definition name:** `degcelsius`

**Unit name:** degree Celsius  
**Latin symbol:** degC  
**Display symbol:** °C  
  
**Description:** A unit of temperature, defined as kelvin offset with +273.15 using the current, or one of the historical, definitions of the SI units.

"If we add to the practical international Celsius temperatures defined above T₀ = 273.15 degrees, we obtain the practical international Kelvin temperatures. By subtracting T₀ from the thermodynamic temperatures, we obtain the thermodynamic Celsius temperatures." [11th CGPM meeting (1960)]

The degree Celsius was defined and included in SI at the 11th CGPM meeting in 1960, resolution 12 and implicitly redefined via the redefinitions of the kelvin at the 13th CGPM Meeting in 1967, resolution 4 and at the 26th CGPM Meeting (2018), resolution 1.

This is a generalized definition taken to reference the current, or one of the historical, SI unit definitions.
This definition is intended for situations when it is not possible to be more precise, e.g., in contexts where data have been collected that uses different historical SI definitions.

**Resources:**

- [Definition at the 11th CGPM meeting (1960)](https://www.bipm.og/en/committees/cg/cgpm/11-1960)
- [Redefinition of the kelvin at the 13th CGPM meeting (1967), resolution 4](https://www.bipm.org/en/committees/cg/cgpm/13-1967/resolution-4)
- [Redefinition of the kelvin at the 26th CGPM meeting (2018), resolution 1](https://www.bipm.org/en/committees/cg/cgpm/26-2018/resolution-1)
- [Wikipedia article describing the unit](https://en.wikipedia.org/wiki/Celsius)


**Compatibility:** (other definitions that are covered by the above definition)

- [`https://schemas.optimade.org/defs/v1.2/units/si/1960/named/degcelsius`](https://schemas.optimade.org/defs/v1.2/units/si/1960/named/degcelsius.md)
- [`https://schemas.optimade.org/defs/v1.2/units/si/1967/named/degcelsius`](https://schemas.optimade.org/defs/v1.2/units/si/1967/named/degcelsius.md)
- [`https://schemas.optimade.org/defs/v1.2/units/si/2019/named/degcelsius`](https://schemas.optimade.org/defs/v1.2/units/si/2019/named/degcelsius.md)


**Formats:** [[JSON](degcelsius.json)] [[MD](degcelsius.md)]

**JSON definition:**

``` json
{
    "$id": "https://schemas.optimade.org/defs/v1.2/units/si/general/degcelsius",
    "$schema": "https://schemas.optimade.org/meta/v1.2/optimade/physical_unit_definition.json",
    "title": "degree Celsius",
    "symbol": "degC",
    "display-symbol": "\u00b0C",
    "alternate-symbols": [
        "degreecelsius"
    ],
    "description": "A unit of temperature, defined as kelvin offset with +273.15 using the current, or one of the historical, definitions of the SI units.\n\n\"If we add to the practical international Celsius temperatures defined above T\u2080 = 273.15 degrees, we obtain the practical international Kelvin temperatures. By subtracting T\u2080 from the thermodynamic temperatures, we obtain the thermodynamic Celsius temperatures.\" [11th CGPM meeting (1960)]\n\nThe degree Celsius was defined and included in SI at the 11th CGPM meeting in 1960, resolution 12 and implicitly redefined via the redefinitions of the kelvin at the 13th CGPM Meeting in 1967, resolution 4 and at the 26th CGPM Meeting (2018), resolution 1.\n\nThis is a generalized definition taken to reference the current, or one of the historical, SI unit definitions.\nThis definition is intended for situations when it is not possible to be more precise, e.g., in contexts where data have been collected that uses different historical SI definitions.",
    "compatibility": [
        "https://schemas.optimade.org/defs/v1.2/units/si/1960/named/degcelsius",
        "https://schemas.optimade.org/defs/v1.2/units/si/1967/named/degcelsius",
        "https://schemas.optimade.org/defs/v1.2/units/si/2019/named/degcelsius"
    ],
    "resources": [
        {
            "relation": "Definition at the 11th CGPM meeting (1960)",
            "resource-id": "https://www.bipm.og/en/committees/cg/cgpm/11-1960"
        },
        {
            "relation": "Redefinition of the kelvin at the 13th CGPM meeting (1967), resolution 4",
            "resource-id": "https://www.bipm.org/en/committees/cg/cgpm/13-1967/resolution-4"
        },
        {
            "relation": "Redefinition of the kelvin at the 26th CGPM meeting (2018), resolution 1",
            "resource-id": "https://www.bipm.org/en/committees/cg/cgpm/26-2018/resolution-1"
        },
        {
            "relation": "Wikipedia article describing the unit",
            "resource-id": "https://en.wikipedia.org/wiki/Celsius"
        }
    ],
    "defining-relation": {
        "base-units": [
            {
                "symbol": "K",
                "id": "https://schemas.optimade.org/defs/v1.2/units/si/general/kelvin"
            }
        ],
        "base-units-expression": "K",
        "offset": {
            "numerator": 27315,
            "denominator": 100
        }
    },
    "x-optimade-definition": {
        "label": "degcelsius_si_general",
        "kind": "unit",
        "format": "1.2",
        "version": "1.2.0",
        "name": "degcelsius"
    }
}
```
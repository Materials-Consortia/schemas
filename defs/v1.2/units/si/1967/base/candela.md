# candela, cd (unit)

This page documents an [OPTIMADE](https://www.optimade.org/) [Unit Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/defs/v1.2/units/si/1967/base/candela`](https://schemas.optimade.org/defs/v1.2/units/si/1967/base/candela.md)**  
**Definition name:** `candela`

**Unit name:** candela  
**Latin symbol:** cd  
**Display symbol:** cd  
  
**Description:** The candela is the SI base unit of luminous intensity in a given direction defined in from the radiation of a black body at the temperature of freezing platinum as defined at the 9th CGPM meeting in 1948, clarifed at the 13th CGPM Meeting in 1967, resolution 5; and implicitly redefined due to the 1967 SI redefinition of the second.

At the 13th CGPM Meeting in 1967, resolution 5 the previous definition from the 9th CGPM meeting in 1948 was rephrased to be more clear: "The candela is the luminous intensity, in the perpendicular direction, of a surface of 1/600000 square metre of a black body at the temperature of freezing platinum under a pressure of 101325 newtons per square metre."

Furthermore, the SI 1967 definition of the candela references:

- the SI 1960 metre (https://schemas.optimade.org/units/v1.2/si/1960/base/metre).
- the SI 1967 derived newton unit (https://schemas.optimade.org/units/v1.2/si/1967/named/newton) equal to kilogram·metre·second⁻², referencing the SI 1960 kilogram (https://schemas.optimade.org/units/v1.2/si/1960/base/kilogram) and metre (https://schemas.optimade.org/units/v1.2/si/1960/base/metre); and the 1967 definition of the second (https://schemas.optimade.org/units/v1.2/si/1967/base/second).

**Resources:**

- [Definition at the 13st CGPM meeting (1967)](https://www.bipm.org/en/committees/cg/cgpm/13-1967/resolution-5)
- [Previous definition at the 9st CGPM meeting (1948)](https://www.bipm.org/en/committees/cg/cgpm/9-1948)
- [Wikipedia article describing the unit](https://en.wikipedia.org/wiki/Candela)


**Formats:** [[JSON](candela.json)] [[MD](candela.md)]

**JSON definition:**

``` json
{
    "$schema": "https://schemas.optimade.org/meta/v1.2/optimade/physical_unit_definition.md",
    "$id": "https://schemas.optimade.org/defs/v1.2/units/si/1967/base/candela",
    "title": "candela",
    "symbol": "cd",
    "display-symbol": "cd",
    "description": "The candela is the SI base unit of luminous intensity in a given direction defined in from the radiation of a black body at the temperature of freezing platinum as defined at the 9th CGPM meeting in 1948, clarifed at the 13th CGPM Meeting in 1967, resolution 5; and implicitly redefined due to the 1967 SI redefinition of the second.\n\nAt the 13th CGPM Meeting in 1967, resolution 5 the previous definition from the 9th CGPM meeting in 1948 was rephrased to be more clear: \"The candela is the luminous intensity, in the perpendicular direction, of a surface of 1/600000 square metre of a black body at the temperature of freezing platinum under a pressure of 101325 newtons per square metre.\"\n\nFurthermore, the SI 1967 definition of the candela references:\n\n- the SI 1960 metre (https://schemas.optimade.org/units/v1.2/si/1960/base/metre).\n- the SI 1967 derived newton unit (https://schemas.optimade.org/units/v1.2/si/1967/named/newton) equal to kilogram\u00b7metre\u00b7second\u207b\u00b2, referencing the SI 1960 kilogram (https://schemas.optimade.org/units/v1.2/si/1960/base/kilogram) and metre (https://schemas.optimade.org/units/v1.2/si/1960/base/metre); and the 1967 definition of the second (https://schemas.optimade.org/units/v1.2/si/1967/base/second).",
    "resources": [
        {
            "relation": "Definition at the 13st CGPM meeting (1967)",
            "resource-id": "https://www.bipm.org/en/committees/cg/cgpm/13-1967/resolution-5"
        },
        {
            "relation": "Previous definition at the 9st CGPM meeting (1948)",
            "resource-id": "https://www.bipm.org/en/committees/cg/cgpm/9-1948"
        },
        {
            "relation": "Wikipedia article describing the unit",
            "resource-id": "https://en.wikipedia.org/wiki/Candela"
        }
    ],
    "standard": {
        "name": "si",
        "year": 1967,
        "category": "base",
        "symbol": "cd"
    },
    "x-optimade-definition": {
        "label": "candela_si_1967_base",
        "kind": "unit",
        "format": "1.2",
        "version": "1.2.0",
        "name": "candela"
    }
}
```
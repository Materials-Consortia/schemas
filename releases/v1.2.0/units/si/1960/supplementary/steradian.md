# steradian, sr (unit)

This page documents an [OPTIMADE](https://www.optimade.org/) [Unit Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/defs/v1.2/units/si/1960/supplementary/steradian`](https://schemas.optimade.org/defs/v1.2/units/si/1960/supplementary/steradian)**  
**Definition name:** `steradian`

**Unit name:** steradian  
**Latin symbol:** sr  
**Display symbol:** sr  
  
**Description:** A supplementary SI unit of solid angle defined from the relation of the area cut out on a sphere at a given radius so that the entire sphere has a solid angle of 4π steradians, defined at the 9th CGPM Meeting in 1948 and included into SI at the 11th CGPM Meeting in 1960.

The radian is defined at the 9th CGPM Meeting in 1948 as: "The unit of solid angle is the steradian. The steradian is the solid angle with its vertex at the center of a sphere with a radius of one meter, which cuts out an area of one square meter on the surface of that sphere."

The International System of Units (SI), 9th Edition give a rephrased but equivalent definition: "The solid angle, expressed in steradian, corresponds to the ratio between an area \(A\) of the surface of a sphere of radius \(r\) and the squared radius, \(\Omega = A/r^2\) sr. One steradian corresponds to the solid angle for which \(A = r^2\), thus 1 sr = 1."

The steradian is categorized in the International System of Units (SI), 1st Edition as a supplementary SI unit.
At the 20th CGPM meeting in 1995, resolution 8 the categorization was changed to a dimensionless derived SI unit.

**Resources:**

- [Definition at the 9st CGPM meeting (1948)](https://www.bipm.org/en/committees/cg/cgpm/9-1948)
- [Establishment of the SI unit system at the 11th CGPM meeting (1960), resolution 12.](https://www.bipm.org/en/committees/cg/cgpm/11-1960/resolution-12)
- [Reclassification at the 20th CGPM meeting (1995)](https://www.bipm.org/en/committees/cg/cgpm/20-1995/resolution-8)
- [Wikipedia article describing the unit](https://en.wikipedia.org/wiki/Radian)


**Formats:** [[JSON](steradian.json)] [[MD](steradian.md)]

**JSON definition:**

``` json
{
    "$schema": "https://schemas.optimade.org/meta/v1.2/optimade/physical_unit_definition.md",
    "$id": "https://schemas.optimade.org/defs/v1.2/units/si/1960/supplementary/steradian",
    "title": "steradian",
    "symbol": "sr",
    "display-symbol": "sr",
    "alternate-symbols": [
        "sterad"
    ],
    "description": "A supplementary SI unit of solid angle defined from the relation of the area cut out on a sphere at a given radius so that the entire sphere has a solid angle of 4\u03c0 steradians, defined at the 9th CGPM Meeting in 1948 and included into SI at the 11th CGPM Meeting in 1960.\n\nThe radian is defined at the 9th CGPM Meeting in 1948 as: \"The unit of solid angle is the steradian. The steradian is the solid angle with its vertex at the center of a sphere with a radius of one meter, which cuts out an area of one square meter on the surface of that sphere.\"\n\nThe International System of Units (SI), 9th Edition give a rephrased but equivalent definition: \"The solid angle, expressed in steradian, corresponds to the ratio between an area \\(A\\) of the surface of a sphere of radius \\(r\\) and the squared radius, \\(\\Omega = A/r^2\\) sr. One steradian corresponds to the solid angle for which \\(A = r^2\\), thus 1 sr = 1.\"\n\nThe steradian is categorized in the International System of Units (SI), 1st Edition as a supplementary SI unit.\nAt the 20th CGPM meeting in 1995, resolution 8 the categorization was changed to a dimensionless derived SI unit.",
    "standard": {
        "name": "gnu units",
        "version": "3.15",
        "symbol": "sr"
    },
    "resources": [
        {
            "relation": "Definition at the 9st CGPM meeting (1948)",
            "resource-id": "https://www.bipm.org/en/committees/cg/cgpm/9-1948"
        },
        {
            "relation": "Establishment of the SI unit system at the 11th CGPM meeting (1960), resolution 12.",
            "resource-id": "https://www.bipm.org/en/committees/cg/cgpm/11-1960/resolution-12"
        },
        {
            "relation": "Reclassification at the 20th CGPM meeting (1995)",
            "resource-id": "https://www.bipm.org/en/committees/cg/cgpm/20-1995/resolution-8"
        },
        {
            "relation": "Wikipedia article describing the unit",
            "resource-id": "https://en.wikipedia.org/wiki/Radian"
        }
    ],
    "x-optimade-definition": {
        "kind": "unit",
        "format": "1.2",
        "version": "1.2.0",
        "name": "steradian"
    }
}
```
# ångström, Å (unit)

This page documents an [OPTIMADE](https://www.optimade.org/) [Unit Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/defs/v1.2/units/si/1970/temporary/angstrom`](https://schemas.optimade.org/defs/v1.2/units/si/1970/temporary/angstrom.md)**  
**Definition name:** `angstrom`

**Unit name:** ångström  
**Latin symbol:** angstrom  
**Display symbol:** Å  
  
**Description:** A length equal to 10⁻¹⁰ meter, with meter defined according to the 1960 SI base units.

The ångström appear in the International System of Units (SI), 1st ed. (1970) defined as "1 Å = 0.1 nm = 10⁻¹⁰ m".

- The International System of Units (SI), 1st ed. (1970) categorizes the unit as "temporarily admitted" for use with the SI units.
- The International System of Units (SI), 7th ed. (1998) changes the categorisation to "Other non-SI units currently accepted for use with the International System."
- The International System of Units (SI), 8th ed. (2006) changes the categorization to "Other non-SI units" and adds as a clarifying footnote "The ångström is widely used by x-ray crystallographers and structural chemists because all chemical bonds lie in the range 1 to 3 ångströms. However it has no official sanction from the CIPM or the CGPM."
- The ångström is omitted in the International System of Units (SI), 9th Edition (2019).

**Resources:**

- [Definition in the International System of Units (SI), 1th Edition](https://www.bipm.org/en/publications/si-brochure)
- [Wikipedia article describing the unit](https://en.wikipedia.org/wiki/Angstrom)


**Formats:** [[JSON](angstrom.json)] [[MD](angstrom.md)]

**JSON definition:**

``` json
{
    "$id": "https://schemas.optimade.org/defs/v1.2/units/si/1970/temporary/angstrom",
    "$schema": "https://schemas.optimade.org/meta/v1.2/optimade/physical_unit_definition.json",
    "title": "\u00e5ngstr\u00f6m",
    "symbol": "angstrom",
    "display-symbol": "\u00c5",
    "description": "A length equal to 10\u207b\u00b9\u2070 meter, with meter defined according to the 1960 SI base units.\n\nThe \u00e5ngstr\u00f6m appear in the International System of Units (SI), 1st ed. (1970) defined as \"1 \u00c5 = 0.1 nm = 10\u207b\u00b9\u2070 m\".\n\n- The International System of Units (SI), 1st ed. (1970) categorizes the unit as \"temporarily admitted\" for use with the SI units.\n- The International System of Units (SI), 7th ed. (1998) changes the categorisation to \"Other non-SI units currently accepted for use with the International System.\"\n- The International System of Units (SI), 8th ed. (2006) changes the categorization to \"Other non-SI units\" and adds as a clarifying footnote \"The \u00e5ngstr\u00f6m is widely used by x-ray crystallographers and structural chemists because all chemical bonds lie in the range 1 to 3 \u00e5ngstr\u00f6ms. However it has no official sanction from the CIPM or the CGPM.\"\n- The \u00e5ngstr\u00f6m is omitted in the International System of Units (SI), 9th Edition (2019).",
    "resources": [
        {
            "relation": "Definition in the International System of Units (SI), 1th Edition",
            "resource-id": "https://www.bipm.org/en/publications/si-brochure"
        },
        {
            "relation": "Wikipedia article describing the unit",
            "resource-id": "https://en.wikipedia.org/wiki/Angstrom"
        }
    ],
    "defining-relation": {
        "base-units": [
            {
                "symbol": "m",
                "id": "https://schemas.optimade.org/defs/v1.2/units/si/1960/base/metre"
            }
        ],
        "base-units-expression": "m",
        "scale": {
            "exponent": -10
        }
    },
    "x-optimade-definition": {
        "label": "angstrom_si_1970_temporary",
        "kind": "unit",
        "format": "1.2",
        "version": "1.2.0",
        "name": "angstrom"
    }
}
```
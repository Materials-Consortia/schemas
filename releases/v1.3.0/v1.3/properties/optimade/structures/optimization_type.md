# optimization type (property)

This page documents an [OPTIMADE](https://www.optimade.org/) [Property Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/defs/v1.3/properties/optimade/structures/optimization_type`](https://schemas.optimade.org/defs/v1.3/properties/optimade/structures/optimization_type.md)**  
**Definition name:** `optimization_type`

**Property name:** optimization type  
**Description:** A string that classifies the type of optimization that has resulted in the structural data.  
**Type:** string  

**Requirements/Conventions**:

* If the property is `null` or omitted, no information is provided about the type of optimization used to obtain the structural data.

* If present and not `null`, the property SHOULD take one of the following values:

    * `experimental`: the structure results from an optimization or refinement process part of an experimental technique, e.g., minimization of the discrepancy between observed and predicted scattered amplitudes from diffraction data.

    * `hybrid`: the structure is the result of the combination of an experiment and further optimization based on a reasonable theoretical energy model so that it remains a fair representation of the original experimental structure.
    For example, experimental structures relaxed using *ab initio* calculations are in this category.
    Structures where the experimental coordinates are kept, but one or more elements are substituted for other elements, are not included in this category.

    * `global`: the structure has been optimized using a theoretical technique based on a reasonable energy model in a way that takes into account the global energy surface.
    The structure has been optimized into the global energy minimum or into a local minimum within an energy range of the global minimum commonly considered for potential metastability (typically on the scale of 100 meV/atom).
    A common technique for this type of optimization is to construct the convex hull of thermodynamical stability from the known minima and dismiss structures outside the relevant energy range.

    * `local`: the structure has been optimized using a theoretical technique based on a reasonable energy model into a local minimum of the energy surface.
    For example, structures relaxed using *ab initio* calculations without consideration of the energy of other minima in configuration space qualify for this category.

    * `none`: the structure has not undergone an optimization process and is thus, in some sense, arbitrary.
    Structures of this kind can come from, e.g., randomly generated coordinates or non-equilibrium snapshots.

    * `indeterminate`: the database declares that the type of optimization used for this specific entry cannot be determined, e.g., because that information is missing.
    This value represents a stronger statement (that the database knows that the type of optimization is not known) than an omitted classification (i.e., the field is missing or has the value `null`) which communicates that the property is unknown only in the sense discussed in the section `Properties with an unknown value`.)

    * `other`: the structure is the result of some optimization process, but none of the other categories correctly represents the type of optimization used.

Other strings prefixed by a database-specific prefix, e.g., `_exmpl_optimized_on_fixed_grid`, SHOULD NOT be used.
Other non-standard strings MUST NOT be used.
Clients encountering unrecognized strings SHOULD treat them to mean the same as the field having the value `"other"`.

Structures produced by AI models and other techniques that have been reasonably tested to reliably generate results equivalent to structural optimization using energy models SHOULD be classified the same as if that type of energy model had been used.

**Explained examples**:

- For a structure entry directly encoding structural information obtained from a neutron diffraction experiment: `"experimental"`.

- For a structure entry that encodes the structural information from a theoretical relaxation of an `"experimental"` entry using computational software that implements density functional theory: `"hybrid"`.

**Examples:**

- `"experimental"`
- `"hybrid"`

**Formats:** [[JSON](optimization_type.json)] [[MD](optimization_type.md)]

**JSON definition:**

``` json
{
    "$id": "https://schemas.optimade.org/defs/v1.3/properties/optimade/structures/optimization_type",
    "$schema": "https://schemas.optimade.org/meta/v1.2/optimade/property_definition.json",
    "title": "optimization type",
    "x-optimade-type": "string",
    "x-optimade-definition": {
        "label": "optimization_type_optimade_structures",
        "kind": "property",
        "version": "1.3.0",
        "format": "1.2",
        "name": "optimization_type"
    },
    "type": [
        "string",
        "null"
    ],
    "description": "A string that classifies the type of optimization that has resulted in the structural data.\n\n**Requirements/Conventions**:\n\n* If the property is `null` or omitted, no information is provided about the type of optimization used to obtain the structural data.\n\n* If present and not `null`, the property SHOULD take one of the following values:\n\n    * `experimental`: the structure results from an optimization or refinement process part of an experimental technique, e.g., minimization of the discrepancy between observed and predicted scattered amplitudes from diffraction data.\n\n    * `hybrid`: the structure is the result of the combination of an experiment and further optimization based on a reasonable theoretical energy model so that it remains a fair representation of the original experimental structure.\n    For example, experimental structures relaxed using *ab initio* calculations are in this category.\n    Structures where the experimental coordinates are kept, but one or more elements are substituted for other elements, are not included in this category.\n\n    * `global`: the structure has been optimized using a theoretical technique based on a reasonable energy model in a way that takes into account the global energy surface.\n    The structure has been optimized into the global energy minimum or into a local minimum within an energy range of the global minimum commonly considered for potential metastability (typically on the scale of 100 meV/atom).\n    A common technique for this type of optimization is to construct the convex hull of thermodynamical stability from the known minima and dismiss structures outside the relevant energy range.\n\n    * `local`: the structure has been optimized using a theoretical technique based on a reasonable energy model into a local minimum of the energy surface.\n    For example, structures relaxed using *ab initio* calculations without consideration of the energy of other minima in configuration space qualify for this category.\n\n    * `none`: the structure has not undergone an optimization process and is thus, in some sense, arbitrary.\n    Structures of this kind can come from, e.g., randomly generated coordinates or non-equilibrium snapshots.\n\n    * `indeterminate`: the database declares that the type of optimization used for this specific entry cannot be determined, e.g., because that information is missing.\n    This value represents a stronger statement (that the database knows that the type of optimization is not known) than an omitted classification (i.e., the field is missing or has the value `null`) which communicates that the property is unknown only in the sense discussed in the section `Properties with an unknown value`.)\n\n    * `other`: the structure is the result of some optimization process, but none of the other categories correctly represents the type of optimization used.\n\nOther strings prefixed by a database-specific prefix, e.g., `_exmpl_optimized_on_fixed_grid`, SHOULD NOT be used.\nOther non-standard strings MUST NOT be used.\nClients encountering unrecognized strings SHOULD treat them to mean the same as the field having the value `\"other\"`.\n\nStructures produced by AI models and other techniques that have been reasonably tested to reliably generate results equivalent to structural optimization using energy models SHOULD be classified the same as if that type of energy model had been used.\n\n**Explained examples**:\n\n- For a structure entry directly encoding structural information obtained from a neutron diffraction experiment: `\"experimental\"`.\n\n- For a structure entry that encodes the structural information from a theoretical relaxation of an `\"experimental\"` entry using computational software that implements density functional theory: `\"hybrid\"`.",
    "examples": [
        "experimental",
        "hybrid"
    ],
    "x-optimade-unit": "inapplicable",
    "enum": [
        "experimental",
        "hybrid",
        "global",
        "local",
        "none",
        "indeterminate",
        "other"
    ]
}
```
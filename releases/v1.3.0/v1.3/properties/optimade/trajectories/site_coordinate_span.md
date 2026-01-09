# list of site coordinate span (property)

This page documents an [OPTIMADE](https://www.optimade.org/) [Property Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/defs/v1.3/properties/optimade/trajectories/site_coordinate_span`](https://schemas.optimade.org/defs/v1.3/properties/optimade/trajectories/site_coordinate_span.md)**  
**Definition name:** `site_coordinate_span`

**Property name:** list of site coordinate span  
**Description:** A list of site_coordinate_span items.
A site_coordinate_span item indicates the extent of the material (crystal) described in structure-related information (usually in reference to a parallel list of other structure properties).
In particular, if the items in this list references structure information described with properties `cartesian_site_positions` and `fractional_site_positions`, they MUST contain all sites *belonging* to the described extent.  
**Type:** list  

The value of each site_coordinate_span item MUST be one of the following:

  * `fundamental_domain`: means that sites described in the response span a fundamental domain (Vinberg, 1994; European Mathematical Society, 2020) of a periodic system.
    When a server indicates this span in the response, it MUST provide those sites that enable reconstruction of the whole periodic system by applying symmetry operations from `space_group_symmetry_operations_xyz` property and then applying translations given by `lattice_vectors`.
    The fundamental domain does not need to be a connected space region.

  * `asymmetric_unit`: all sites are in a simply connected space region that is a fundamental domain, as per IUCr Online Dictionary of Crystallography definition (IUCr, 2017).

  * `molecular_fundamental_domain`: a fundamental domain where all atoms connected by covalent or donor-acceptor coordination bonds are adjacent to each other, placed at a bond distance.

  * `molecular_asymmetric_unit`: an asymmetric unit (a simply connected fundamental domain) where all atoms bound by covalent or donor-acceptor coordination bonds are adjacent to each other, placed at a bond distance.

  * `unit_cell`: a full unit cell of a periodic system (crystal), i.e., any repeating unit chosen by the server defined by the property `lattice_vectors`.
    For this span, the server MUST provide a set of sites in the response that can be used to reconstruct the whole periodic system (crystal) by simply applying translations from the `lattice_vectors` property to those sites.

  * `molecular_unit_cell`: same as `unit_cell`, but in addition places atoms that are bound by covalent or coordination bonds at a bond distance from each other.

  * `molecular_entities`: sets of atoms that are bound by covalent or coordination bonds, as per IUPAC definition of a 'molecular entity'.
    This set of sites MAY be larger than a fundamental domain.

  * `other`: any other collection of sites that does not fit the enumerated values above.

  * `null`: if omitted or `null`, the default value of `site_coordinate_span` is `unit_cell`.
    This is the assumed behavior of all main implementations before the `site_coordinate_span` definition was introduced.

**Note**: In all cases it is RECOMMENDED that only the minimal set of the sites that is needed to reconstruct the whole material is provided.
For example, for the 'unit_cell' span the server SHOULD NOT return sites that can be obtained from other returned sites through the translations given in `lattice_vectors`; only a non-redundant set of sites SHOULD be provided.

**Bibliographic References**:

E.B. Vinberg (originator). (1994) Encyclopedia of Mathematics. ISBN `1402006098 <https://isbnsearch.org/isbn/1402006098>`__, URL: https://encyclopediaofmath.org/index.php?title=Fundamental_domain&oldid=13590 [accessed 2025-04-30T08:55+03:00].

European Mathematical Society (2020). Fundamental domain. Encyclopedia of Mathematics. URL: http://encyclopediaofmath.org/index.php?title=Fundamental_domain&oldid=47023 [accessed 2025-04-30T08:53+03:00].

IUCr (2017). Asymmetric unit. Online Dictionary of Crystallography, URL: https://dictionary.iucr.org/Asymmetric_unit [accessed 2025-04-30T09:01+03:00].

**Examples:**



**Formats:** [[JSON](site_coordinate_span.json)] [[MD](site_coordinate_span.md)]

**JSON definition:**

``` json
{
    "$id": "https://schemas.optimade.org/defs/v1.3/properties/optimade/trajectories/site_coordinate_span",
    "$schema": "https://schemas.optimade.org/meta/v1.3/optimade/property_definition.json",
    "title": "list of site coordinate span",
    "x-optimade-type": "list",
    "x-optimade-definition": {
        "label": "site_coordinate_span_optimade_trajectories",
        "kind": "property",
        "version": "1.3.0",
        "format": "1.3",
        "name": "site_coordinate_span"
    },
    "x-optimade-dimensions": {
        "names": [
            "dim_frames"
        ],
        "compactable": [
            "constant"
        ],
        "sizes": [
            null
        ]
    },
    "type": [
        "array",
        "null"
    ],
    "description": "A list of site_coordinate_span items.\nA site_coordinate_span item indicates the extent of the material (crystal) described in structure-related information (usually in reference to a parallel list of other structure properties).\nIn particular, if the items in this list references structure information described with properties `cartesian_site_positions` and `fractional_site_positions`, they MUST contain all sites *belonging* to the described extent.\n\nThe value of each site_coordinate_span item MUST be one of the following:\n\n  * `fundamental_domain`: means that sites described in the response span a fundamental domain (Vinberg, 1994; European Mathematical Society, 2020) of a periodic system.\n    When a server indicates this span in the response, it MUST provide those sites that enable reconstruction of the whole periodic system by applying symmetry operations from `space_group_symmetry_operations_xyz` property and then applying translations given by `lattice_vectors`.\n    The fundamental domain does not need to be a connected space region.\n\n  * `asymmetric_unit`: all sites are in a simply connected space region that is a fundamental domain, as per IUCr Online Dictionary of Crystallography definition (IUCr, 2017).\n\n  * `molecular_fundamental_domain`: a fundamental domain where all atoms connected by covalent or donor-acceptor coordination bonds are adjacent to each other, placed at a bond distance.\n\n  * `molecular_asymmetric_unit`: an asymmetric unit (a simply connected fundamental domain) where all atoms bound by covalent or donor-acceptor coordination bonds are adjacent to each other, placed at a bond distance.\n\n  * `unit_cell`: a full unit cell of a periodic system (crystal), i.e., any repeating unit chosen by the server defined by the property `lattice_vectors`.\n    For this span, the server MUST provide a set of sites in the response that can be used to reconstruct the whole periodic system (crystal) by simply applying translations from the `lattice_vectors` property to those sites.\n\n  * `molecular_unit_cell`: same as `unit_cell`, but in addition places atoms that are bound by covalent or coordination bonds at a bond distance from each other.\n\n  * `molecular_entities`: sets of atoms that are bound by covalent or coordination bonds, as per IUPAC definition of a 'molecular entity'.\n    This set of sites MAY be larger than a fundamental domain.\n\n  * `other`: any other collection of sites that does not fit the enumerated values above.\n\n  * `null`: if omitted or `null`, the default value of `site_coordinate_span` is `unit_cell`.\n    This is the assumed behavior of all main implementations before the `site_coordinate_span` definition was introduced.\n\n**Note**: In all cases it is RECOMMENDED that only the minimal set of the sites that is needed to reconstruct the whole material is provided.\nFor example, for the 'unit_cell' span the server SHOULD NOT return sites that can be obtained from other returned sites through the translations given in `lattice_vectors`; only a non-redundant set of sites SHOULD be provided.\n\n**Bibliographic References**:\n\nE.B. Vinberg (originator). (1994) Encyclopedia of Mathematics. ISBN `1402006098 <https://isbnsearch.org/isbn/1402006098>`__, URL: https://encyclopediaofmath.org/index.php?title=Fundamental_domain&oldid=13590 [accessed 2025-04-30T08:55+03:00].\n\nEuropean Mathematical Society (2020). Fundamental domain. Encyclopedia of Mathematics. URL: http://encyclopediaofmath.org/index.php?title=Fundamental_domain&oldid=47023 [accessed 2025-04-30T08:53+03:00].\n\nIUCr (2017). Asymmetric unit. Online Dictionary of Crystallography, URL: https://dictionary.iucr.org/Asymmetric_unit [accessed 2025-04-30T09:01+03:00].",
    "x-optimade-unit": "inapplicable",
    "items": {
        "$id": "https://schemas.optimade.org/defs/v1.3/properties/optimade/structures/site_coordinate_span",
        "title": "site coordinate span",
        "x-optimade-type": "string",
        "x-optimade-definition": {
            "label": "site_coordinate_span_optimade_structures",
            "kind": "property",
            "version": "1.3.0",
            "format": "1.2",
            "name": "site_coordinate_span"
        },
        "type": [
            "string",
            "null"
        ],
        "description": "Indicates the extent of the material (crystal) described in the response.\nIn particular, properties `cartesian_site_positions` and `fractional_site_positions` MUST contain all sites *belonging* to the described extent.\n\nThe value of this property MUST be one of the following:\n\n  * `fundamental_domain`: means that sites described in the response span a fundamental domain (Vinberg, 1994; European Mathematical Society, 2020) of a periodic system.\n    When a server indicates this span in the response, it MUST provide those sites that enable reconstruction of the whole periodic system by applying symmetry operations from `space_group_symmetry_operations_xyz` property and then applying translations given by `lattice_vectors`.\n    The fundamental domain does not need to be a connected space region.\n\n  * `asymmetric_unit`: all sites are in a simply connected space region that is a fundamental domain, as per IUCr Online Dictionary of Crystallography definition (IUCr, 2017).\n\n  * `molecular_fundamental_domain`: a fundamental domain where all atoms connected by covalent or donor-acceptor coordination bonds are adjacent to each other, placed at a bond distance.\n\n  * `molecular_asymmetric_unit`: an asymmetric unit (a simply connected fundamental domain) where all atoms bound by covalent or donor-acceptor coordination bonds are adjacent to each other, placed at a bond distance.\n\n  * `unit_cell`: a full unit cell of a periodic system (crystal), i.e., any repeating unit chosen by the server defined by the property `lattice_vectors`.\n    For this span, the server MUST provide a set of sites in the response that can be used to reconstruct the whole periodic system (crystal) by simply applying translations from the `lattice_vectors` property to those sites.\n\n  * `molecular_unit_cell`: same as `unit_cell`, but in addition places atoms that are bound by covalent or coordination bonds at a bond distance from each other.\n\n  * `molecular_entities`: sets of atoms that are bound by covalent or coordination bonds, as per IUPAC definition of a 'molecular entity'.\n    This set of sites MAY be larger than a fundamental domain.\n\n  * `other`: any other collection of sites that does not fit the enumerated values above.\n\n  * `null`: if omitted or `null`, the default value of `site_coordinate_span` is `unit_cell`.\n    This is the assumed behavior of all main implementations before the `site_coordinate_span` definition was introduced.\n\n**Note**: In all cases it is RECOMMENDED that only the minimal set of the sites that is needed to reconstruct the whole material is provided.\nFor example, for the 'unit_cell' span the server SHOULD NOT return sites that can be obtained from other returned sites through the translations given in `lattice_vectors`; only a non-redundant set of sites SHOULD be provided.\n\n**Bibliographic References**:\n\nE.B. Vinberg (originator). (1994) Encyclopedia of Mathematics. ISBN `1402006098 <https://isbnsearch.org/isbn/1402006098>`__, URL: https://encyclopediaofmath.org/index.php?title=Fundamental_domain&oldid=13590 [accessed 2025-04-30T08:55+03:00].\n\nEuropean Mathematical Society (2020). Fundamental domain. Encyclopedia of Mathematics. URL: http://encyclopediaofmath.org/index.php?title=Fundamental_domain&oldid=47023 [accessed 2025-04-30T08:53+03:00].\n\nIUCr (2017). Asymmetric unit. Online Dictionary of Crystallography, URL: https://dictionary.iucr.org/Asymmetric_unit [accessed 2025-04-30T09:01+03:00].",
        "examples": [
            "asymmetric_unit",
            "unit_cell"
        ],
        "x-optimade-unit": "inapplicable",
        "enum": [
            "fundamental_domain",
            "asymmetric_unit",
            "molecular_fundamental_domain",
            "molecular_asymmetric_unit",
            "unit_cell",
            "molecular_unit_cell",
            "molecular_entities",
            "other"
        ]
    }
}
```
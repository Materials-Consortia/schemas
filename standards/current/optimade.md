files
-----

media_type
==========

**Name**: Media type
**Description**: Media type identifier (also known as MIME type), for a file as per [RFC 6838 Media Type Specifications and Registration Procedures](https://datatracker.ietf.org/doc/html/rfc6838).
**Type**: string
**Requirements/Conventions**:
- **Support**: OPTIONAL support in implementations, i.e., MAY be :val:`null`.
- **Query**: Support for queries on this property is OPTIONAL.
- **Response**:

**Examples**:

- `chemical/x-cif`

modification_timestamp
======================

**Name**: Modification timestamp
**Description**: Timestamp of the last modification of file contents. A modification is understood as an addition, change or deletion of one or more bytes, resulting in file contents different from the previous.
**Type**: timestamp
**Requirements/Conventions**:
- **Support**: OPTIONAL support in implementations, i.e., MAY be :val:`null`.
- **Query**: Support for queries on this property is OPTIONAL.
- **Response**:
- Timestamps of subsequent file modifications SHOULD be increasing (not earlier than previous timestamps).
**Examples**:

- `2020-04-05T14:30:20Z`

name
====

**Name**: Name
**Description**: Base name of a file.
**Type**: string
**Requirements/Conventions**:
- **Support**: MUST be supported by all implementations, MUST NOT be :val:`null`.
- **Query**: Support for queries on this property is OPTIONAL.
- **Response**:
- File name extension is an integral part of a file name and, if available, MUST be included.
**Examples**:

- `1000000.cif`

size
====

**Name**: Size
**Description**: Size of a file in bytes.
**Type**: integer
**Requirements/Conventions**:
- **Support**: OPTIONAL support in implementations, i.e., MAY be :val:`null`.
- **Query**: Support for queries on this property is OPTIONAL.
- **Response**:
- If provided, it MUST be guaranteed that either exact size of a file is given or its upper bound.
  This way if a client reserves a static buffer or truncates the download stream after this many bytes the whole file would be received.
  Such provision is included to allow the providers to serve on-the-fly compressed files.
**Examples**:

- `4711`

url
===

**Name**: URL
**Description**: The URL to get the contents of a file.
**Type**: string
**Requirements/Conventions**:
- **Support**: MUST be supported by all implementations, MUST NOT be :val:`null`.
- **Query**: Support for queries on this property is OPTIONAL.
- **Response**:
- The URL MUST point to the actual contents of a file (i.e. byte stream), not an intermediate (preview) representation. For example, if referring to a file on GitHub, a link should point to raw contents.
**Examples**:

- `https://example.org/files/cifs/1000000.cif`

url_stable_until
================

**Name**: URL stable until
**Description**: Point in time until which the URL in `url` is guaranteed to stay stable.
**Type**: timestamp
**Requirements/Conventions**:
- **Support**: OPTIONAL support in implementations, i.e., MAY be :val:`null`.
- **Query**: Support for queries on this property is OPTIONAL.
- **Response**:
- `null` means that there is no stability guarantee for the URL in url.
  Indefinite support could be communicated by providing a date sufficiently far in the future, for example, 9999-12-31.
**Examples**:

- `2052-04-05T14:30:20Z`

version
=======

**Name**: Version
**Description**: Version information of a file (e.g. commit, revision, timestamp).
**Type**: string
**Requirements/Conventions**:
- **Support**: OPTIONAL support in implementations, i.e., MAY be :val:`null`.
- **Query**: Support for queries on this property is OPTIONAL.
- **Response**:
- If provided, it MUST be guaranteed that file contents pertaining to the same combination of id and version are the same.
**Examples**:

- `3.2.6`


structures
----------

assemblies
==========

**Name**: Assemblies
**Description**: A description of groups of sites that are statistically correlated.

**Requirements/Conventions**:

- The property SHOULD be `null` for entries that have no partial occupancies.
- If present, the correct flag MUST be set in the list `structure_features` (see property `structure_features`).
- Client implementations MUST check its presence (as its presence changes the interpretation of the structure).
- If present, it MUST be a list of dictionaries, each of which represents an assembly and MUST have the following two keys:

  - **sites_in_groups**: Index of the sites (0-based) that belong to each group for each assembly.

    Example: `[[1], [2]]`: two groups, one with the second site, one with the third.
    Example: `[[1,2], [3]]`: one group with the second and third site, one with the fourth.

  - **group_probabilities**: Statistical probability of each group. It MUST have the same length as `sites_in_groups`.
    It SHOULD sum to one.
    See below for examples of how to specify the probability of the occurrence of a vacancy.
    The possible reasons for the values not to sum to one are the same as already specified above for the `concentration` of each `species`, see property `species`.

- If a site is not present in any group, it means that it is present with 100 % probability (as if no assembly was specified).
- A site MUST NOT appear in more than one group.

**Explained examples**:

- `{"sites_in_groups": [[0], [1]], "group_probabilities": [0.3, 0.7]}`: the first site and the second site never occur at the same time in the unit cell.
  Statistically, 30 % of the times the first site is present, while 70 % of the times the second site is present.
- `{"sites_in_groups": [[1,2], [3]], "group_probabilities": [0.3, 0.7]}`: the second and third sites are either present together or not present; they form the first group of atoms for this assembly.
  The second group is formed by the fourth site.
  Sites of the first group (the second and the third) are never present at the same time as the fourth site.
  30 % of times sites 1 and 2 are present (and site 3 is absent); 70 % of times site 3 is present (and sites 1 and 2 are absent).

- **Notes**:

  - Assemblies are essential to represent, for instance, the situation where an atom can statistically occupy two different positions (sites).
  - By defining groups, it is possible to represent, e.g., the case where a functional molecule (and not just one atom) is either present or absent (or the case where it is present in two conformations).
  - Considerations on virtual alloys and on vacancies: In the special case of a virtual alloy, these specifications allow two different, equivalent ways of specifying them.
    For instance, for a site at the origin with 30 % probability of being occupied by Si, 50 % probability of being occupied by Ge, and 20 % of being a vacancy, the following two representations are possible:

    - Using a single species:

      ```

           {
             "cartesian_site_positions": [[0,0,0]],
             "species_at_sites": ["SiGe-vac"],
             "species": [
               {
                 "name": "SiGe-vac",
                 "chemical_symbols": ["Si", "Ge", "vacancy"],
                 "concentration": [0.3, 0.5, 0.2]
               }
             ]
             // ...
           }
      ```


    - Using multiple species and the assemblies:

      ```

           {
             "cartesian_site_positions": [ [0,0,0], [0,0,0], [0,0,0] ],
             "species_at_sites": ["Si", "Ge", "vac"],
             "species": [
               { "name": "Si", "chemical_symbols": ["Si"], "concentration": [1.0] },
               { "name": "Ge", "chemical_symbols": ["Ge"], "concentration": [1.0] },
               { "name": "vac", "chemical_symbols": ["vacancy"], "concentration": [1.0] }
             ],
             "assemblies": [
               {
                 "sites_in_groups": [ [0], [1], [2] ],
                 "group_probabilities": [0.3, 0.5, 0.2]
               }
             ]
             // ...
           }
      ```

  - It is up to the database provider to decide which representation to use, typically depending on the internal format in which the structure is stored.
    However, given a structure identified by a unique ID, the API implementation MUST always provide the same representation for it.
  - The probabilities of occurrence of different assemblies are uncorrelated.
    So, for instance in the following case with two assemblies:

    ```

         {
           "assemblies": [
             {
               "sites_in_groups": [ [0], [1] ],
               "group_probabilities": [0.2, 0.8]
             },
             {
               "sites_in_groups": [ [2], [3] ],
               "group_probabilities": [0.3, 0.7]
             }
           ]
         }
    ```

    Site 0 is present with a probability of 20 % and site 1 with a probability of 80 %. These two sites are correlated (either site 0 or 1 is present). Similarly, site 2 is present with a probability of 30 % and site 3 with a probability of 70 %.
    These two sites are correlated (either site 2 or 3 is present).
    However, the presence or absence of sites 0 and 1 is not correlated with the presence or absence of sites 2 and 3 (in the specific example, the pair of sites (0, 2) can occur with 0.2*0.3 = 6 % probability; the pair (0, 3) with 0.2*0.7 = 14 % probability; the pair (1, 2) with 0.8*0.3 = 24 % probability; and the pair (1, 3) with 0.8*0.7 = 56 % probability).
**Type**: dictionary
**Requirements/Conventions**:
- **Support**: SHOULD be supported by all implementations, i.e., SHOULD NOT be :val:`null`.
- **Query**: Support for queries on this property is OPTIONAL.
- **Response**:

**Examples**:

- `{'sites_in_groups': [[0], [1]], 'group_probabilities': [0.3, 0.7]}`
- `{'sites_in_groups': [[1, 2], [3]], 'group_probabilities': [0.3, 0.7]}`

cartesian_site_positions
========================

**Name**: Cartesian site positions
**Description**: Cartesian positions of each site in the structure. A site is usually used to describe positions of atoms; what atoms can be encountered at a given site is conveyed by the `species_at_sites` property, and the species themselves are described in the `species` property.

**Requirements/Conventions**:

- It MUST be a list of length equal to the number of sites in the structure, where every element is a list of the three Cartesian coordinates of a site expressed as float values in the unit angstrom (Å).
- An entry MAY have multiple sites at the same Cartesian position (for a relevant use of this, see e.g., the property `assemblies`).

**Explained examples**:

- :val:`[[0,0,0],[0,0,2]]` indicates a structure with two sites, one sitting at the origin and one along the (positive) *z*-axis, 2 Å away from the origin.
**Type**: list
**Requirements/Conventions**:
- **Support**: SHOULD be supported by all implementations, i.e., SHOULD NOT be :val:`null`.
- **Query**: Support for queries on this property is OPTIONAL.
- **Response**:

**Examples**:

- `[[0, 0, 0], [0, 0, 2]]`

chemical_formula_anonymous
==========================

**Name**: Anonymous chemical formula
**Description**: The anonymous formula is the chemical_formula_reduced, but where the elements are instead first ordered by their chemical proportion number, and then, in order left to right, replaced by anonymous symbols A, B, C, ..., Z, Aa, Ba, ..., Za, Ab, Bb, ... and so on.
**Type**: string
**Requirements/Conventions**:
- **Support**: SHOULD be supported by all implementations, i.e., SHOULD NOT be :val:`null`.
- **Query**: MUST be a queryable property with support for all mandatory filter features.
- **Response**:

**Examples**:

- `A2B`
- `A42B42C16D12E10F9G5`

chemical_formula_descriptive
============================

**Name**: Descriptive chemical formula
**Description**: The chemical formula for a structure as a string in a form chosen by the API implementation.

**Requirements/Conventions**:

- The chemical formula is given as a string consisting of properly capitalized element symbols followed by integers or decimal numbers, balanced parentheses, square, and curly brackets `(`,\ `)`, `[`,\ `]`, `{`, `}`, commas, the `+`, `-`, `:` and `=` symbols.
  The parentheses are allowed to be followed by a number.
  Spaces are allowed anywhere except within chemical symbols.
  The order of elements and any groupings indicated by parentheses or brackets are chosen freely by the API implementation.
- The string SHOULD be arithmetically consistent with the element ratios in the `chemical_formula_reduced` property.
- It is RECOMMENDED, but not mandatory, that symbols, parentheses and brackets, if used, are used with the meanings prescribed by [IUPAC's Nomenclature of Organic Chemistry](https://www.qmul.ac.uk/sbcs/iupac/bibliog/blue.html).

**Query examples**:

- Note: the free-form nature of this property is likely to make queries on it across different databases inconsistent.
- A filter that matches an exactly given formula: :filter:`chemical_formula_descriptive="(H2O)2 Na"`.
- A filter that does a partial match: :filter:`chemical_formula_descriptive CONTAINS "H2O"`.
**Type**: string
**Requirements/Conventions**:
- **Support**: SHOULD be supported by all implementations, i.e., SHOULD NOT be :val:`null`.
- **Query**: MUST be a queryable property with support for all mandatory filter features.
- **Response**:

**Examples**:

- `(H2O)2 Na`
- `NaCl`
- `CaCO3`
- `CCaO3`
- `(CH3)3N+ - [CH2]2-OH = Me3N+ - CH2 - CH2OH`

chemical_formula_hill
=====================

**Name**: Hill chemical formula
**Description**: The chemical formula for a structure in `Hill form <https://dx.doi.org/10.1021/ja02046a005>`__ with element symbols followed by integer chemical proportion numbers. The proportion number MUST be omitted if it is 1.

**Requirements/Conventions**:

- The overall scale factor of the chemical proportions is chosen such that the resulting values are integers that indicate the most chemically relevant unit of which the system is composed.
  For example, if the structure is a repeating unit cell with four hydrogens and four oxygens that represents two hydroperoxide molecules, :property:`chemical_formula_hill` is :val:`"H2O2"` (i.e., not :val:`"HO"`, nor :val:`"H4O4"`).
- If the chemical insight needed to ascribe a Hill formula to the system is not present, the property MUST be handled as unset.
- Element symbols MUST have proper capitalization (e.g., :val:`"Si"`, not :VAL:`"SI"` for "silicon").
- Elements MUST be placed in `Hill order <https://dx.doi.org/10.1021/ja02046a005>`__, followed by their integer chemical proportion number.
  Hill order means: if carbon is present, it is placed first, and if also present, hydrogen is placed second.
  After that, all other elements are ordered alphabetically.
  If carbon is not present, all elements are ordered alphabetically.
- If the system has sites with partial occupation and the total occupations of each element do not all sum up to integers, then the Hill formula SHOULD be handled as unset.
- No spaces or separators are allowed.

**Query examples**:

- A filter that matches an exactly given formula is `chemical_formula_hill="H2O2"`.
**Type**: string
**Requirements/Conventions**:
- **Support**: OPTIONAL support in implementations, i.e., MAY be :val:`null`.
- **Query**: Support for queries on this property is OPTIONAL.
- **Response**:

**Examples**:

- `H2O2`

chemical_formula_reduced
========================

**Name**: Reduced chemical formula
**Description**: The reduced chemical formula for a structure as a string with element symbols and integer chemical proportion numbers.

**Requirements/Conventions**:

- Intricate queries on formula components are suggested to be formulated using set-type filter operators on the multi valued :property:`elements` and :property:`elements_ratios` properties.
- Element symbols MUST have proper capitalization (e.g., :val:`"Si"`, not :VAL:`"SI"` for "silicon").
- Elements MUST be placed in alphabetical order, followed by their integer chemical proportion number.
- For structures with no partial occupation, the chemical proportion numbers are the smallest integers for which the chemical proportion is exactly correct.
- For structures with partial occupation, the chemical proportion numbers are integers that within reasonable approximation indicate the correct chemical proportions. The precise details of how to perform the rounding is chosen by the API implementation.
- No spaces or separators are allowed.

**Query examples**:

- A filter that matches an exactly given formula is `chemical_formula_reduced="H2NaO"`.
**Type**: string
**Requirements/Conventions**:
- **Support**: SHOULD be supported by all implementations, i.e., SHOULD NOT be :val:`null`.
- **Query**: MUST be queryable using the OPTIMADE filter language equality and inequality operators. Other filter language features do not need to be available.
- **Response**:

**Examples**:

- `H2NaO`
- `ClNa`
- `CCaO3`

dimension_types
===============

**Name**: Dimension types
**Description**: List of three integers describing the periodicity of the boundaries of the unit cell. For each direction indicated by the three lattice_vectors, this list indicates if the direction is periodic (value 1) or non-periodic (value 0). Note: the elements in this list each refer to the direction of the corresponding entry in lattice_vectors and not the Cartesian x, y, z directions.

**Requirements/Conventions**:

- MUST be a list of length 3.
- Each integer element MUST assume only the value 0 or 1.

**Explained examples**:

- A nonperiodic structure, for example, for a single molecule : `[0, 0, 0]`
- A unit cell that is periodic in the direction of the third lattice vector, for example for a carbon nanotube: `[0, 0, 1]`
- For a 2D surface/slab, with a unit cell that is periodic in the direction of the first and third lattice vectors: `[1, 0, 1]`
- For a bulk 3D system with a unit cell that is periodic in all directions: `[1, 1, 1]`
**Type**: list
**Requirements/Conventions**:
- **Support**: SHOULD be supported by all implementations, i.e., SHOULD NOT be :val:`null`.
- **Query**: Support for queries on this property is OPTIONAL.
- **Response**:

**Examples**:

- `[0, 0, 0]`
- `[0, 0, 1]`
- `[1, 0, 1]`

elements
========

**Name**: Elements
**Description**: The chemical symbols of the different elements present in the structure.

**Requirements/Conventions**:

- The strings are the chemical symbols, i.e., either a single uppercase letter or an uppercase letter followed by a number of lowercase letters.
- The order MUST be alphabetical.
- MUST refer to the same elements in the same order, and therefore be of the same length, as elements_ratios, if the latter is provided.
- Note: This property SHOULD NOT contain the string "X" to indicate non-chemical elements or "vacancy" to indicate vacancies (in contrast to the field chemical_symbols for the species property).

**Query examples**:

- A filter that matches all records of structures that contain Si, Al **and** O, and possibly other elements: `elements HAS ALL "Si", "Al", "O"`.
- To match structures with exactly these three elements, use `elements HAS ALL "Si", "Al", "O" AND elements LENGTH 3`.
- Note: length queries on this property can be equivalently formulated by filtering on the `nelements`_ property directly.
**Type**: list
**Requirements/Conventions**:
- **Support**: SHOULD be supported by all implementations, i.e., SHOULD NOT be :val:`null`.
- **Query**: MUST be a queryable property with support for all mandatory filter features.
- **Response**:

**Examples**:

- `['Al', 'Si', 'O']`
- `['He']`

elements_ratios
===============

**Name**: Elements ratios
**Description**: Relative proportions of different elements in the structure.

**Requirements/Conventions**:

- Composed by the proportions of elements in the structure as a list of floating point numbers.
- The sum of the numbers MUST be 1.0 (within floating point accuracy)
- MUST refer to the same elements in the same order, and therefore be of the same length, as `elements`_, if the latter is provided.

**Query examples**:

- Note: Useful filters can be formulated using the set operator syntax for correlated values.
  However, since the values are floating point values, the use of equality comparisons is generally inadvisable.
- OPTIONAL: a filter that matches structures where approximately 1/3 of the atoms in the structure are the element Al is: `elements:elements_ratios HAS ALL "Al":>0.3333, "Al":<0.3334`.
**Type**: list
**Requirements/Conventions**:
- **Support**: SHOULD be supported by all implementations, i.e., SHOULD NOT be :val:`null`.
- **Query**: MUST be a queryable property with support for all mandatory filter features.
- **Response**:

**Examples**:

- `[1.0]`
- `[0.3333333333333333, 0.2222222222222222, 0.4444444444444444]`

id
==

**Name**: Immutable ID
**Description**: The entry's immutable ID (e.g., a UUID).
**Type**: string
**Requirements/Conventions**:
- **Support**: MUST be supported by all implementations, MUST NOT be :val:`null`.
- **Query**: MUST be a queryable property with support for all mandatory filter features.
- **Response**:
- This is important for databases having preferred IDs that point to "the latest version" of a record, but still offer access to older variants.
- This ID maps to the version-specific record, in case it changes in the future.
**Examples**:

- `8bd3e750-b477-41a0-9b11-3a799f21b44f`
- `fjeiwoj,54;@=%<>#32`

immutable_id
============

**Name**: Immutable ID
**Description**: The entry's immutable ID (e.g., a UUID).
**Type**: string
**Requirements/Conventions**:
- **Support**: OPTIONAL support in implementations, i.e., MAY be :val:`null`.
- **Query**: MUST be a queryable property with support for all mandatory filter features.
- **Response**:
- This is important for databases having preferred IDs that point to "the latest version" of a record, but still offer access to older variants.
- This ID maps to the version-specific record, in case it changes in the future.
**Examples**:

- `8bd3e750-b477-41a0-9b11-3a799f21b44f`
- `fjeiwoj,54;@=%<>#32`

last_modified
=============

**Name**: Last modified
**Description**: Date and time representing when the entry was last modified.
**Type**: timestamp
**Requirements/Conventions**:
- **Support**: MUST be supported by all implementations, MUST NOT be :val:`null`.
- **Query**: MUST be a queryable property with support for all mandatory filter features.
- **Response**:

**Examples**:

- `2007-04-05T14:30:20Z`

lattice_vectors
===============

**Name**: Lattice vectors
**Description**: The three lattice vectors in Cartesian coordinates, in ångström (Å).

**Requirements/Conventions**:

- MUST be a list of three vectors *a*, *b*, and *c*, where each of the vectors MUST BE a list of the vector's coordinates along the x, y, and z Cartesian coordinates.
  (Therefore, the first index runs over the three lattice vectors and the second index runs over the x, y, z Cartesian coordinates).
- For databases that do not define an absolute Cartesian system (e.g., only defining the length and angles between vectors), the first lattice vector SHOULD be set along *x* and the second on the *xy*-plane.
- MUST always contain three vectors of three coordinates each, independently of the elements of property `dimension\_types`_.
  The vectors SHOULD by convention be chosen so the determinant of the `lattice_vectors` matrix is different from zero.
  The vectors in the non-periodic directions have no significance beyond fulfilling these requirements.
- The coordinates of the lattice vectors of non-periodic dimensions (i.e., those dimensions for which `dimension\_types`_ is `0`) MAY be given as a list of all `null` values.
  If a lattice vector contains the value `null`, all coordinates of that lattice vector MUST be `null`.

**Explained examples**:

- `[[4.0,0.0,0.0],[0.0,4.0,0.0],[0.0,1.0,4.0]]` represents a cell, where the first vector is (4, 0, 0), i.e., a vector aligned along the x axis of length 4 Å; the second vector is (0, 4, 0); and the third vector is (0, 1, 4).
**Type**: list
**Requirements/Conventions**:
- **Support**: SHOULD be supported by all implementations, i.e., SHOULD NOT be :val:`null`.
- **Query**: Support for queries on this property is OPTIONAL.
- **Response**:

**Examples**:

- `[[4.0, 0.0, 0.0], [0.0, 4.0, 0.0], [0.0, 1.0, 4.0]]`

nelements
=========

**Name**: Number of elements
**Description**: Number of different elements in the structure as an integer.

**Requirements/Conventions**:

- MUST be equal to the lengths of the list properties elements and elements_ratios, if they are provided.

**Querying**:

- Queries on this property can equivalently be formulated using `elements LENGTH`.
- A filter that matches structures that have exactly 4 elements: `nelements=4`.
- A filter that matches structures that have between 2 and 7 elements: `nelements>=2 AND nelements<=7`.
**Type**: integer
**Requirements/Conventions**:
- **Support**: SHOULD be supported by all implementations, i.e., SHOULD NOT be :val:`null`.
- **Query**: MUST be a queryable property with support for all mandatory filter features.
- **Response**:

**Examples**:

- `3`

nperiodic_dimensions
====================

**Name**: Number of periodic dimensions
**Description**: An integer specifying the number of periodic dimensions in the structure, equivalent to the number of non-zero entries in `dimension_types`.

**Requirements/Conventions**:

- The integer value MUST be between 0 and 3 inclusive and MUST be equal to the sum of the items in the dimension_types property.

- This property only reflects the treatment of the lattice vectors provided for the structure, and not any physical interpretation of the dimensionality of its contents.

**Explained examples**

- `2` should be indicated in cases where dimension_types is any of `[1, 1, 0]`, `[1, 0, 1]`, `[0, 1, 1]`.

**Query examples**:

- Match only structures with exactly 3 periodic dimensions: `nperiodic_dimensions=3`
- Match all structures with 2 or fewer periodic dimensions: `nperiodic_dimensions<=2`
**Type**: integer
**Requirements/Conventions**:
- **Support**: SHOULD be supported by all implementations, i.e., SHOULD NOT be :val:`null`.
- **Query**: MUST be a queryable property with support for all mandatory filter features.
- **Response**:

**Examples**:

- `2`

nsites
======

**Name**: Number of sites
**Description**: An integer specifying the length of the `cartesian_site_positions` property.

**Requirements/Conventions**:

- MUST be equal to the lengths of the list properties elements and elements_ratios, if they are provided.

**Query examples**:

- Match only structures with exactly 4 sites: `nsites=4`
- Match structures that have between 2 and 7 sites: `nsites>=2 AND nsites<=7`
**Type**: integer
**Requirements/Conventions**:
- **Support**: SHOULD be supported by all implementations, i.e., SHOULD NOT be :val:`null`.
- **Query**: MUST be a queryable property with support for all mandatory filter features.
- **Response**:

**Examples**:

- `42`

space_group_hall
================

**Name**: Hall space group
**Description**: A Hall space group symbol representing the symmetry of the structure as defined in Hall, S. R. (1981), Acta Cryst. A37, 517-525 and erratum (1981), A37, 921.

**Requirements/Conventions**:

- Each component of the Hall symbol MUST be separated by a single space symbol.
- If there exists a standard Hall symbol which represents the symmetry it SHOULD be used.
- MUST be null if n`periodic_dimensions` is not equal to 3.
**Type**: string
**Requirements/Conventions**:
- **Support**: OPTIONAL support in implementations, i.e., MAY be :val:`null`.
- **Query**: Support for queries on this property is OPTIONAL.
- **Response**:

**Examples**:

- `P 2c -2ac`
- `-I 4db 2ab 3`

space_group_it_number
=====================

**Name**: Hall space group
**Description**: Space group number for the structure assigned by the International Tables for Crystallography Vol. A.

**Requirements/Conventions**:

- The integer value MUST be between 1 and 230.
- MUST be null if `nperiodic_dimensions` is not equal to 3.
**Type**: integer
**Requirements/Conventions**:
- **Support**: OPTIONAL support in implementations, i.e., MAY be :val:`null`.
- **Query**: Support for queries on this property is OPTIONAL.
- **Response**:

**Examples**:

- `42`

species
=======

**Name**: Species
**Description**: A list describing the species of the sites of this structure. Species can represent pure chemical elements, virtual-crystal atoms representing a statistical occupation of a given site by multiple chemical elements, and/or a location to which there are attached atoms, i.e., atoms whose precise location are unknown beyond that they are attached to that position (frequently used to indicate hydrogen atoms attached to another element, e.g., a carbon with three attached hydrogens might represent a methyl group, -CH3).

**Requirements/Conventions**:

- Each list member MUST be a dictionary with the following keys:

  - **name**: REQUIRED; gives the name of the species; the **name** value MUST be unique in the `species` list;

  - **chemical\_symbols**: REQUIRED; MUST be a list of strings of all chemical elements composing this species. Each item of the list MUST be one of the following:

    - a valid chemical-element symbol, or
    - the special value `"X"` to represent a non-chemical element, or
    - the special value `"vacancy"` to represent that this site has a non-zero probability of having a vacancy (the respective probability is indicated in the `concentration` list, see below).

    If any one entry in the `species` list has a `chemical_symbols` list that is longer than 1 element, the correct flag MUST be set in the list `structure_features` (see property `structure_features`_).

  - **concentration**: REQUIRED; MUST be a list of floats, with same length as `chemical_symbols`. The numbers represent the relative concentration of the corresponding chemical symbol in this species.
    The numbers SHOULD sum to one. Cases in which the numbers do not sum to one typically fall only in the following two categories:

    - Numerical errors when representing float numbers in fixed precision, e.g. for two chemical symbols with concentrations `1/3` and `2/3`, the concentration might look something like `[0.33333333333, 0.66666666666]`. If the client is aware that the sum is not one because of numerical precision, it can renormalize the values so that the sum is exactly one.
    - Experimental errors in the data present in the database. In this case, it is the responsibility of the client to decide how to process the data.

    Note that concentrations are uncorrelated between different sites (even of the same species).

  - **attached**: OPTIONAL; if provided MUST be a list of length 1 or more of strings of chemical symbols for the elements attached to this site, or "X" for a non-chemical element.
  - **nattached**: OPTIONAL; if provided MUST be a list of length 1 or more of integers indicating the number of attached atoms of the kind specified in the value of the `attached` key.

    The implementation MUST include either both or none of the `attached` and `nattached` keys, and if they are provided, they MUST be of the same length.
    Furthermore, if they are provided, the `structure_features`_ property MUST include the string `site_attachments`.

  - **mass**: OPTIONAL. If present MUST be a list of floats, with the same length as `chemical_symbols`, providing element masses expressed in a.m.u.
    Elements denoting vacancies MUST have masses equal to 0.
  - **original\_name**: OPTIONAL. Can be any valid Unicode string, and SHOULD contain (if specified) the name of the species that is used internally in the source database.

        **Note**: With regard to "source database", we refer to the immediate source being queried via the OPTIMADE API implementation.
        The main use of this field is for source databases that use species names, containing characters that are not allowed (see description of the list property `species_at_sites`_).

- For systems that have only species formed by a single chemical symbol, and that have at most one species per chemical symbol, SHOULD use the chemical symbol as species name (e.g., `"Ti"` for titanium, `"O"` for oxygen, etc.)
  However, note that this is OPTIONAL, and client implementations MUST NOT assume that the key corresponds to a chemical symbol, nor assume that if the species name is a valid chemical symbol, that it represents a species with that chemical symbol.
  This means that a species `{"name": "C", "chemical_symbols": ["Ti"], "concentration": [1.0]}` is valid and represents a titanium species (and *not* a carbon species).
- It is NOT RECOMMENDED that a structure includes species that do not have at least one corresponding site.

**Explained examples**:

- `[ {"name": "Ti", "chemical_symbols": ["Ti"], "concentration": [1.0]} ]`: any site with this species is occupied by a Ti atom.
- `[ {"name": "Ti", "chemical_symbols": ["Ti", "vacancy"], "concentration": [0.9, 0.1]} ]`: any site with this species is occupied by a Ti atom with 90 % probability, and has a vacancy with 10 % probability.
- `[ {"name": "BaCa", "chemical_symbols": ["vacancy", "Ba", "Ca"], "concentration": [0.05, 0.45, 0.5], "mass": [0.0, 137.327, 40.078]} ]`: any site with this species is occupied by a Ba atom with 45 % probability, a Ca atom with 50 % probability, and by a vacancy with 5 % probability.
- `[ {"name": "C12", "chemical_symbols": ["C"], "concentration": [1.0], "mass": [12.0]} ]`: any site with this species is occupied by a carbon isotope with mass 12.
- `[ {"name": "C13", "chemical_symbols": ["C"], "concentration": [1.0], "mass": [13.0]} ]`: any site with this species is occupied by a carbon isotope with mass 13.
- `[ {"name": "CH3", "chemical_symbols": ["C"], "concentration": [1.0], "attached": ["H"], "nattached": [3]} ]`: any site with this species is occupied by a methyl group, -CH3, which is represented without specifying precise positions of the hydrogen atoms.
**Type**: list
**Requirements/Conventions**:
- **Support**: SHOULD be supported by all implementations, i.e., SHOULD NOT be :val:`null`.
- **Query**: Support for queries on this property is OPTIONAL.
- **Response**:

**Examples**:

- `[{'name': 'Ti', 'chemical_symbols': ['Ti'], 'concentration': [1.0]}]`
- `[{'name': 'Ti', 'chemical_symbols': ['Ti', 'vacancy'], 'concentration': [0.9, 0.1]}]`
- `[{'name': 'BaCa', 'chemical_symbols': ['vacancy', 'Ba', 'Ca'], 'concentration': [0.05, 0.45, 0.5], 'mass': [0.0, 137.327, 40.078]}]`
- `[{'name': 'C12', 'chemical_symbols': ['C'], 'concentration': [1.0], 'mass': [12.0]}]`
- `[{'name': 'C13', 'chemical_symbols': ['C'], 'concentration': [1.0], 'mass': [13.0]}]`
- `[{'name': 'CH3', 'chemical_symbols': ['C'], 'concentration': [1.0], 'attached': ['H'], 'nattached': [3]}]`

species_at_sites
================

**Name**: Species at sites
**Description**: Name of the species at each site (where values for sites are specified with the same order of the property `cartesian_site_positions`_). The properties of the species are found in the property `species`_.

**Requirements/Conventions**:

- MUST have length equal to the number of sites in the structure (first dimension of the list property `cartesian_site_positions`_).
- Each species name mentioned in the `species_at_sites` list MUST be described in the list property `species`_ (i.e. for each value in the `species_at_sites` list there MUST exist exactly one dictionary in the `species` list with the `name` attribute equal to the corresponding `species_at_sites` value).
- Each site MUST be associated only to a single species.
  **Note**: However, species can represent mixtures of atoms, and multiple species MAY be defined for the same chemical element.
  This latter case is useful when different atoms of the same type need to be grouped or distinguished, for instance in simulation codes to assign different initial spin states.

**Explained examples**:

- `["Ti","O2"]` indicates that the first site is hosting a species labeled :val:`"Ti"` and the second a species labeled :val:`"O2"`
- `["Ac", "Ac", "Ag", "Ir"]` indicates that the first two sites contain the :val:`"Ac"` species, while the third and fourth sites contain the :val:`"Ag"` and :val:`"Ir"` species, respectively.
**Type**: list
**Requirements/Conventions**:
- **Support**: SHOULD be supported by all implementations, i.e., SHOULD NOT be :val:`null`.
- **Query**: Support for queries on this property is OPTIONAL.
- **Response**:

**Examples**:

- `['Ti', 'O2']`
- `['Ac', 'Ac', 'Ag', 'Ir']`

structure_features
==================

**Name**: Structure features
**Description**: A list of strings that flag which special features are used by the structure.
**Type**: list
**Requirements/Conventions**:
- **Support**: MUST be supported by all implementations, MUST NOT be :val:`null`.
- **Query**: MUST be a queryable property with support for all mandatory filter features.
- **Response**:
- MUST be an empty list if no special features are used.
- MUST be sorted alphabetically.
- If a special feature listed below is used, the list MUST contain the corresponding string.
- If a special feature listed below is not used, the list MUST NOT contain the corresponding string.
- **List of strings used to indicate special structure features:**
  - `disorder`: this flag MUST be present if any one entry in the species list has a `chemical_symbols` list that is longer than 1 element.
  - `implicit_atoms`: this flag MUST be present if the structure contains atoms that are not assigned to sites via the property `species_at_sites` (e.g., because their positions are unknown). When this flag is present, the properties related to the chemical formula will likely not match the type and count of atoms represented by the `species_at_sites`, `species`, and `assemblies` properties.
  - `site_attachments`: this flag MUST be present if any one entry in the species list includes `attached` and `nattached`.
  - `assemblies`: this flag MUST be present if the property assemblies is present.

  **Explained examples**:
  - A structure having implicit atoms and using assemblies: `["assemblies", "implicit_atoms"]`
**Examples**:

- `['assemblies', 'implicit_atoms']`

type
====

**Name**: Immutable ID
**Description**: The entry's immutable ID (e.g., a UUID).
**Type**: string
**Requirements/Conventions**:
- **Support**: MUST be supported by all implementations, MUST NOT be :val:`null`.
- **Query**: MUST be a queryable property with support for all mandatory filter features.
- **Response**:
- This is important for databases having preferred IDs that point to "the latest version" of a record, but still offer access to older variants.
- This ID maps to the version-specific record, in case it changes in the future.
**Examples**:

- `8bd3e750-b477-41a0-9b11-3a799f21b44f`
- `fjeiwoj,54;@=%<>#32`



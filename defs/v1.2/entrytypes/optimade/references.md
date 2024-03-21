# references (entrytype)

This page documents an [OPTIMADE](https://www.optimade.org/) [Entrytype Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/defs/v1.2/entrytypes/optimade/references`](https://schemas.optimade.org/defs/v1.2/entrytypes/optimade/references.md)**  
**Definition name:** `references`

**Entrytype name:** references  
**Description:** The references entry type describes a reference  

**Formats:** [[JSON](references.json)] [[MD](references.md)]

This entrytype defines the following properties:

* **[ID](../../properties/core/id.md)** (property) - [`https://schemas.optimade.org/defs/v1.2/properties/core/id`](https://schemas.optimade.org/defs/v1.2/properties/core/id.md)  
  A unique string referencing a specific entry in the database.

    **Requirements/Conventions:**  

    - **Support:** MUST be supported by all implementations, MUST NOT be `null`.
    - **Query:** MUST be a queryable property with support for all mandatory filter features.
    - **Response:** MUST always be included in the response.
    - Taken together, the ID and entry type MUST uniquely identify the entry.
    - Reasonably short IDs are encouraged and SHOULD NOT be longer than 255 characters.
    - IDs MAY change over time.


* **[type](../../properties/core/type.md)** (property) - [`https://schemas.optimade.org/defs/v1.2/properties/core/type`](https://schemas.optimade.org/defs/v1.2/properties/core/type.md)  
  The name of the type of an entry.

    **Requirements/Conventions:**  

    - **Support:** MUST be supported by all implementations, MUST NOT be `null`.
    - **Query:** MUST be a queryable property with support for all mandatory filter features.
    - **Response:** MUST always be included in the response.
    - MUST be an existing entry type.
    - The entry of type <type> and ID <id> MUST be returned in response to a request for /<type>/<id> under the versioned or unversioned base URL serving the API.


* **[immutable ID (immutable_id)](../../properties/core/immutable_id.md)** (property) - [`https://schemas.optimade.org/defs/v1.2/properties/core/immutable_id`](https://schemas.optimade.org/defs/v1.2/properties/core/immutable_id.md)  
  The entry's immutable ID (e.g., a UUID).

    **Requirements/Conventions:**  

    - **Support:** OPTIONAL support in implementations, i.e., MAY be `null`.
    - **Query:** MUST be a queryable property with support for all mandatory filter features.
    - **Response:** MAY be included by default in the response.
    - This is important for databases having preferred IDs that point to "the latest version" of a record, but still offer access to older variants.
    - This ID maps to the version-specific record, in case it changes in the future.


* **[last modified (last_modified)](../../properties/core/last_modified.md)** (property) - [`https://schemas.optimade.org/defs/v1.2/properties/core/last_modified`](https://schemas.optimade.org/defs/v1.2/properties/core/last_modified.md)  
  Date and time representing when the entry was last modified.

    **Requirements/Conventions:**  

    - **Support:** SHOULD be supported by all implementations, i.e., SHOULD NOT be `null`.
    - **Query:** MUST be a queryable property with support for all mandatory filter features.
    - **Response:** MUST be included by default in the response.

* **[address](../../properties/optimade/references/address.md)** (property) - [`https://schemas.optimade.org/defs/v1.2/properties/optimade/references/address`](https://schemas.optimade.org/defs/v1.2/properties/optimade/references/address.md)  
  Typically the location of the publisher or institution (the address field in the BibTeX specification).

    **Requirements/Conventions:**  

    - **Support:** OPTIONAL support in implementations, i.e., MAY be `null`.
    - **Query:** Support for queries on this property is OPTIONAL.
    - **Response:** MAY be included by default in the response.

* **[annote](../../properties/optimade/references/annote.md)** (property) - [`https://schemas.optimade.org/defs/v1.2/properties/optimade/references/annote`](https://schemas.optimade.org/defs/v1.2/properties/optimade/references/annote.md)  
  Additional notes or comments on the reference (the annote field in the BibTeX specification).

    **Requirements/Conventions:**  

    - **Support:** OPTIONAL support in implementations, i.e., MAY be `null`.
    - **Query:** Support for queries on this property is OPTIONAL.
    - **Response:** MAY be included by default in the response.

* **[booktitle](../../properties/optimade/references/booktitle.md)** (property) - [`https://schemas.optimade.org/defs/v1.2/properties/optimade/references/booktitle`](https://schemas.optimade.org/defs/v1.2/properties/optimade/references/booktitle.md)  
  The title of a book being cited; for parts of a book, use the title field instead (the booktitle field in the BibTeX specification).

    **Requirements/Conventions:**  

    - **Support:** OPTIONAL support in implementations, i.e., MAY be `null`.
    - **Query:** Support for queries on this property is OPTIONAL.
    - **Response:** MAY be included by default in the response.

* **[chapter](../../properties/optimade/references/chapter.md)** (property) - [`https://schemas.optimade.org/defs/v1.2/properties/optimade/references/chapter`](https://schemas.optimade.org/defs/v1.2/properties/optimade/references/chapter.md)  
  The chapter, section, or similar part number (the chapter field in the BibTeX specification).

    **Requirements/Conventions:**  

    - **Support:** OPTIONAL support in implementations, i.e., MAY be `null`.
    - **Query:** Support for queries on this property is OPTIONAL.
    - **Response:** MAY be included by default in the response.

* **[crossref](../../properties/optimade/references/crossref.md)** (property) - [`https://schemas.optimade.org/defs/v1.2/properties/optimade/references/crossref`](https://schemas.optimade.org/defs/v1.2/properties/optimade/references/crossref.md)  
  The database key of the entry being cross referenced (the crossref field in the BibTeX specification).

    **Requirements/Conventions:**  

    - **Support:** OPTIONAL support in implementations, i.e., MAY be `null`.
    - **Query:** Support for queries on this property is OPTIONAL.
    - **Response:** MAY be included by default in the response.

* **[edition](../../properties/optimade/references/edition.md)** (property) - [`https://schemas.optimade.org/defs/v1.2/properties/optimade/references/edition`](https://schemas.optimade.org/defs/v1.2/properties/optimade/references/edition.md)  
  The edition of a book (the edition field in the BibTeX specification).

    **Requirements/Conventions:**  

    - **Support:** OPTIONAL support in implementations, i.e., MAY be `null`.
    - **Query:** Support for queries on this property is OPTIONAL.
    - **Response:** MAY be included by default in the response.

* **[how published (howpublished)](../../properties/optimade/references/howpublished.md)** (property) - [`https://schemas.optimade.org/defs/v1.2/properties/optimade/references/howpublished`](https://schemas.optimade.org/defs/v1.2/properties/optimade/references/howpublished.md)  
  The method of publication (the howpublished field in the BibTeX specification)

    **Requirements/Conventions:**  

    - **Support:** OPTIONAL support in implementations, i.e., MAY be `null`.
    - **Query:** Support for queries on this property is OPTIONAL.
    - **Response:** MAY be included by default in the response.

* **[institution](../../properties/optimade/references/institution.md)** (property) - [`https://schemas.optimade.org/defs/v1.2/properties/optimade/references/institution`](https://schemas.optimade.org/defs/v1.2/properties/optimade/references/institution.md)  
  The sponsoring institution of a technical report (the institution field in the BibTeX specification).

    **Requirements/Conventions:**  

    - **Support:** OPTIONAL support in implementations, i.e., MAY be `null`.
    - **Query:** Support for queries on this property is OPTIONAL.
    - **Response:** MAY be included by default in the response.

* **[journal](../../properties/optimade/references/journal.md)** (property) - [`https://schemas.optimade.org/defs/v1.2/properties/optimade/references/journal`](https://schemas.optimade.org/defs/v1.2/properties/optimade/references/journal.md)  
  The name of a journal (the journal field in the BibTeX specification).

    **Requirements/Conventions:**  

    - **Support:** OPTIONAL support in implementations, i.e., MAY be `null`.
    - **Query:** Support for queries on this property is OPTIONAL.
    - **Response:** MAY be included by default in the response.

* **[key](../../properties/optimade/references/key.md)** (property) - [`https://schemas.optimade.org/defs/v1.2/properties/optimade/references/key`](https://schemas.optimade.org/defs/v1.2/properties/optimade/references/key.md)  
  Used for alphabetizing, cross-referencing, and creating a label (the key field in the BibTeX specification).

    **Requirements/Conventions:**  

    - **Support:** OPTIONAL support in implementations, i.e., MAY be `null`.
    - **Query:** Support for queries on this property is OPTIONAL.
    - **Response:** MAY be included by default in the response.

* **[month](../../properties/optimade/references/month.md)** (property) - [`https://schemas.optimade.org/defs/v1.2/properties/optimade/references/month`](https://schemas.optimade.org/defs/v1.2/properties/optimade/references/month.md)  
  The three-letter abbreviation of the month of publication or writing (the month field in the BibTeX specification).

    **Requirements/Conventions:**  

    - **Support:** OPTIONAL support in implementations, i.e., MAY be `null`.
    - **Query:** Support for queries on this property is OPTIONAL.
    - **Response:** MAY be included by default in the response.

* **[note](../../properties/optimade/references/note.md)** (property) - [`https://schemas.optimade.org/defs/v1.2/properties/optimade/references/note`](https://schemas.optimade.org/defs/v1.2/properties/optimade/references/note.md)  
  Additional information about the reference (the note field in the BibTeX specification).

    **Requirements/Conventions:**  

    - **Support:** OPTIONAL support in implementations, i.e., MAY be `null`.
    - **Query:** Support for queries on this property is OPTIONAL.
    - **Response:** MAY be included by default in the response.

* **[number](../../properties/optimade/references/number.md)** (property) - [`https://schemas.optimade.org/defs/v1.2/properties/optimade/references/number`](https://schemas.optimade.org/defs/v1.2/properties/optimade/references/number.md)  
  The number of a journal, magazine, technical report, or work in a series (the number field in the BibTeX specification).

    **Requirements/Conventions:**  

    - **Support:** OPTIONAL support in implementations, i.e., MAY be `null`.
    - **Query:** Support for queries on this property is OPTIONAL.
    - **Response:** MAY be included by default in the response.

* **[organization](../../properties/optimade/references/organization.md)** (property) - [`https://schemas.optimade.org/defs/v1.2/properties/optimade/references/organization`](https://schemas.optimade.org/defs/v1.2/properties/optimade/references/organization.md)  
  The organization sponsoring a conference or publishing a manual (the organization field in the BibTeX specification)

    **Requirements/Conventions:**  

    - **Support:** OPTIONAL support in implementations, i.e., MAY be `null`.
    - **Query:** Support for queries on this property is OPTIONAL.
    - **Response:** MAY be included by default in the response.

* **[pages](../../properties/optimade/references/pages.md)** (property) - [`https://schemas.optimade.org/defs/v1.2/properties/optimade/references/pages`](https://schemas.optimade.org/defs/v1.2/properties/optimade/references/pages.md)  
  The page number(s) of the reference (the pages field in the BibTeX specification).

    **Requirements/Conventions:**  

    - **Support:** OPTIONAL support in implementations, i.e., MAY be `null`.
    - **Query:** Support for queries on this property is OPTIONAL.
    - **Response:** MAY be included by default in the response.

* **[publisher](../../properties/optimade/references/publisher.md)** (property) - [`https://schemas.optimade.org/defs/v1.2/properties/optimade/references/publisher`](https://schemas.optimade.org/defs/v1.2/properties/optimade/references/publisher.md)  
  The name of the publisher (the publisher field in the BibTeX specification).

    **Requirements/Conventions:**  

    - **Support:** OPTIONAL support in implementations, i.e., MAY be `null`.
    - **Query:** Support for queries on this property is OPTIONAL.
    - **Response:** MAY be included by default in the response.

* **[school](../../properties/optimade/references/school.md)** (property) - [`https://schemas.optimade.org/defs/v1.2/properties/optimade/references/school`](https://schemas.optimade.org/defs/v1.2/properties/optimade/references/school.md)  
  The name of the school where a thesis was written (the school field in the BibTeX specification).

    **Requirements/Conventions:**  

    - **Support:** OPTIONAL support in implementations, i.e., MAY be `null`.
    - **Query:** Support for queries on this property is OPTIONAL.
    - **Response:** MAY be included by default in the response.

* **[series](../../properties/optimade/references/series.md)** (property) - [`https://schemas.optimade.org/defs/v1.2/properties/optimade/references/series`](https://schemas.optimade.org/defs/v1.2/properties/optimade/references/series.md)  
  The name of a series or set of books (the series field in the BibTeX specification).

    **Requirements/Conventions:**  

    - **Support:** OPTIONAL support in implementations, i.e., MAY be `null`.
    - **Query:** Support for queries on this property is OPTIONAL.
    - **Response:** MAY be included by default in the response.

* **[title](../../properties/optimade/references/title.md)** (property) - [`https://schemas.optimade.org/defs/v1.2/properties/optimade/references/title`](https://schemas.optimade.org/defs/v1.2/properties/optimade/references/title.md)  
  The title of the work (the title field in the BibTeX specification).

    **Requirements/Conventions:**  

    - **Support:** OPTIONAL support in implementations, i.e., MAY be `null`.
    - **Query:** Support for queries on this property is OPTIONAL.
    - **Response:** MAY be included by default in the response.

* **[volume](../../properties/optimade/references/volume.md)** (property) - [`https://schemas.optimade.org/defs/v1.2/properties/optimade/references/volume`](https://schemas.optimade.org/defs/v1.2/properties/optimade/references/volume.md)  
  The volume number of a journal or multivolume book (the volume field in the BibTeX specification).

    **Requirements/Conventions:**  

    - **Support:** OPTIONAL support in implementations, i.e., MAY be `null`.
    - **Query:** Support for queries on this property is OPTIONAL.
    - **Response:** MAY be included by default in the response.

* **[year](../../properties/optimade/references/year.md)** (property) - [`https://schemas.optimade.org/defs/v1.2/properties/optimade/references/year`](https://schemas.optimade.org/defs/v1.2/properties/optimade/references/year.md)  
  The year of publication or writing.

    **Requirements/Conventions:**  

    - **Support:** OPTIONAL support in implementations, i.e., MAY be `null`.
    - **Query:** Support for queries on this property is OPTIONAL.
    - **Response:** MAY be included by default in the response.

* **[bibliographic type (bib_type)](../../properties/optimade/references/bib_type.md)** (property) - [`https://schemas.optimade.org/defs/v1.2/properties/optimade/references/bib_type`](https://schemas.optimade.org/defs/v1.2/properties/optimade/references/bib_type.md)  
  Type of the reference (the type field in the BibTeX specification).

    **Requirements/Conventions:**  

    - **Support:** OPTIONAL support in implementations, i.e., MAY be `null`.
    - **Query:** Support for queries on this property is OPTIONAL.
    - **Response:** MAY be included by default in the response.

* **[authors](../../properties/optimade/references/authors.md)** (property) - [`https://schemas.optimade.org/defs/v1.2/properties/optimade/references/authors`](https://schemas.optimade.org/defs/v1.2/properties/optimade/references/authors.md)  
  A list of dictionaries with names of the authors.

    **Requirements/Conventions:**  

    - **Support:** OPTIONAL support in implementations, i.e., MAY be `null`.
    - **Query:** Support for queries on this property is OPTIONAL.
    - **Response:** MAY be included by default in the response.
    - Each list member MUST be a dictionary with the following keys:
    
      - **name**: Full name of the person, REQUIRED.
      - **firstname**, **lastname**: Parts of the person's name, OPTIONAL.


* **[editors](../../properties/optimade/references/editors.md)** (property) - [`https://schemas.optimade.org/defs/v1.2/properties/optimade/references/editors`](https://schemas.optimade.org/defs/v1.2/properties/optimade/references/editors.md)  
  A list of dictionaries with names of the editors.

    **Requirements/Conventions:**  

    - **Support:** OPTIONAL support in implementations, i.e., MAY be `null`.
    - **Query:** Support for queries on this property is OPTIONAL.
    - **Response:** MAY be included by default in the response.
    - Each list member MUST be a dictionary with the following keys:
    
      - **name**: Full name of the person, REQUIRED.
      - **firstname**, **lastname**: Parts of the person's name, OPTIONAL.


* **[doi](../../properties/optimade/references/doi.md)** (property) - [`https://schemas.optimade.org/defs/v1.2/properties/optimade/references/doi`](https://schemas.optimade.org/defs/v1.2/properties/optimade/references/doi.md)  
  The doi identifier of the object being referenced.

    **Requirements/Conventions:**  

    - **Support:** OPTIONAL support in implementations, i.e., MAY be `null`.
    - **Query:** Support for queries on this property is OPTIONAL.
    - **Response:** MAY be included by default in the response.

* **[URL](../../properties/optimade/references/url.md)** (property) - [`https://schemas.optimade.org/defs/v1.2/properties/optimade/references/url`](https://schemas.optimade.org/defs/v1.2/properties/optimade/references/url.md)  
  The URL of the object being referenced.

    **Requirements/Conventions:**  

    - **Support:** OPTIONAL support in implementations, i.e., MAY be `null`.
    - **Query:** Support for queries on this property is OPTIONAL.
    - **Response:** MAY be included by default in the response.


**JSON definition:**

``` json
{
    "$id": "https://schemas.optimade.org/defs/v1.2/entrytypes/optimade/references",
    "$schema": "https://schemas.optimade.org/meta/v1.2/optimade/entrytype_definition.json",
    "title": "references",
    "description": "The references entry type describes a reference",
    "x-optimade-definition": {
        "label": "references_entrytype_optimade",
        "kind": "entrytype",
        "format": "1.2",
        "version": "1.2.0",
        "name": "references"
    },
    "type": "object",
    "properties": {
        "id": {
            "$id": "https://schemas.optimade.org/defs/v1.2/properties/core/id",
            "x-optimade-requirements": {
                "support": "must",
                "sortable": false,
                "query-support": "all mandatory",
                "response-level": "always"
            },
            "title": "ID",
            "x-optimade-type": "string",
            "x-optimade-definition": {
                "label": "id_core",
                "kind": "property",
                "version": "1.2.0",
                "format": "1.2",
                "name": "id"
            },
            "type": [
                "string"
            ],
            "description": "A unique string referencing a specific entry in the database.\n\n**Requirements/Conventions:**\n\n- Taken together, the ID and entry type MUST uniquely identify the entry.\n- Reasonably short IDs are encouraged and SHOULD NOT be longer than 255 characters.\n- IDs MAY change over time.",
            "examples": [
                "db/1234567",
                "cod/2000000",
                "cod/2000000@1234567",
                "nomad/L1234567890",
                "42"
            ],
            "x-optimade-unit": "inapplicable"
        },
        "type": {
            "$id": "https://schemas.optimade.org/defs/v1.2/properties/core/type",
            "x-optimade-requirements": {
                "support": "must",
                "sortable": false,
                "query-support": "all mandatory",
                "response-level": "always"
            },
            "title": "type",
            "x-optimade-type": "string",
            "x-optimade-definition": {
                "label": "type_core",
                "kind": "property",
                "version": "1.2.0",
                "format": "1.2",
                "name": "type"
            },
            "type": [
                "string"
            ],
            "description": "The name of the type of an entry.\n\n**Requirements/Conventions:**\n\n- MUST be an existing entry type.\n- The entry of type <type> and ID <id> MUST be returned in response to a request for /<type>/<id> under the versioned or unversioned base URL serving the API.",
            "examples": [
                "structures"
            ],
            "x-optimade-unit": "inapplicable"
        },
        "immutable_id": {
            "$id": "https://schemas.optimade.org/defs/v1.2/properties/core/immutable_id",
            "x-optimade-requirements": {
                "support": "may",
                "sortable": false,
                "query-support": "all mandatory",
                "response-level": "may"
            },
            "title": "immutable ID",
            "x-optimade-type": "string",
            "x-optimade-definition": {
                "label": "immutable_id_core",
                "kind": "property",
                "version": "1.2.0",
                "format": "1.2",
                "name": "immutable_id"
            },
            "type": [
                "string",
                "null"
            ],
            "description": "The entry's immutable ID (e.g., a UUID).\n\n**Requirements/Conventions:**\n\n- This is important for databases having preferred IDs that point to \"the latest version\" of a record, but still offer access to older variants.\n- This ID maps to the version-specific record, in case it changes in the future.",
            "examples": [
                "8bd3e750-b477-41a0-9b11-3a799f21b44f",
                "fjeiwoj,54;@=%<>#32"
            ],
            "x-optimade-unit": "inapplicable"
        },
        "last_modified": {
            "$id": "https://schemas.optimade.org/defs/v1.2/properties/core/last_modified",
            "x-optimade-requirements": {
                "support": "should",
                "sortable": false,
                "query-support": "all mandatory",
                "response-level": "must"
            },
            "title": "last modified",
            "x-optimade-type": "timestamp",
            "x-optimade-definition": {
                "label": "last_modified_core",
                "kind": "property",
                "version": "1.2.0",
                "format": "1.2",
                "name": "last_modified"
            },
            "type": [
                "string",
                "null"
            ],
            "format": "date-time",
            "description": "Date and time representing when the entry was last modified.",
            "examples": [
                "2007-04-05T14:30:20Z"
            ],
            "x-optimade-unit": "inapplicable"
        },
        "address": {
            "$id": "https://schemas.optimade.org/defs/v1.2/properties/optimade/references/address",
            "x-optimade-requirements": {
                "support": "may",
                "sortable": false,
                "query-support": "none",
                "response-level": "may"
            },
            "title": "address",
            "x-optimade-type": "string",
            "x-optimade-definition": {
                "label": "address_optimade_references",
                "kind": "property",
                "version": "1.2.0",
                "format": "1.2",
                "name": "address"
            },
            "type": [
                "string",
                "null"
            ],
            "description": "Typically the location of the publisher or institution (the address field in the BibTeX specification).",
            "examples": [
                "New York, NY"
            ],
            "x-optimade-unit": "inapplicable"
        },
        "annote": {
            "$id": "https://schemas.optimade.org/defs/v1.2/properties/optimade/references/annote",
            "x-optimade-requirements": {
                "support": "may",
                "sortable": false,
                "query-support": "none",
                "response-level": "may"
            },
            "title": "annote",
            "x-optimade-type": "string",
            "x-optimade-definition": {
                "label": "annote_optimade_references",
                "kind": "property",
                "version": "1.2.0",
                "format": "1.2",
                "name": "annote"
            },
            "type": [
                "string",
                "null"
            ],
            "description": "Additional notes or comments on the reference (the annote field in the BibTeX specification).",
            "examples": [
                "This article obtains structures via density-functional theory."
            ],
            "x-optimade-unit": "inapplicable"
        },
        "booktitle": {
            "$id": "https://schemas.optimade.org/defs/v1.2/properties/optimade/references/booktitle",
            "x-optimade-requirements": {
                "support": "may",
                "sortable": false,
                "query-support": "none",
                "response-level": "may"
            },
            "title": "booktitle",
            "x-optimade-type": "string",
            "x-optimade-definition": {
                "label": "booktitle_optimade_references",
                "kind": "property",
                "version": "1.2.0",
                "format": "1.2",
                "name": "booktitle"
            },
            "type": [
                "string",
                "null"
            ],
            "description": "The title of a book being cited; for parts of a book, use the title field instead (the booktitle field in the BibTeX specification).",
            "examples": [
                "Density-functional Theory of Atoms and Molecules"
            ],
            "x-optimade-unit": "inapplicable"
        },
        "chapter": {
            "$id": "https://schemas.optimade.org/defs/v1.2/properties/optimade/references/chapter",
            "x-optimade-requirements": {
                "support": "may",
                "sortable": false,
                "query-support": "none",
                "response-level": "may"
            },
            "title": "chapter",
            "x-optimade-type": "string",
            "x-optimade-definition": {
                "label": "chapter_optimade_references",
                "kind": "property",
                "version": "1.2.0",
                "format": "1.2",
                "name": "chapter"
            },
            "type": [
                "string",
                "null"
            ],
            "description": "The chapter, section, or similar part number (the chapter field in the BibTeX specification).",
            "examples": [
                "5"
            ],
            "x-optimade-unit": "inapplicable"
        },
        "crossref": {
            "$id": "https://schemas.optimade.org/defs/v1.2/properties/optimade/references/crossref",
            "x-optimade-requirements": {
                "support": "may",
                "sortable": false,
                "query-support": "none",
                "response-level": "may"
            },
            "title": "crossref",
            "x-optimade-type": "string",
            "x-optimade-definition": {
                "label": "crossref_optimade_references",
                "kind": "property",
                "version": "1.2.0",
                "format": "1.2",
                "name": "crossref"
            },
            "type": [
                "string",
                "null"
            ],
            "description": "The database key of the entry being cross referenced (the crossref field in the BibTeX specification).",
            "examples": [
                "smith2022"
            ],
            "x-optimade-unit": "inapplicable"
        },
        "edition": {
            "$id": "https://schemas.optimade.org/defs/v1.2/properties/optimade/references/edition",
            "x-optimade-requirements": {
                "support": "may",
                "sortable": false,
                "query-support": "none",
                "response-level": "may"
            },
            "title": "edition",
            "x-optimade-type": "string",
            "x-optimade-definition": {
                "label": "edition_optimade_references",
                "kind": "property",
                "version": "1.2.0",
                "format": "1.2",
                "name": "edition"
            },
            "type": [
                "string",
                "null"
            ],
            "description": "The edition of a book (the edition field in the BibTeX specification).",
            "examples": [
                "Second"
            ],
            "x-optimade-unit": "inapplicable"
        },
        "howpublished": {
            "$id": "https://schemas.optimade.org/defs/v1.2/properties/optimade/references/howpublished",
            "x-optimade-requirements": {
                "support": "may",
                "sortable": false,
                "query-support": "none",
                "response-level": "may"
            },
            "title": "how published",
            "x-optimade-type": "string",
            "x-optimade-definition": {
                "label": "howpublished_optimade_references",
                "kind": "property",
                "version": "1.2.0",
                "format": "1.2",
                "name": "howpublished"
            },
            "type": [
                "string",
                "null"
            ],
            "description": "The method of publication (the howpublished field in the BibTeX specification)",
            "examples": [
                "\\url{https://www.example.com/papers/example_paper}"
            ],
            "x-optimade-unit": "inapplicable"
        },
        "institution": {
            "$id": "https://schemas.optimade.org/defs/v1.2/properties/optimade/references/institution",
            "x-optimade-requirements": {
                "support": "may",
                "sortable": false,
                "query-support": "none",
                "response-level": "may"
            },
            "title": "institution",
            "x-optimade-type": "string",
            "x-optimade-definition": {
                "label": "institution_optimade_references",
                "kind": "property",
                "version": "1.2.0",
                "format": "1.2",
                "name": "institution"
            },
            "type": [
                "string",
                "null"
            ],
            "description": "The sponsoring institution of a technical report (the institution field in the BibTeX specification).",
            "examples": [
                "Massachusetts Institute of Technology"
            ],
            "x-optimade-unit": "inapplicable"
        },
        "journal": {
            "$id": "https://schemas.optimade.org/defs/v1.2/properties/optimade/references/journal",
            "x-optimade-requirements": {
                "support": "may",
                "sortable": false,
                "query-support": "none",
                "response-level": "may"
            },
            "title": "journal",
            "x-optimade-type": "string",
            "x-optimade-definition": {
                "label": "journal_optimade_references",
                "kind": "property",
                "version": "1.2.0",
                "format": "1.2",
                "name": "journal"
            },
            "type": [
                "string",
                "null"
            ],
            "description": "The name of a journal (the journal field in the BibTeX specification).",
            "examples": [
                "Journal of Environmental Science"
            ],
            "x-optimade-unit": "inapplicable"
        },
        "key": {
            "$id": "https://schemas.optimade.org/defs/v1.2/properties/optimade/references/key",
            "x-optimade-requirements": {
                "support": "may",
                "sortable": false,
                "query-support": "none",
                "response-level": "may"
            },
            "title": "key",
            "x-optimade-type": "string",
            "x-optimade-definition": {
                "label": "key_optimade_references",
                "kind": "property",
                "version": "1.2.0",
                "format": "1.2",
                "name": "key"
            },
            "type": [
                "string",
                "null"
            ],
            "description": "Used for alphabetizing, cross-referencing, and creating a label (the key field in the BibTeX specification).",
            "examples": [
                "smith2022"
            ],
            "x-optimade-unit": "inapplicable"
        },
        "month": {
            "$id": "https://schemas.optimade.org/defs/v1.2/properties/optimade/references/month",
            "x-optimade-requirements": {
                "support": "may",
                "sortable": false,
                "query-support": "none",
                "response-level": "may"
            },
            "title": "month",
            "x-optimade-type": "string",
            "x-optimade-definition": {
                "label": "month_optimade_references",
                "kind": "property",
                "version": "1.2.0",
                "format": "1.2",
                "name": "month"
            },
            "type": [
                "string",
                "null"
            ],
            "description": "The three-letter abbreviation of the month of publication or writing (the month field in the BibTeX specification).",
            "examples": [
                "jul"
            ],
            "x-optimade-unit": "inapplicable"
        },
        "note": {
            "$id": "https://schemas.optimade.org/defs/v1.2/properties/optimade/references/note",
            "x-optimade-requirements": {
                "support": "may",
                "sortable": false,
                "query-support": "none",
                "response-level": "may"
            },
            "title": "note",
            "x-optimade-type": "string",
            "x-optimade-definition": {
                "label": "note_optimade_references",
                "kind": "property",
                "version": "1.2.0",
                "format": "1.2",
                "name": "note"
            },
            "type": [
                "string",
                "null"
            ],
            "description": "Additional information about the reference (the note field in the BibTeX specification).",
            "examples": [
                "Accessed: 2022-11-04"
            ],
            "x-optimade-unit": "inapplicable"
        },
        "number": {
            "$id": "https://schemas.optimade.org/defs/v1.2/properties/optimade/references/number",
            "x-optimade-requirements": {
                "support": "may",
                "sortable": false,
                "query-support": "none",
                "response-level": "may"
            },
            "title": "number",
            "x-optimade-type": "string",
            "x-optimade-definition": {
                "label": "number_optimade_references",
                "kind": "property",
                "version": "1.2.0",
                "format": "1.2",
                "name": "number"
            },
            "type": [
                "string",
                "null"
            ],
            "description": "The number of a journal, magazine, technical report, or work in a series (the number field in the BibTeX specification).",
            "examples": [
                "3"
            ],
            "x-optimade-unit": "inapplicable"
        },
        "organization": {
            "$id": "https://schemas.optimade.org/defs/v1.2/properties/optimade/references/organization",
            "x-optimade-requirements": {
                "support": "may",
                "sortable": false,
                "query-support": "none",
                "response-level": "may"
            },
            "title": "organization",
            "x-optimade-type": "string",
            "x-optimade-definition": {
                "label": "organization_optimade_references",
                "kind": "property",
                "version": "1.2.0",
                "format": "1.2",
                "name": "organization"
            },
            "type": [
                "string",
                "null"
            ],
            "description": "The organization sponsoring a conference or publishing a manual (the organization field in the BibTeX specification)",
            "examples": [
                "International Association of Engineers"
            ],
            "x-optimade-unit": "inapplicable"
        },
        "pages": {
            "$id": "https://schemas.optimade.org/defs/v1.2/properties/optimade/references/pages",
            "x-optimade-requirements": {
                "support": "may",
                "sortable": false,
                "query-support": "none",
                "response-level": "may"
            },
            "title": "pages",
            "x-optimade-type": "string",
            "x-optimade-definition": {
                "label": "pages_optimade_references",
                "kind": "property",
                "version": "1.2.0",
                "format": "1.2",
                "name": "pages"
            },
            "type": [
                "string",
                "null"
            ],
            "description": "The page number(s) of the reference (the pages field in the BibTeX specification).",
            "examples": [
                "147--154"
            ],
            "x-optimade-unit": "inapplicable"
        },
        "publisher": {
            "$id": "https://schemas.optimade.org/defs/v1.2/properties/optimade/references/publisher",
            "x-optimade-requirements": {
                "support": "may",
                "sortable": false,
                "query-support": "none",
                "response-level": "may"
            },
            "title": "publisher",
            "x-optimade-type": "string",
            "x-optimade-definition": {
                "label": "publisher_optimade_references",
                "kind": "property",
                "version": "1.2.0",
                "format": "1.2",
                "name": "publisher"
            },
            "type": [
                "string",
                "null"
            ],
            "description": "The name of the publisher (the publisher field in the BibTeX specification).",
            "examples": [
                "ACM"
            ],
            "x-optimade-unit": "inapplicable"
        },
        "school": {
            "$id": "https://schemas.optimade.org/defs/v1.2/properties/optimade/references/school",
            "x-optimade-requirements": {
                "support": "may",
                "sortable": false,
                "query-support": "none",
                "response-level": "may"
            },
            "title": "school",
            "x-optimade-type": "string",
            "x-optimade-definition": {
                "label": "school_optimade_references",
                "kind": "property",
                "version": "1.2.0",
                "format": "1.2",
                "name": "school"
            },
            "type": [
                "string",
                "null"
            ],
            "description": "The name of the school where a thesis was written (the school field in the BibTeX specification).",
            "examples": [
                "Stanford University"
            ],
            "x-optimade-unit": "inapplicable"
        },
        "series": {
            "$id": "https://schemas.optimade.org/defs/v1.2/properties/optimade/references/series",
            "x-optimade-requirements": {
                "support": "may",
                "sortable": false,
                "query-support": "none",
                "response-level": "may"
            },
            "title": "series",
            "x-optimade-type": "string",
            "x-optimade-definition": {
                "label": "series_optimade_references",
                "kind": "property",
                "version": "1.2.0",
                "format": "1.2",
                "name": "series"
            },
            "type": [
                "string",
                "null"
            ],
            "description": "The name of a series or set of books (the series field in the BibTeX specification).",
            "examples": [
                "Lecture Notes in Computer Science"
            ],
            "x-optimade-unit": "inapplicable"
        },
        "title": {
            "$id": "https://schemas.optimade.org/defs/v1.2/properties/optimade/references/title",
            "x-optimade-requirements": {
                "support": "may",
                "sortable": false,
                "query-support": "none",
                "response-level": "may"
            },
            "title": "title",
            "x-optimade-type": "string",
            "x-optimade-definition": {
                "label": "title_optimade_references",
                "kind": "property",
                "version": "1.2.0",
                "format": "1.2",
                "name": "title"
            },
            "type": [
                "string",
                "null"
            ],
            "description": "The title of the work (the title field in the BibTeX specification).",
            "examples": [
                "A Study on the Effects of Sleep Deprivation on Cognitive Performance"
            ],
            "x-optimade-unit": "inapplicable"
        },
        "volume": {
            "$id": "https://schemas.optimade.org/defs/v1.2/properties/optimade/references/volume",
            "x-optimade-requirements": {
                "support": "may",
                "sortable": false,
                "query-support": "none",
                "response-level": "may"
            },
            "title": "volume",
            "x-optimade-type": "string",
            "x-optimade-definition": {
                "label": "volume_optimade_references",
                "kind": "property",
                "version": "1.2.0",
                "format": "1.2",
                "name": "volume"
            },
            "type": [
                "string",
                "null"
            ],
            "description": "The volume number of a journal or multivolume book (the volume field in the BibTeX specification).",
            "examples": [
                "14"
            ],
            "x-optimade-unit": "inapplicable"
        },
        "year": {
            "$id": "https://schemas.optimade.org/defs/v1.2/properties/optimade/references/year",
            "x-optimade-requirements": {
                "support": "may",
                "sortable": false,
                "query-support": "none",
                "response-level": "may"
            },
            "title": "year",
            "x-optimade-type": "string",
            "x-optimade-definition": {
                "label": "year_optimade_references",
                "kind": "property",
                "version": "1.2.0",
                "format": "1.2",
                "name": "year"
            },
            "type": [
                "string",
                "null"
            ],
            "description": "The year of publication or writing.",
            "examples": [
                "1984"
            ],
            "x-optimade-unit": "inapplicable"
        },
        "bib_type": {
            "$id": "https://schemas.optimade.org/defs/v1.2/properties/optimade/references/bib_type",
            "x-optimade-requirements": {
                "support": "may",
                "sortable": false,
                "query-support": "none",
                "response-level": "may"
            },
            "title": "bibliographic type",
            "x-optimade-type": "string",
            "x-optimade-definition": {
                "label": "bib_type_optimade_references",
                "kind": "property",
                "version": "1.2.0",
                "format": "1.2",
                "name": "bib_type"
            },
            "type": [
                "string",
                "null"
            ],
            "description": "Type of the reference (the type field in the BibTeX specification).",
            "examples": [
                "Research Note"
            ],
            "x-optimade-unit": "inapplicable"
        },
        "authors": {
            "$id": "https://schemas.optimade.org/defs/v1.2/properties/optimade/references/authors",
            "x-optimade-requirements": {
                "support": "may",
                "sortable": false,
                "query-support": "none",
                "response-level": "may"
            },
            "title": "authors",
            "x-optimade-type": "list",
            "x-optimade-definition": {
                "label": "authors_optimade_references",
                "kind": "property",
                "version": "1.2.0",
                "format": "1.2",
                "name": "authors"
            },
            "x-optimade-dimensions": {
                "names": [
                    "dim_authors"
                ]
            },
            "type": [
                "array",
                "null"
            ],
            "description": "A list of dictionaries with names of the authors.\n\n**Requirements/Conventions**:\n\n- Each list member MUST be a dictionary with the following keys:\n\n  - **name**: Full name of the person, REQUIRED.\n  - **firstname**, **lastname**: Parts of the person's name, OPTIONAL.",
            "items": {
                "$id": "https://schemas.optimade.org/defs/v1.2/properties/optimade/common/person",
                "title": "person",
                "x-optimade-type": "dictionary",
                "x-optimade-definition": {
                    "label": "person_optimade_common",
                    "kind": "property",
                    "version": "1.2.0",
                    "format": "1.2",
                    "name": "person"
                },
                "type": [
                    "object",
                    "null"
                ],
                "description": "A dictionary with name information about a person.\n\n**Requirements/Conventions**:\n\n- The dictionary MUST adhere to the following format:\n\n  - **name**: Full name of the person, REQUIRED.\n  - **firstname**, **lastname**: Parts of the person's name, OPTIONAL.",
                "required": [
                    "name"
                ],
                "properties": {
                    "name": {
                        "x-optimade-type": "string",
                        "x-optimade-unit": "inapplicable",
                        "type": [
                            "string"
                        ]
                    },
                    "firstname": {
                        "x-optimade-type": "string",
                        "x-optimade-unit": "inapplicable",
                        "type": [
                            "string"
                        ]
                    },
                    "lastname": {
                        "x-optimade-type": "string",
                        "x-optimade-unit": "inapplicable",
                        "type": [
                            "string"
                        ]
                    }
                },
                "examples": [
                    {
                        "name": "John Smith"
                    },
                    {
                        "name": "Arthur Dent",
                        "firstname": "Arthur",
                        "lastname": "Dent"
                    }
                ],
                "x-optimade-unit": "inapplicable"
            },
            "examples": [
                [
                    {
                        "name": "John Smith"
                    },
                    {
                        "name": "Arthur Dent",
                        "firstname": "Arthur",
                        "lastname": "Dent"
                    }
                ]
            ],
            "x-optimade-unit": "inapplicable"
        },
        "editors": {
            "$id": "https://schemas.optimade.org/defs/v1.2/properties/optimade/references/editors",
            "x-optimade-requirements": {
                "support": "may",
                "sortable": false,
                "query-support": "none",
                "response-level": "may"
            },
            "title": "editors",
            "x-optimade-type": "list",
            "x-optimade-definition": {
                "label": "editors_optimade_references",
                "kind": "property",
                "version": "1.2.0",
                "format": "1.2",
                "name": "editors"
            },
            "x-optimade-dimensions": {
                "names": [
                    "dim_editors"
                ]
            },
            "type": [
                "array",
                "null"
            ],
            "description": "A list of dictionaries with names of the editors.\n\n**Requirements/Conventions**:\n\n- Each list member MUST be a dictionary with the following keys:\n\n  - **name**: Full name of the person, REQUIRED.\n  - **firstname**, **lastname**: Parts of the person's name, OPTIONAL.",
            "items": {
                "$id": "https://schemas.optimade.org/defs/v1.2/properties/optimade/common/person",
                "title": "person",
                "x-optimade-type": "dictionary",
                "x-optimade-definition": {
                    "label": "person_optimade_common",
                    "kind": "property",
                    "version": "1.2.0",
                    "format": "1.2",
                    "name": "person"
                },
                "type": [
                    "object",
                    "null"
                ],
                "description": "A dictionary with name information about a person.\n\n**Requirements/Conventions**:\n\n- The dictionary MUST adhere to the following format:\n\n  - **name**: Full name of the person, REQUIRED.\n  - **firstname**, **lastname**: Parts of the person's name, OPTIONAL.",
                "required": [
                    "name"
                ],
                "properties": {
                    "name": {
                        "x-optimade-type": "string",
                        "x-optimade-unit": "inapplicable",
                        "type": [
                            "string"
                        ]
                    },
                    "firstname": {
                        "x-optimade-type": "string",
                        "x-optimade-unit": "inapplicable",
                        "type": [
                            "string"
                        ]
                    },
                    "lastname": {
                        "x-optimade-type": "string",
                        "x-optimade-unit": "inapplicable",
                        "type": [
                            "string"
                        ]
                    }
                },
                "examples": [
                    {
                        "name": "John Smith"
                    },
                    {
                        "name": "Arthur Dent",
                        "firstname": "Arthur",
                        "lastname": "Dent"
                    }
                ],
                "x-optimade-unit": "inapplicable"
            },
            "examples": [
                [
                    {
                        "name": "John Smith"
                    },
                    {
                        "name": "Arthur Dent",
                        "firstname": "Arthur",
                        "lastname": "Dent"
                    }
                ]
            ],
            "x-optimade-unit": "inapplicable"
        },
        "doi": {
            "$id": "https://schemas.optimade.org/defs/v1.2/properties/optimade/references/doi",
            "x-optimade-requirements": {
                "support": "may",
                "sortable": false,
                "query-support": "none",
                "response-level": "may"
            },
            "title": "doi",
            "x-optimade-type": "string",
            "x-optimade-definition": {
                "label": "doi_optimade_references",
                "kind": "property",
                "version": "1.2.0",
                "format": "1.2",
                "name": "doi"
            },
            "type": [
                "string",
                "null"
            ],
            "description": "The doi identifier of the object being referenced.",
            "examples": [
                "10.1103/PhysRev.136.B864"
            ],
            "x-optimade-unit": "inapplicable"
        },
        "url": {
            "$id": "https://schemas.optimade.org/defs/v1.2/properties/optimade/references/url",
            "x-optimade-requirements": {
                "support": "may",
                "sortable": false,
                "query-support": "none",
                "response-level": "may"
            },
            "title": "URL",
            "x-optimade-type": "string",
            "x-optimade-definition": {
                "label": "url_optimade_references",
                "kind": "property",
                "version": "1.2.0",
                "format": "1.2",
                "name": "url"
            },
            "type": [
                "string",
                "null"
            ],
            "description": "The URL of the object being referenced.",
            "examples": [
                "https://example.com/papers/my_paper"
            ],
            "x-optimade-unit": "inapplicable"
        }
    }
}
```
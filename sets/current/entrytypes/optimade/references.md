# References (entrytype)
This page documents an [OPTIMADE](https://www.optimade.org/) [Entrytype Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/sets/v1.2.0/entrytypes/optimade/references`](https://schemas.optimade.org/sets/v1.2.0/entrytypes/optimade/references)**  
**Definition name:** `references`

**Entrytype name:** References  
**Description:** The references entry type describes a reference  

**Formats:** [[JSON](references.json)] [[MD](references.md)]

This entrytype defines the following properties:

* **[ID](../../../../properties/v1.2.0/core/id)** (property) - [`https://schemas.optimade.org/properties/v1.2.0/core/id`](https://schemas.optimade.org/sets/v1.2.0/entrytypes/optimade/references)  
  A unique string referencing a specific entry in the database.

    **Requirements/Conventions:**  

    - **Support:** MUST be supported by all implementations, MUST NOT be `null`.
    - **Query:** MUST be a queryable property with support for all mandatory filter features.
    - **Response:** MUST always be included in the response.
    - Taken together, the ID and entry type MUST uniquely identify the entry.
    - Reasonably short IDs are encouraged and SHOULD NOT be longer than 255 characters.
    - IDs MAY change over time.


* **[Type](../../../../properties/v1.2.0/core/type)** (property) - [`https://schemas.optimade.org/properties/v1.2.0/core/type`](https://schemas.optimade.org/sets/v1.2.0/entrytypes/optimade/references)  
  The name of the type of an entry.

    **Requirements/Conventions:**  

    - **Support:** MUST be supported by all implementations, MUST NOT be `null`.
    - **Query:** MUST be a queryable property with support for all mandatory filter features.
    - **Response:** MUST always be included in the response.
    - MUST be an existing entry type.
    - The entry of type <type> and ID <id> MUST be returned in response to a request for /<type>/<id> under the versioned or unversioned base URL serving the API.


* **[Immutable ID (immutable_id)](../../../../properties/v1.2.0/core/immutable_id)** (property) - [`https://schemas.optimade.org/properties/v1.2.0/core/immutable_id`](https://schemas.optimade.org/sets/v1.2.0/entrytypes/optimade/references)  
  The entry's immutable ID (e.g., a UUID).

    **Requirements/Conventions:**  

    - **Support:** OPTIONAL support in implementations, i.e., MAY be `null`.
    - **Query:** MUST be a queryable property with support for all mandatory filter features.
    - **Response:** MAY be included by default in the response.
    - This is important for databases having preferred IDs that point to "the latest version" of a record, but still offer access to older variants.
    - This ID maps to the version-specific record, in case it changes in the future.


* **[Last modified (last_modified)](../../../../properties/v1.2.0/core/last_modified)** (property) - [`https://schemas.optimade.org/properties/v1.2.0/core/last_modified`](https://schemas.optimade.org/sets/v1.2.0/entrytypes/optimade/references)  
  Date and time representing when the entry was last modified.

    **Requirements/Conventions:**  

    - **Support:** SHOULD be supported by all implementations, i.e., SHOULD NOT be `null`.
    - **Query:** MUST be a queryable property with support for all mandatory filter features.
    - **Response:** MUST be included by default in the response.

* **[address](../../../../properties/v1.2.0/optimade/references/address)** (property) - [`https://schemas.optimade.org/properties/v1.2.0/optimade/references/address`](https://schemas.optimade.org/sets/v1.2.0/entrytypes/optimade/references)  
  Typically the location of the publisher or institution (the address field in the BibTeX specification).

    **Requirements/Conventions:**  

    - **Support:** OPTIONAL support in implementations, i.e., MAY be `null`.
    - **Query:** Support for queries on this property is OPTIONAL.
    - **Response:** MAY be included by default in the response.

* **[annote](../../../../properties/v1.2.0/optimade/references/annote)** (property) - [`https://schemas.optimade.org/properties/v1.2.0/optimade/references/annote`](https://schemas.optimade.org/sets/v1.2.0/entrytypes/optimade/references)  
  Additional notes or comments on the reference (the annote field in the BibTeX specification).

    **Requirements/Conventions:**  

    - **Support:** OPTIONAL support in implementations, i.e., MAY be `null`.
    - **Query:** Support for queries on this property is OPTIONAL.
    - **Response:** MAY be included by default in the response.

* **[booktitle](../../../../properties/v1.2.0/optimade/references/booktitle)** (property) - [`https://schemas.optimade.org/properties/v1.2.0/optimade/references/booktitle`](https://schemas.optimade.org/sets/v1.2.0/entrytypes/optimade/references)  
  The title of a book being cited; for parts of a book, use the title field instead (the booktitle field in the BibTeX specification).

    **Requirements/Conventions:**  

    - **Support:** OPTIONAL support in implementations, i.e., MAY be `null`.
    - **Query:** Support for queries on this property is OPTIONAL.
    - **Response:** MAY be included by default in the response.

* **[chapter](../../../../properties/v1.2.0/optimade/references/chapter)** (property) - [`https://schemas.optimade.org/properties/v1.2.0/optimade/references/chapter`](https://schemas.optimade.org/sets/v1.2.0/entrytypes/optimade/references)  
  The chapter, section, or similar part number (the chapter field in the BibTeX specification).

    **Requirements/Conventions:**  

    - **Support:** OPTIONAL support in implementations, i.e., MAY be `null`.
    - **Query:** Support for queries on this property is OPTIONAL.
    - **Response:** MAY be included by default in the response.

* **[crossref](../../../../properties/v1.2.0/optimade/references/crossref)** (property) - [`https://schemas.optimade.org/properties/v1.2.0/optimade/references/crossref`](https://schemas.optimade.org/sets/v1.2.0/entrytypes/optimade/references)  
  The database key of the entry being cross referenced (the crossref field in the BibTeX specification).

    **Requirements/Conventions:**  

    - **Support:** OPTIONAL support in implementations, i.e., MAY be `null`.
    - **Query:** Support for queries on this property is OPTIONAL.
    - **Response:** MAY be included by default in the response.

* **[edition](../../../../properties/v1.2.0/optimade/references/edition)** (property) - [`https://schemas.optimade.org/properties/v1.2.0/optimade/references/edition`](https://schemas.optimade.org/sets/v1.2.0/entrytypes/optimade/references)  
  The edition of a book (the edition field in the BibTeX specification).

    **Requirements/Conventions:**  

    - **Support:** OPTIONAL support in implementations, i.e., MAY be `null`.
    - **Query:** Support for queries on this property is OPTIONAL.
    - **Response:** MAY be included by default in the response.

* **[howpublished](../../../../properties/v1.2.0/optimade/references/howpublished)** (property) - [`https://schemas.optimade.org/properties/v1.2.0/optimade/references/howpublished`](https://schemas.optimade.org/sets/v1.2.0/entrytypes/optimade/references)  
  The method of publication (the howpublished field in the BibTeX specification)

    **Requirements/Conventions:**  

    - **Support:** OPTIONAL support in implementations, i.e., MAY be `null`.
    - **Query:** Support for queries on this property is OPTIONAL.
    - **Response:** MAY be included by default in the response.

* **[institution](../../../../properties/v1.2.0/optimade/references/institution)** (property) - [`https://schemas.optimade.org/properties/v1.2.0/optimade/references/institution`](https://schemas.optimade.org/sets/v1.2.0/entrytypes/optimade/references)  
  The sponsoring institution of a technical report (the institution field in the BibTeX specification).

    **Requirements/Conventions:**  

    - **Support:** OPTIONAL support in implementations, i.e., MAY be `null`.
    - **Query:** Support for queries on this property is OPTIONAL.
    - **Response:** MAY be included by default in the response.

* **[journal](../../../../properties/v1.2.0/optimade/references/journal)** (property) - [`https://schemas.optimade.org/properties/v1.2.0/optimade/references/journal`](https://schemas.optimade.org/sets/v1.2.0/entrytypes/optimade/references)  
  The name of a journal (the journal field in the BibTeX specification).

    **Requirements/Conventions:**  

    - **Support:** OPTIONAL support in implementations, i.e., MAY be `null`.
    - **Query:** Support for queries on this property is OPTIONAL.
    - **Response:** MAY be included by default in the response.

* **[key](../../../../properties/v1.2.0/optimade/references/key)** (property) - [`https://schemas.optimade.org/properties/v1.2.0/optimade/references/key`](https://schemas.optimade.org/sets/v1.2.0/entrytypes/optimade/references)  
  Used for alphabetizing, cross-referencing, and creating a label (the key field in the BibTeX specification).

    **Requirements/Conventions:**  

    - **Support:** OPTIONAL support in implementations, i.e., MAY be `null`.
    - **Query:** Support for queries on this property is OPTIONAL.
    - **Response:** MAY be included by default in the response.

* **[month](../../../../properties/v1.2.0/optimade/references/month)** (property) - [`https://schemas.optimade.org/properties/v1.2.0/optimade/references/month`](https://schemas.optimade.org/sets/v1.2.0/entrytypes/optimade/references)  
  The three letter abbreviation of the month of publication or writing (the month field in the BibTeX specification).

    **Requirements/Conventions:**  

    - **Support:** OPTIONAL support in implementations, i.e., MAY be `null`.
    - **Query:** Support for queries on this property is OPTIONAL.
    - **Response:** MAY be included by default in the response.

* **[note](../../../../properties/v1.2.0/optimade/references/note)** (property) - [`https://schemas.optimade.org/properties/v1.2.0/optimade/references/note`](https://schemas.optimade.org/sets/v1.2.0/entrytypes/optimade/references)  
  Additional information about the reference (the note field in the BibTeX specification).

    **Requirements/Conventions:**  

    - **Support:** OPTIONAL support in implementations, i.e., MAY be `null`.
    - **Query:** Support for queries on this property is OPTIONAL.
    - **Response:** MAY be included by default in the response.

* **[number](../../../../properties/v1.2.0/optimade/references/number)** (property) - [`https://schemas.optimade.org/properties/v1.2.0/optimade/references/number`](https://schemas.optimade.org/sets/v1.2.0/entrytypes/optimade/references)  
  The number of a journal, magazine, technical report, or work in a series (the number field in the BibTeX specification).

    **Requirements/Conventions:**  

    - **Support:** OPTIONAL support in implementations, i.e., MAY be `null`.
    - **Query:** Support for queries on this property is OPTIONAL.
    - **Response:** MAY be included by default in the response.

* **[organization](../../../../properties/v1.2.0/optimade/references/organization)** (property) - [`https://schemas.optimade.org/properties/v1.2.0/optimade/references/organization`](https://schemas.optimade.org/sets/v1.2.0/entrytypes/optimade/references)  
  The organization sponsoring a conference or publishing a manual (the organization field in the BibTeX specification)

    **Requirements/Conventions:**  

    - **Support:** OPTIONAL support in implementations, i.e., MAY be `null`.
    - **Query:** Support for queries on this property is OPTIONAL.
    - **Response:** MAY be included by default in the response.

* **[pages](../../../../properties/v1.2.0/optimade/references/pages)** (property) - [`https://schemas.optimade.org/properties/v1.2.0/optimade/references/pages`](https://schemas.optimade.org/sets/v1.2.0/entrytypes/optimade/references)  
  The page number(s) of the reference (the pages field in the BibTeX specification).

    **Requirements/Conventions:**  

    - **Support:** OPTIONAL support in implementations, i.e., MAY be `null`.
    - **Query:** Support for queries on this property is OPTIONAL.
    - **Response:** MAY be included by default in the response.

* **[publisher](../../../../properties/v1.2.0/optimade/references/publisher)** (property) - [`https://schemas.optimade.org/properties/v1.2.0/optimade/references/publisher`](https://schemas.optimade.org/sets/v1.2.0/entrytypes/optimade/references)  
  The name of the publisher (the publisher field in the BibTeX specification).

    **Requirements/Conventions:**  

    - **Support:** OPTIONAL support in implementations, i.e., MAY be `null`.
    - **Query:** Support for queries on this property is OPTIONAL.
    - **Response:** MAY be included by default in the response.

* **[school](../../../../properties/v1.2.0/optimade/references/school)** (property) - [`https://schemas.optimade.org/properties/v1.2.0/optimade/references/school`](https://schemas.optimade.org/sets/v1.2.0/entrytypes/optimade/references)  
  The name of the school where a thesis was written (the school field in the BibTeX specification).

    **Requirements/Conventions:**  

    - **Support:** OPTIONAL support in implementations, i.e., MAY be `null`.
    - **Query:** Support for queries on this property is OPTIONAL.
    - **Response:** MAY be included by default in the response.

* **[series](../../../../properties/v1.2.0/optimade/references/series)** (property) - [`https://schemas.optimade.org/properties/v1.2.0/optimade/references/series`](https://schemas.optimade.org/sets/v1.2.0/entrytypes/optimade/references)  
  The name of a series or set of books (the series field in the BibTeX specification).

    **Requirements/Conventions:**  

    - **Support:** OPTIONAL support in implementations, i.e., MAY be `null`.
    - **Query:** Support for queries on this property is OPTIONAL.
    - **Response:** MAY be included by default in the response.

* **[title](../../../../properties/v1.2.0/optimade/references/title)** (property) - [`https://schemas.optimade.org/properties/v1.2.0/optimade/references/title`](https://schemas.optimade.org/sets/v1.2.0/entrytypes/optimade/references)  
  The title of the work (the title field in the BibTeX specification).

    **Requirements/Conventions:**  

    - **Support:** OPTIONAL support in implementations, i.e., MAY be `null`.
    - **Query:** Support for queries on this property is OPTIONAL.
    - **Response:** MAY be included by default in the response.

* **[volume](../../../../properties/v1.2.0/optimade/references/volume)** (property) - [`https://schemas.optimade.org/properties/v1.2.0/optimade/references/volume`](https://schemas.optimade.org/sets/v1.2.0/entrytypes/optimade/references)  
  The volume number of a journal or multivolume book (the volume field in the BibTeX specification).

    **Requirements/Conventions:**  

    - **Support:** OPTIONAL support in implementations, i.e., MAY be `null`.
    - **Query:** Support for queries on this property is OPTIONAL.
    - **Response:** MAY be included by default in the response.

* **[year](../../../../properties/v1.2.0/optimade/references/year)** (property) - [`https://schemas.optimade.org/properties/v1.2.0/optimade/references/year`](https://schemas.optimade.org/sets/v1.2.0/entrytypes/optimade/references)  
  The year of publication or writing.

    **Requirements/Conventions:**  

    - **Support:** OPTIONAL support in implementations, i.e., MAY be `null`.
    - **Query:** Support for queries on this property is OPTIONAL.
    - **Response:** MAY be included by default in the response.

* **[bibliographic type (bib_type)](../../../../properties/v1.2.0/optimade/references/bib_type)** (property) - [`https://schemas.optimade.org/properties/v1.2.0/optimade/references/bib_type`](https://schemas.optimade.org/sets/v1.2.0/entrytypes/optimade/references)  
  Type of the reference (the type field in the BibTeX specification).

    **Requirements/Conventions:**  

    - **Support:** OPTIONAL support in implementations, i.e., MAY be `null`.
    - **Query:** Support for queries on this property is OPTIONAL.
    - **Response:** MAY be included by default in the response.

* **[authors](../../../../properties/v1.2.0/optimade/references/authors)** (property) - [`https://schemas.optimade.org/properties/v1.2.0/optimade/references/authors`](https://schemas.optimade.org/sets/v1.2.0/entrytypes/optimade/references)  
  A list of dictionaries with names of the authors.

    **Requirements/Conventions:**  

    - **Support:** OPTIONAL support in implementations, i.e., MAY be `null`.
    - **Query:** Support for queries on this property is OPTIONAL.
    - **Response:** MAY be included by default in the response.
    - Each list member MUST be a dictionary with the following keys:
    
      - **name**: Full name of the person, REQUIRED.
      - **firstname**, **lastname**: Parts of the person's name, OPTIONAL.


* **[editors](../../../../properties/v1.2.0/optimade/references/editors)** (property) - [`https://schemas.optimade.org/properties/v1.2.0/optimade/references/editors`](https://schemas.optimade.org/sets/v1.2.0/entrytypes/optimade/references)  
  A list of dictionaries with names of the editors.

    **Requirements/Conventions:**  

    - **Support:** OPTIONAL support in implementations, i.e., MAY be `null`.
    - **Query:** Support for queries on this property is OPTIONAL.
    - **Response:** MAY be included by default in the response.
    - Each list member MUST be a dictionary with the following keys:
    
      - **name**: Full name of the person, REQUIRED.
      - **firstname**, **lastname**: Parts of the person's name, OPTIONAL.


* **[doi](../../../../properties/v1.2.0/optimade/references/doi)** (property) - [`https://schemas.optimade.org/properties/v1.2.0/optimade/references/doi`](https://schemas.optimade.org/sets/v1.2.0/entrytypes/optimade/references)  
  The doi identifier of the object being referenced.

    **Requirements/Conventions:**  

    - **Support:** OPTIONAL support in implementations, i.e., MAY be `null`.
    - **Query:** Support for queries on this property is OPTIONAL.
    - **Response:** MAY be included by default in the response.

* **[url](../../../../properties/v1.2.0/optimade/references/url)** (property) - [`https://schemas.optimade.org/properties/v1.2.0/optimade/references/url`](https://schemas.optimade.org/sets/v1.2.0/entrytypes/optimade/references)  
  The URL of the object being referenced.

    **Requirements/Conventions:**  

    - **Support:** OPTIONAL support in implementations, i.e., MAY be `null`.
    - **Query:** Support for queries on this property is OPTIONAL.
    - **Response:** MAY be included by default in the response.


**JSON definition:**

``` json
{
    "$id": "https://schemas.optimade.org/sets/v1.2.0/entrytypes/optimade/references",
    "title": "References",
    "description": "The references entry type describes a reference",
    "x-optimade-definition": {
        "kind": "entrytype",
        "format": "1.2",
        "version": "1.2.0",
        "name": "references"
    },
    "type": "object",
    "properties": {
        "id": {
            "x-optimade-requirements": {
                "support": "must",
                "sortable": false,
                "query-support": "all mandatory",
                "response-level": "always"
            },
            "$id": "https://schemas.optimade.org/properties/v1.2.0/core/id",
            "title": "ID",
            "x-optimade-type": "string",
            "x-optimade-definition": {
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
            "x-optimade-requirements": {
                "support": "must",
                "sortable": false,
                "query-support": "all mandatory",
                "response-level": "always"
            },
            "$id": "https://schemas.optimade.org/properties/v1.2.0/core/type",
            "title": "Type",
            "x-optimade-type": "string",
            "x-optimade-definition": {
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
            "x-optimade-requirements": {
                "support": "may",
                "sortable": false,
                "query-support": "all mandatory",
                "response-level": "may"
            },
            "$id": "https://schemas.optimade.org/properties/v1.2.0/core/immutable_id",
            "title": "Immutable ID",
            "x-optimade-type": "string",
            "x-optimade-definition": {
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
            "x-optimade-requirements": {
                "support": "should",
                "sortable": false,
                "query-support": "all mandatory",
                "response-level": "must"
            },
            "$id": "https://schemas.optimade.org/properties/v1.2.0/core/last_modified",
            "title": "Last modified",
            "x-optimade-type": "timestamp",
            "x-optimade-definition": {
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
            "x-optimade-requirements": {
                "support": "may",
                "sortable": false,
                "query-support": "none",
                "response-level": "may"
            },
            "$id": "https://schemas.optimade.org/properties/v1.2.0/optimade/references/address",
            "title": "address",
            "x-optimade-type": "string",
            "x-optimade-definition": {
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
            "x-optimade-requirements": {
                "support": "may",
                "sortable": false,
                "query-support": "none",
                "response-level": "may"
            },
            "$id": "https://schemas.optimade.org/properties/v1.2.0/optimade/references/annote",
            "title": "annote",
            "x-optimade-type": "string",
            "x-optimade-definition": {
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
            "x-optimade-requirements": {
                "support": "may",
                "sortable": false,
                "query-support": "none",
                "response-level": "may"
            },
            "$id": "https://schemas.optimade.org/properties/v1.2.0/optimade/references/booktitle",
            "title": "booktitle",
            "x-optimade-type": "string",
            "x-optimade-definition": {
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
            "x-optimade-requirements": {
                "support": "may",
                "sortable": false,
                "query-support": "none",
                "response-level": "may"
            },
            "$id": "https://schemas.optimade.org/properties/v1.2.0/optimade/references/chapter",
            "title": "chapter",
            "x-optimade-type": "string",
            "x-optimade-definition": {
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
            "x-optimade-requirements": {
                "support": "may",
                "sortable": false,
                "query-support": "none",
                "response-level": "may"
            },
            "$id": "https://schemas.optimade.org/properties/v1.2.0/optimade/references/crossref",
            "title": "crossref",
            "x-optimade-type": "string",
            "x-optimade-definition": {
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
            "x-optimade-requirements": {
                "support": "may",
                "sortable": false,
                "query-support": "none",
                "response-level": "may"
            },
            "$id": "https://schemas.optimade.org/properties/v1.2.0/optimade/references/edition",
            "title": "edition",
            "x-optimade-type": "string",
            "x-optimade-definition": {
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
            "x-optimade-requirements": {
                "support": "may",
                "sortable": false,
                "query-support": "none",
                "response-level": "may"
            },
            "$id": "https://schemas.optimade.org/properties/v1.2.0/optimade/references/howpublished",
            "title": "howpublished",
            "x-optimade-type": "string",
            "x-optimade-definition": {
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
            "x-optimade-requirements": {
                "support": "may",
                "sortable": false,
                "query-support": "none",
                "response-level": "may"
            },
            "$id": "https://schemas.optimade.org/properties/v1.2.0/optimade/references/institution",
            "title": "institution",
            "x-optimade-type": "string",
            "x-optimade-definition": {
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
            "x-optimade-requirements": {
                "support": "may",
                "sortable": false,
                "query-support": "none",
                "response-level": "may"
            },
            "$id": "https://schemas.optimade.org/properties/v1.2.0/optimade/references/journal",
            "title": "journal",
            "x-optimade-type": "string",
            "x-optimade-definition": {
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
            "x-optimade-requirements": {
                "support": "may",
                "sortable": false,
                "query-support": "none",
                "response-level": "may"
            },
            "$id": "https://schemas.optimade.org/properties/v1.2.0/optimade/references/key",
            "title": "key",
            "x-optimade-type": "string",
            "x-optimade-definition": {
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
            "x-optimade-requirements": {
                "support": "may",
                "sortable": false,
                "query-support": "none",
                "response-level": "may"
            },
            "$id": "https://schemas.optimade.org/properties/v1.2.0/optimade/references/month",
            "title": "month",
            "x-optimade-type": "string",
            "x-optimade-definition": {
                "kind": "property",
                "version": "1.2.0",
                "format": "1.2",
                "name": "month"
            },
            "type": [
                "string",
                "null"
            ],
            "description": "The three letter abbreviation of the month of publication or writing (the month field in the BibTeX specification).",
            "examples": [
                "jul"
            ],
            "x-optimade-unit": "inapplicable"
        },
        "note": {
            "x-optimade-requirements": {
                "support": "may",
                "sortable": false,
                "query-support": "none",
                "response-level": "may"
            },
            "$id": "https://schemas.optimade.org/properties/v1.2.0/optimade/references/note",
            "title": "note",
            "x-optimade-type": "string",
            "x-optimade-definition": {
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
            "x-optimade-requirements": {
                "support": "may",
                "sortable": false,
                "query-support": "none",
                "response-level": "may"
            },
            "$id": "https://schemas.optimade.org/properties/v1.2.0/optimade/references/number",
            "title": "number",
            "x-optimade-type": "string",
            "x-optimade-definition": {
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
            "x-optimade-requirements": {
                "support": "may",
                "sortable": false,
                "query-support": "none",
                "response-level": "may"
            },
            "$id": "https://schemas.optimade.org/properties/v1.2.0/optimade/references/organization",
            "title": "organization",
            "x-optimade-type": "string",
            "x-optimade-definition": {
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
            "x-optimade-requirements": {
                "support": "may",
                "sortable": false,
                "query-support": "none",
                "response-level": "may"
            },
            "$id": "https://schemas.optimade.org/properties/v1.2.0/optimade/references/pages",
            "title": "pages",
            "x-optimade-type": "string",
            "x-optimade-definition": {
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
            "x-optimade-requirements": {
                "support": "may",
                "sortable": false,
                "query-support": "none",
                "response-level": "may"
            },
            "$id": "https://schemas.optimade.org/properties/v1.2.0/optimade/references/publisher",
            "title": "publisher",
            "x-optimade-type": "string",
            "x-optimade-definition": {
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
            "x-optimade-requirements": {
                "support": "may",
                "sortable": false,
                "query-support": "none",
                "response-level": "may"
            },
            "$id": "https://schemas.optimade.org/properties/v1.2.0/optimade/references/school",
            "title": "school",
            "x-optimade-type": "string",
            "x-optimade-definition": {
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
            "x-optimade-requirements": {
                "support": "may",
                "sortable": false,
                "query-support": "none",
                "response-level": "may"
            },
            "$id": "https://schemas.optimade.org/properties/v1.2.0/optimade/references/series",
            "title": "series",
            "x-optimade-type": "string",
            "x-optimade-definition": {
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
            "x-optimade-requirements": {
                "support": "may",
                "sortable": false,
                "query-support": "none",
                "response-level": "may"
            },
            "$id": "https://schemas.optimade.org/properties/v1.2.0/optimade/references/title",
            "title": "title",
            "x-optimade-type": "string",
            "x-optimade-definition": {
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
            "x-optimade-requirements": {
                "support": "may",
                "sortable": false,
                "query-support": "none",
                "response-level": "may"
            },
            "$id": "https://schemas.optimade.org/properties/v1.2.0/optimade/references/volume",
            "title": "volume",
            "x-optimade-type": "string",
            "x-optimade-definition": {
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
            "x-optimade-requirements": {
                "support": "may",
                "sortable": false,
                "query-support": "none",
                "response-level": "may"
            },
            "$id": "https://schemas.optimade.org/properties/v1.2.0/optimade/references/year",
            "title": "year",
            "x-optimade-type": "string",
            "x-optimade-definition": {
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
            "x-optimade-requirements": {
                "support": "may",
                "sortable": false,
                "query-support": "none",
                "response-level": "may"
            },
            "$id": "https://schemas.optimade.org/properties/v1.2.0/optimade/references/bib_type",
            "title": "bibliographic type",
            "x-optimade-type": "string",
            "x-optimade-definition": {
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
            "x-optimade-requirements": {
                "support": "may",
                "sortable": false,
                "query-support": "none",
                "response-level": "may"
            },
            "$id": "https://schemas.optimade.org/properties/v1.2.0/optimade/references/authors",
            "title": "authors",
            "x-optimade-type": "list",
            "x-optimade-definition": {
                "kind": "property",
                "version": "1.2.0",
                "format": "1.2",
                "name": "authors"
            },
            "type": [
                "array",
                "null"
            ],
            "description": "A list of dictionaries with names of the authors.\n\n**Requirements/Conventions**:\n\n- Each list member MUST be a dictionary with the following keys:\n\n  - **name**: Full name of the person, REQUIRED.\n  - **firstname**, **lastname**: Parts of the person's name, OPTIONAL.",
            "items": {
                "$id": "https://schemas.optimade.org/properties/v1.2.0/optimade/common/person",
                "title": "authors",
                "x-optimade-type": "dictionary",
                "x-optimade-definition": {
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
            "x-optimade-requirements": {
                "support": "may",
                "sortable": false,
                "query-support": "none",
                "response-level": "may"
            },
            "$id": "https://schemas.optimade.org/properties/v1.2.0/optimade/references/editors",
            "title": "editors",
            "x-optimade-type": "list",
            "x-optimade-definition": {
                "kind": "property",
                "version": "1.2.0",
                "format": "1.2",
                "name": "editors"
            },
            "type": [
                "array",
                "null"
            ],
            "description": "A list of dictionaries with names of the editors.\n\n**Requirements/Conventions**:\n\n- Each list member MUST be a dictionary with the following keys:\n\n  - **name**: Full name of the person, REQUIRED.\n  - **firstname**, **lastname**: Parts of the person's name, OPTIONAL.",
            "items": {
                "$id": "https://schemas.optimade.org/properties/v1.2.0/optimade/common/person",
                "title": "authors",
                "x-optimade-type": "dictionary",
                "x-optimade-definition": {
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
            "x-optimade-requirements": {
                "support": "may",
                "sortable": false,
                "query-support": "none",
                "response-level": "may"
            },
            "$id": "https://schemas.optimade.org/properties/v1.2.0/optimade/references/doi",
            "title": "doi",
            "x-optimade-type": "string",
            "x-optimade-definition": {
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
            "x-optimade-requirements": {
                "support": "may",
                "sortable": false,
                "query-support": "none",
                "response-level": "may"
            },
            "$id": "https://schemas.optimade.org/properties/v1.2.0/optimade/references/url",
            "title": "url",
            "x-optimade-type": "string",
            "x-optimade-definition": {
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
    },
    "$schema": "https://schemas.optimade.org/meta/v1.2.0/optimade/entrytype_definition.md"
}
```
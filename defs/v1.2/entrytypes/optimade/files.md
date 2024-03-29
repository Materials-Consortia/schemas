# files (entrytype)

This page documents an [OPTIMADE](https://www.optimade.org/) [Entrytype Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/defs/v1.2/entrytypes/optimade/files`](https://schemas.optimade.org/defs/v1.2/entrytypes/optimade/files.md)**  
**Definition name:** `files`

**Entrytype name:** files  
**Description:** The files entry type describes a file with metadata and a URL to retrieve it  

**Formats:** [[JSON](files.json)] [[MD](files.md)]

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

* **[URL](../../properties/optimade/files/url.md)** (property) - [`https://schemas.optimade.org/defs/v1.2/properties/optimade/files/url`](https://schemas.optimade.org/defs/v1.2/properties/optimade/files/url.md)  
  The URL to get the contents of a file.

    **Requirements/Conventions:**  

    - **Support:** MUST be supported by all implementations, MUST NOT be `null`.
    - **Query:** Support for queries on this property is OPTIONAL.
    - **Response:** MUST be included by default in the response.
    - The URL MUST point to the actual contents of a file (i.e. byte stream), not an intermediate (preview) representation. For example, if referring to a file on GitHub, a link should point to raw contents.


* **[URL stable until (url_stable_until)](../../properties/optimade/files/url_stable_until.md)** (property) - [`https://schemas.optimade.org/defs/v1.2/properties/optimade/files/url_stable_until`](https://schemas.optimade.org/defs/v1.2/properties/optimade/files/url_stable_until.md)  
  Point in time until which the URL in `url` is guaranteed to stay stable.

    **Requirements/Conventions:**  

    - **Support:** OPTIONAL support in implementations, i.e., MAY be `null`.
    - **Query:** Support for queries on this property is OPTIONAL.
    - **Response:** MAY be included by default in the response.
    - `null` means that there is no stability guarantee for the URL in `url`.
      Indefinite support could be communicated by providing a date sufficiently far in the future, for example, 9999-12-31.


* **[name](../../properties/optimade/files/name.md)** (property) - [`https://schemas.optimade.org/defs/v1.2/properties/optimade/files/name`](https://schemas.optimade.org/defs/v1.2/properties/optimade/files/name.md)  
  Base name of a file.

    **Requirements/Conventions:**  

    - **Support:** SHOULD be supported by all implementations, i.e., SHOULD NOT be `null`.
    - **Query:** Support for queries on this property is OPTIONAL.
    - **Response:** MAY be included by default in the response.
    - File name extension is an integral part of a file name and, if available, MUST be included.


* **[size](../../properties/optimade/files/size.md)** (property) - [`https://schemas.optimade.org/defs/v1.2/properties/optimade/files/size`](https://schemas.optimade.org/defs/v1.2/properties/optimade/files/size.md)  
  Size of a file in bytes.

    **Requirements/Conventions:**  

    - **Support:** OPTIONAL support in implementations, i.e., MAY be `null`.
    - **Query:** Support for queries on this property is OPTIONAL.
    - **Response:** MAY be included by default in the response.
    - If provided, it MUST be guaranteed that either exact size of a file is given or its upper bound.
      This way if a client reserves a static buffer or truncates the download stream after this many bytes the whole file would be received.
      Such provision is included to allow the providers to serve on-the-fly compressed files.


* **[media type (media_type)](../../properties/optimade/files/media_type.md)** (property) - [`https://schemas.optimade.org/defs/v1.2/properties/optimade/files/media_type`](https://schemas.optimade.org/defs/v1.2/properties/optimade/files/media_type.md)  
  Media type identifier (also known as MIME type), for a file as per [RFC 6838 Media Type Specifications and Registration Procedures](https://datatracker.ietf.org/doc/html/rfc6838).

    **Requirements/Conventions:**  

    - **Support:** OPTIONAL support in implementations, i.e., MAY be `null`.
    - **Query:** Support for queries on this property is OPTIONAL.
    - **Response:** MAY be included by default in the response.

* **[version](../../properties/optimade/files/version.md)** (property) - [`https://schemas.optimade.org/defs/v1.2/properties/optimade/files/version`](https://schemas.optimade.org/defs/v1.2/properties/optimade/files/version.md)  
  Version information of a file (e.g., commit, revision, timestamp).

    **Requirements/Conventions:**  

    - **Support:** OPTIONAL support in implementations, i.e., MAY be `null`.
    - **Query:** Support for queries on this property is OPTIONAL.
    - **Response:** MAY be included by default in the response.
    - If provided, it MUST be guaranteed that file contents pertaining to the same combination of id and version are the same.


* **[modification timestamp (modification_timestamp)](../../properties/optimade/files/modification_timestamp.md)** (property) - [`https://schemas.optimade.org/defs/v1.2/properties/optimade/files/modification_timestamp`](https://schemas.optimade.org/defs/v1.2/properties/optimade/files/modification_timestamp.md)  
  Timestamp of the last modification of file contents. A modification is understood as an addition, change or deletion of one or more bytes, resulting in file contents different from the previous.

    **Requirements/Conventions:**  

    - **Support:** OPTIONAL support in implementations, i.e., MAY be `null`.
    - **Query:** Support for queries on this property is OPTIONAL.
    - **Response:** MAY be included by default in the response.
    - Timestamps of subsequent file modifications SHOULD be increasing (not earlier than previous timestamps).


* **[description](../../properties/optimade/files/description.md)** (property) - [`https://schemas.optimade.org/defs/v1.2/properties/optimade/files/description`](https://schemas.optimade.org/defs/v1.2/properties/optimade/files/description.md)  
  Free-form description of a file.

    **Requirements/Conventions:**  

    - **Support:** OPTIONAL support in implementations, i.e., MAY be `null`.
    - **Query:** Support for queries on this property is OPTIONAL.
    - **Response:** MAY be included by default in the response.

* **[checksums](../../properties/optimade/files/checksums.md)** (property) - [`https://schemas.optimade.org/defs/v1.2/properties/optimade/files/checksums`](https://schemas.optimade.org/defs/v1.2/properties/optimade/files/checksums.md)  
  Dictionary providing checksums of file contents.

    **Requirements/Conventions:**  

    - **Support:** OPTIONAL support in implementations, i.e., MAY be `null`.
    - **Query:** Support for queries on this property is OPTIONAL.
    - **Response:** MAY be included by default in the response.
    - The keys in the dictionary identify checksum functions and the values are strings containing the corresponding checksum.
    
    - Supported dictionary keys: `md5`, `sha1`, `sha224`, `sha256`, `sha384`, `sha512`.
      Checksums outside this list MAY be used, but their names MUST be prefixed by database-provider-specific namespace prefix.


* **[access time (atime)](../../properties/optimade/files/atime.md)** (property) - [`https://schemas.optimade.org/defs/v1.2/properties/optimade/files/atime`](https://schemas.optimade.org/defs/v1.2/properties/optimade/files/atime.md)  
  Time of last access of a file as per POSIX standard.

    **Requirements/Conventions:**  

    - **Support:** OPTIONAL support in implementations, i.e., MAY be `null`.
    - **Query:** Support for queries on this property is OPTIONAL.
    - **Response:** MAY be included by default in the response.

* **[change time (ctime)](../../properties/optimade/files/ctime.md)** (property) - [`https://schemas.optimade.org/defs/v1.2/properties/optimade/files/ctime`](https://schemas.optimade.org/defs/v1.2/properties/optimade/files/ctime.md)  
  Time of last status change of a file as per POSIX standard.

    **Requirements/Conventions:**  

    - **Support:** OPTIONAL support in implementations, i.e., MAY be `null`.
    - **Query:** Support for queries on this property is OPTIONAL.
    - **Response:** MAY be included by default in the response.

* **[modification time (mtime)](../../properties/optimade/files/mtime.md)** (property) - [`https://schemas.optimade.org/defs/v1.2/properties/optimade/files/mtime`](https://schemas.optimade.org/defs/v1.2/properties/optimade/files/mtime.md)  
  Time of last modification of a file as per POSIX standard.

    **Requirements/Conventions:**  

    - **Support:** OPTIONAL support in implementations, i.e., MAY be `null`.
    - **Query:** Support for queries on this property is OPTIONAL.
    - **Response:** MAY be included by default in the response.
    - It should be noted that the values of `last_modified`, `modification_timestamp` and `mtime` do not necessary match.
      `last_modified` pertains to the modification of the OPTIMADE metadata, `modification_timestamp` pertains to file contents and `mtime` pertains to the modification of the file (not necessary changing its contents).
      For example, appending an empty string to a file would result in the change of `mtime` in some operating systems, but this would not be deemed as a modification of its contents.



**JSON definition:**

``` json
{
    "$id": "https://schemas.optimade.org/defs/v1.2/entrytypes/optimade/files",
    "$schema": "https://schemas.optimade.org/meta/v1.2/optimade/entrytype_definition.json",
    "title": "files",
    "description": "The files entry type describes a file with metadata and a URL to retrieve it",
    "x-optimade-definition": {
        "label": "files_entrytype_optimade",
        "kind": "entrytype",
        "format": "1.2",
        "version": "1.2.0",
        "name": "files"
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
        "url": {
            "$id": "https://schemas.optimade.org/defs/v1.2/properties/optimade/files/url",
            "x-optimade-requirements": {
                "support": "must",
                "sortable": false,
                "query-support": "none",
                "response-level": "must"
            },
            "title": "URL",
            "x-optimade-type": "string",
            "x-optimade-definition": {
                "label": "url_optimade_files",
                "kind": "property",
                "version": "1.2.0",
                "format": "1.2",
                "name": "url"
            },
            "type": [
                "string"
            ],
            "description": "The URL to get the contents of a file.\n\n**Requirements/Conventions:**\n\n- The URL MUST point to the actual contents of a file (i.e. byte stream), not an intermediate (preview) representation. For example, if referring to a file on GitHub, a link should point to raw contents.",
            "examples": [
                "https://example.org/files/cifs/1000000.cif"
            ],
            "x-optimade-unit": "inapplicable"
        },
        "url_stable_until": {
            "$id": "https://schemas.optimade.org/defs/v1.2/properties/optimade/files/url_stable_until",
            "x-optimade-requirements": {
                "support": "may",
                "sortable": false,
                "query-support": "none",
                "response-level": "may"
            },
            "title": "URL stable until",
            "x-optimade-type": "timestamp",
            "x-optimade-definition": {
                "label": "url_stable_until_optimade_files",
                "kind": "property",
                "version": "1.2.0",
                "format": "1.2",
                "name": "url_stable_until"
            },
            "type": [
                "string",
                "null"
            ],
            "description": "Point in time until which the URL in `url` is guaranteed to stay stable.\n\n**Requirements/Conventions:**\n\n- `null` means that there is no stability guarantee for the URL in `url`.\n  Indefinite support could be communicated by providing a date sufficiently far in the future, for example, 9999-12-31.",
            "examples": [
                "2052-04-05T14:30:20Z"
            ],
            "x-optimade-unit": "inapplicable",
            "format": "date-time"
        },
        "name": {
            "$id": "https://schemas.optimade.org/defs/v1.2/properties/optimade/files/name",
            "x-optimade-requirements": {
                "support": "should",
                "sortable": false,
                "query-support": "none",
                "response-level": "may"
            },
            "title": "name",
            "x-optimade-type": "string",
            "x-optimade-definition": {
                "label": "name_optimade_files",
                "kind": "property",
                "version": "1.2.0",
                "format": "1.2",
                "name": "name"
            },
            "type": [
                "string"
            ],
            "description": "Base name of a file.\n\n**Requirements/Conventions:**\n\n- File name extension is an integral part of a file name and, if available, MUST be included.",
            "examples": [
                "1000000.cif"
            ],
            "x-optimade-unit": "inapplicable"
        },
        "size": {
            "$id": "https://schemas.optimade.org/defs/v1.2/properties/optimade/files/size",
            "x-optimade-requirements": {
                "support": "may",
                "sortable": false,
                "query-support": "none",
                "response-level": "may"
            },
            "title": "size",
            "x-optimade-type": "integer",
            "x-optimade-definition": {
                "label": "size_optimade_files",
                "kind": "property",
                "version": "1.2.0",
                "format": "1.2",
                "name": "size"
            },
            "x-optimade-unit-definitions": [
                {
                    "$id": "https://schemas.optimade.org/defs/v1.2/units/iso-iec-80000/2008/information_science_and_technology/byte",
                    "title": "byte",
                    "symbol": "B",
                    "display-symbol": "B",
                    "description": "A unit of digital information representing eight bits, defined in the International System of Quantities in ISO/IEC 80000-13 (2008).\n\n\"In English, the name byte, symbol B, is used as a synonym for octet. Here byte means an eight-bit byte.\" [ISO/IEC 80000-13 (2008)]",
                    "resources": [
                        {
                            "relation": "Defining standard",
                            "resource-id": "https://www.iso.org/standard/31898.html"
                        },
                        {
                            "relation": "Wikipedia article describing the unit",
                            "resource-id": "https://en.wikipedia.org/wiki/Byte"
                        }
                    ],
                    "defining-relation": {
                        "base-units": [
                            {
                                "symbol": "bit",
                                "id": "https://schemas.optimade.org/defs/v1.2/units/independent/1948/information/bit"
                            }
                        ],
                        "base-units-expression": "bit",
                        "scale": {
                            "numerator": 8
                        }
                    },
                    "standard": {
                        "name": "iso-iec-80000",
                        "year": 2008,
                        "category": "information_science_and_technology",
                        "symbol": "B"
                    },
                    "x-optimade-definition": {
                        "label": "byte_iso_iec_80000_2008_information_science_and_technology",
                        "kind": "unit",
                        "format": "1.2",
                        "version": "1.2.0",
                        "name": "byte"
                    }
                }
            ],
            "type": [
                "integer",
                "null"
            ],
            "description": "Size of a file in bytes.\n\n**Requirements/Conventions:**\n\n- If provided, it MUST be guaranteed that either exact size of a file is given or its upper bound.\n  This way if a client reserves a static buffer or truncates the download stream after this many bytes the whole file would be received.\n  Such provision is included to allow the providers to serve on-the-fly compressed files.",
            "examples": [
                4711
            ],
            "x-optimade-unit": "byte"
        },
        "media_type": {
            "$id": "https://schemas.optimade.org/defs/v1.2/properties/optimade/files/media_type",
            "x-optimade-requirements": {
                "support": "may",
                "sortable": false,
                "query-support": "none",
                "response-level": "may"
            },
            "title": "media type",
            "x-optimade-type": "string",
            "x-optimade-definition": {
                "label": "media_type_optimade_files",
                "kind": "property",
                "version": "1.2.0",
                "format": "1.2",
                "name": "media_type"
            },
            "type": [
                "string",
                "null"
            ],
            "description": "Media type identifier (also known as MIME type), for a file as per [RFC 6838 Media Type Specifications and Registration Procedures](https://datatracker.ietf.org/doc/html/rfc6838).",
            "examples": [
                "chemical/x-cif"
            ],
            "x-optimade-unit": "inapplicable"
        },
        "version": {
            "$id": "https://schemas.optimade.org/defs/v1.2/properties/optimade/files/version",
            "x-optimade-requirements": {
                "support": "may",
                "sortable": false,
                "query-support": "none",
                "response-level": "may"
            },
            "title": "version",
            "x-optimade-type": "string",
            "x-optimade-definition": {
                "label": "version_optimade_files",
                "kind": "property",
                "version": "1.2.0",
                "format": "1.2",
                "name": "version"
            },
            "type": [
                "string",
                "null"
            ],
            "description": "Version information of a file (e.g., commit, revision, timestamp).\n\n**Requirements/Conventions:**\n\n- If provided, it MUST be guaranteed that file contents pertaining to the same combination of id and version are the same.",
            "examples": [
                "3.2.6"
            ],
            "x-optimade-unit": "inapplicable"
        },
        "modification_timestamp": {
            "$id": "https://schemas.optimade.org/defs/v1.2/properties/optimade/files/modification_timestamp",
            "x-optimade-requirements": {
                "support": "may",
                "sortable": false,
                "query-support": "none",
                "response-level": "may"
            },
            "title": "modification timestamp",
            "x-optimade-type": "timestamp",
            "x-optimade-definition": {
                "label": "modification_timestamp_optimade_files",
                "kind": "property",
                "version": "1.2.0",
                "format": "1.2",
                "name": "modification_timestamp"
            },
            "type": [
                "string",
                "null"
            ],
            "description": "Timestamp of the last modification of file contents. A modification is understood as an addition, change or deletion of one or more bytes, resulting in file contents different from the previous.\n\n**Requirements/Conventions:**\n\n- Timestamps of subsequent file modifications SHOULD be increasing (not earlier than previous timestamps).",
            "examples": [
                "2020-04-05T14:30:20Z"
            ],
            "x-optimade-unit": "inapplicable"
        },
        "description": {
            "$id": "https://schemas.optimade.org/defs/v1.2/properties/optimade/files/description",
            "x-optimade-requirements": {
                "support": "may",
                "sortable": false,
                "query-support": "none",
                "response-level": "may"
            },
            "title": "description",
            "x-optimade-type": "string",
            "x-optimade-definition": {
                "label": "description_optimade_files",
                "kind": "property",
                "version": "1.2.0",
                "format": "1.2",
                "name": "description"
            },
            "type": [
                "string",
                "null"
            ],
            "description": "Free-form description of a file.",
            "examples": [
                "POSCAR format file"
            ],
            "x-optimade-unit": "inapplicable"
        },
        "checksums": {
            "$id": "https://schemas.optimade.org/defs/v1.2/properties/optimade/files/checksums",
            "x-optimade-requirements": {
                "support": "may",
                "sortable": false,
                "query-support": "none",
                "response-level": "may"
            },
            "title": "checksums",
            "x-optimade-type": "dictionary",
            "x-optimade-definition": {
                "label": "checksums_optimade_files",
                "kind": "property",
                "version": "1.2.0",
                "format": "1.2",
                "name": "checksums"
            },
            "type": [
                "object",
                "null"
            ],
            "description": "Dictionary providing checksums of file contents.\n\n**Requirements/Conventions:**\n\n- The keys in the dictionary identify checksum functions and the values are strings containing the corresponding checksum.\n\n- Supported dictionary keys: `md5`, `sha1`, `sha224`, `sha256`, `sha384`, `sha512`.\n  Checksums outside this list MAY be used, but their names MUST be prefixed by database-provider-specific namespace prefix.",
            "examples": [
                {
                    "sha1": "8072f787eada2c50b60a27f3f098fbac7eea08cf"
                }
            ],
            "x-optimade-unit": "inapplicable",
            "properties": {
                "md5": {
                    "x-optimade-type": "string",
                    "x-optimade-unit": "inapplicable",
                    "type": [
                        "string"
                    ]
                },
                "sha1": {
                    "x-optimade-type": "string",
                    "x-optimade-unit": "inapplicable",
                    "type": [
                        "string"
                    ]
                },
                "sha224": {
                    "x-optimade-type": "string",
                    "x-optimade-unit": "inapplicable",
                    "type": [
                        "string"
                    ]
                },
                "sha384": {
                    "x-optimade-type": "string",
                    "x-optimade-unit": "inapplicable",
                    "type": [
                        "string"
                    ]
                },
                "sha512": {
                    "x-optimade-type": "string",
                    "x-optimade-unit": "inapplicable",
                    "type": [
                        "string"
                    ]
                }
            }
        },
        "atime": {
            "$id": "https://schemas.optimade.org/defs/v1.2/properties/optimade/files/atime",
            "x-optimade-requirements": {
                "support": "may",
                "sortable": false,
                "query-support": "none",
                "response-level": "may"
            },
            "title": "access time",
            "x-optimade-type": "timestamp",
            "x-optimade-definition": {
                "label": "atime_optimade_files",
                "kind": "property",
                "version": "1.2.0",
                "format": "1.2",
                "name": "atime"
            },
            "type": [
                "string",
                "null"
            ],
            "format": "date-time",
            "description": "Time of last access of a file as per POSIX standard.",
            "examples": [
                "2007-04-05T14:30:20Z"
            ],
            "x-optimade-unit": "inapplicable"
        },
        "ctime": {
            "$id": "https://schemas.optimade.org/defs/v1.2/properties/optimade/files/ctime",
            "x-optimade-requirements": {
                "support": "may",
                "sortable": false,
                "query-support": "none",
                "response-level": "may"
            },
            "title": "change time",
            "x-optimade-type": "timestamp",
            "x-optimade-definition": {
                "label": "ctime_optimade_files",
                "kind": "property",
                "version": "1.2.0",
                "format": "1.2",
                "name": "ctime"
            },
            "type": [
                "string",
                "null"
            ],
            "format": "date-time",
            "description": "Time of last status change of a file as per POSIX standard.",
            "examples": [
                "2007-04-05T14:30:20Z"
            ],
            "x-optimade-unit": "inapplicable"
        },
        "mtime": {
            "$id": "https://schemas.optimade.org/defs/v1.2/properties/optimade/files/mtime",
            "x-optimade-requirements": {
                "support": "may",
                "sortable": false,
                "query-support": "none",
                "response-level": "may"
            },
            "title": "modification time",
            "x-optimade-type": "timestamp",
            "x-optimade-definition": {
                "label": "mtime_optimade_files",
                "kind": "property",
                "version": "1.2.0",
                "format": "1.2",
                "name": "mtime"
            },
            "type": [
                "string",
                "null"
            ],
            "format": "date-time",
            "description": "Time of last modification of a file as per POSIX standard.\n\n**Requirements/Conventions:**\n\n- It should be noted that the values of `last_modified`, `modification_timestamp` and `mtime` do not necessary match.\n  `last_modified` pertains to the modification of the OPTIMADE metadata, `modification_timestamp` pertains to file contents and `mtime` pertains to the modification of the file (not necessary changing its contents).\n  For example, appending an empty string to a file would result in the change of `mtime` in some operating systems, but this would not be deemed as a modification of its contents.",
            "examples": [
                "2007-04-05T14:30:20Z"
            ],
            "x-optimade-unit": "inapplicable"
        }
    }
}
```
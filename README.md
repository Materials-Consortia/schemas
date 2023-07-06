<img width="180px" align="center" src="https://raw.githubusercontent.com/wiki/Materials-Consortia/OPTIMADE/images/logos/optimade-text-below-transparent-bg.png">


# OPTIMADE schemas

This repository hosts the permanent URLs to OPTIMADE schemas, currently the OpenAPI 3.0 format.

Find out more about OPTIMADE at our [homepage](https://optimade.org).

Minor versions of the schema can be acquired by modifying the version tag in the URL.
Version tags will always point to the latest release compatible with that version.

- [v1](./openapi/v1/optimade.json)
- [v1 Index Meta-database](./openapi/v1/optimade_index.json)

# EXPERIMENTAL

## OPTIMADE Property Definitions

We are readying the release of OPTIMADE v1.2, which is intended to introduce schemas that define properties (OPTIMADE property definitions).

In preparation for that upcoming release, we serve the preliminary versions of the definition files here.
However, note that until v1.2 is officially released, these are subject to change.

An index of the definition files is available at:

- [defs/index.md](defs/index.md)
- https://schemas.optimade.org/defs/index.html

Generated from the definitons are also:

- A JSON Schema for validation of OPTIMADE JSON:API responses:

  - [json-schema/v1.2.0/optimade.json](json-schema/v1.2.0/optimade.json)
  - https://schemas.optimade.org/json-schema/v1.2/optimade.json

- A JSON-LD context to be used with OPTIMADE v1.2 responses:

  - [json-ld/v1.2.0/optimade.json](json-ld/v1.2.0/optimade.json)
  - https://schemas.optimade.org/json-ld/v1.2/optimade.json

- An updated OpenAPI schema for v1.2 is not yet available.

An index of all definition files in the v1.2.0 release are available here:

- [releases/v1.2.0/index.md](releases/v1.2.0/index.md)
- https://schemas.optimade.org/releases/v1.2.0/index.html

(Until a new versions are released, this index will represent the exact same information as the definition index)

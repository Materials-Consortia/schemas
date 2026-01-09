<img width="180px" align="center" src="https://raw.githubusercontent.com/wiki/Materials-Consortia/OPTIMADE/images/logos/optimade-text-below-transparent-bg.png">


# OPTIMADE schemas

The OPTIMADE schemas website [https://schemas.optimade.org](https://schemas.optimade.org) and its [corresponding repository](https://github.com/Materials-Consortia/schemas) hosts permanent URLs to OPTIMADE schemas.

Find out more about OPTIMADE at our [homepage](https://optimade.org).

Minor versions of the schema can be acquired by modifying the version tag in the URL.
Version tags will always point to the latest release compatible with that version.

Full respone format schemas in json-schema format:

- v1.3: [json-schema/v1.3.0/optimade.json](json-schema/v1.3.0/optimade.json)
- v1.2: [json-schema/v1.2.0/optimade.json](json-schema/v1.2.0/optimade.json)

OpenAPI schemas of older versions:

- [v1.1.0](./openapi/v1.1.0/optimade.json)
- [v1.1.0 Index Meta-database](./openapi/v1/optimade_index.json)

# OPTIMADE Property Schemas (property definitions)

OPTIMADE publishes *OPTIMADE Property Definitions* for the standard properties part of the OPTIMADE API.

All definitions have stable URI IDs (`$id` in JSON) that represent the entity being defined.
The URIs are resolvable URLs that resolve to a human-readable description.
If `.json` is appended to the URL it resolves to a machine readable JSON version of the definition is provided with a format documented in the [OPTIMADE specification](https://www.optimade.org/optimade).
The content at these URLs may change with amendedments or clarifications, but a URI ID will always refer to what is functionally the same definition.
If an entity needs to be redefined it is given a new URI and the old URI is retained to represent the prior definition.

A good place to start to browse these definitions is the definition of the OPTIMADE standard v1.3:

- [defs/v1.3/standards/optimade](defs/v1.3/standards/optimade.md)

For the Physical Unit definitions, a good place to start is a collection of units suitable for use with OPTIMADE:

- [defs/v1.2/unitsystems/optimade/optimade](defs/v1.2/unitsystems/optimade/optimade.md)

A complete index of all provided definition files is available at:

- [defs/index](defs/index.md)

We also provide, generated from the definitons:

- JSON Schemas for validation of OPTIMADE JSON:API responses:

  - v1.3: [json-schema/v1.3.0/optimade.json](json-schema/v1.3.0/optimade.json)
  - v1.2: [json-schema/v1.2.0/optimade.json](json-schema/v1.2.0/optimade.json)

- JSON-LD contexts to be used with OPTIMADE responses (as a topmost `@context` field):

  - v1.3: [json-ld/v1.3.0/optimade.json](json-ld/v1.3.0/optimade.json)
  - v1.2: [json-ld/v1.2.0/optimade.json](json-ld/v1.2.0/optimade.json)

- OpenAPI schemas for v1.3 and v1.2 are not yet available.

The exact state of the definition files at the time of a patch release of OPTIMADE are placed at URLs with the format `https://schemas.optimade.org/releases/vMAJOR.MINOR.PATCH/vMAJOR.MINOR/...` and indexed at `https://schemas.optimade.org/releases/vMAJOR.MINOR.PATCH/vMAJOR.MINOR/index.html`.
The double URL segments for versions may look redundant, however, they take this form to keep a complete historical record that preserves amendments and clarifications that may have altered older definition files even after the entity has been redefined.

For the v1.3.0 patch release the complete index is available here:

- [releases/v1.3.0/index](releases/v1.3.0/index.md)

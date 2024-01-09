<img width="180px" align="center" src="https://raw.githubusercontent.com/wiki/Materials-Consortia/OPTIMADE/images/logos/optimade-text-below-transparent-bg.png">


# OPTIMADE schemas

The OPTIMADE schemas website [https://schemas.optimade.org](https://schemas.optimade.org) and its [corresponding repository](https://github.com/Materials-Consortia/schemas) hosts permanent URLs to OPTIMADE schemas.

Find out more about OPTIMADE at our [homepage](https://optimade.org).

For the present version of OPTIMADE, the schemas are in OpenAPI 3.0 format.

Minor versions of the schema can be acquired by modifying the version tag in the URL.
Version tags will always point to the latest release compatible with that version.

- [v1](./openapi/v1/optimade.json)
- [v1 Index Meta-database](./openapi/v1/optimade_index.json)

# EXPERIMENTAL

## OPTIMADE Property Definitions

We are readying the release of OPTIMADE v1.2, which is intended to introduce schemas that define properties, named OPTIMADE Property Definitions.

In preparation for the upcoming release, we serve the preliminary versions of the definition files here.
**Until v1.2 is officially released, these are not to be considered stable and may change without notice.**

All definitions have stable URI IDs (`$id` in JSON) that represent the entity being defined.
The URIs are resolvable URLs that resolve to a human-readable description.
If `.json` is appended to the URL it resolves to a machine readable JSON version of the definition is provided with a format documented in the [OPTIMADE specification](https://www.optimade.org/optimade).
The content at these URLs may change with amendedments or clarifications, but a URI ID will always refer to what is functionally the same definition.
If an entity needs to be redefined it is given a new URI and the old URI is retained to represent the prior definition.

A good place to start to browse these definitions is the definition of the OPTIMADE v1.2 standard:

- [defs/v1.2/standards/optimade](defs/v1.2/standards/optimade.md)

For the Physical Unit definitions, a good place to start is a collection of units suitable for use with OPTIMADE:

- [defs/v1.2/unitsystems/optimade/optimade](defs/v1.2/unitsystems/optimade/optimade.md)

A complete index of all provided definition files is available at:

- [defs/index](defs/index.md)

We also provide, generated from the definitons:

- A JSON Schema for validation of OPTIMADE JSON:API responses:

  - [json-schema/v1.2.0/optimade.json](json-schema/v1.2.0/optimade.json)

- A JSON-LD context to be used with OPTIMADE responses (as a topmost `@context` field):

  - [json-ld/v1.2.0/optimade.json](json-ld/v1.2.0/optimade.json)

- An updated OpenAPI schema for v1.2 is not yet available.

The exact state of the definition files at the time of a patch release of OPTIMADE are placed at URLs with the format `https://schemas.optimade.org/releases/vMAJOR.MINOR.PATCH/vMAJOR.MINOR/...` and indexed at `https://schemas.optimade.org/releases/vMAJOR.MINOR.PATCH/vMAJOR.MINOR/index.html`.
The double URL segments for versions may look redundant, however, they take this form to keep a complete historical record that preserves amendments and clarifications that may have altered older definition files even after the entity has been redefined.

For the v1.2.0 patch release the complete index is available here:

- [releases/v1.2.0/index](releases/v1.2.0/index.md)

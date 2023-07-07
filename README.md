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
The URIs are resolvable URLs that resolve to a human-readable description of the entity being defined.
By appending ".json" to the URL, a machine readable JSON version of the definition is provided with a format documented in the [OPTIMADE specification](https://www.optimade.org/optimade).
The content at these URLs may be amended or clarified, but the same URI ID always refer to what is functionally the same definition.
If a property needs to be redefined, the redefinition is given a new URI, and the old one is retained to represent the prior definition.

To browse the definitions, a good place to start is the definition of the OPTIMADE v1.2 standard:

- [https://schemas.optimade.org/defs/v1.2/standards/optimade](https://schemas.optimade.org/defs/v1.2/standards/optimade)
- [defs/v1.2/standards/optimade.md](defs/v1.2/standards/optimade.md)

For the Physical Unit definitions, a good place to start is a collection of units suitable for use with OPTIMADE:

- [https://schemas.optimade.org/defs/v1.2/unitsystems/optimade/optimade](https://schemas.optimade.org/defs/v1.2/unitsystems/optimade/optimade)
- [defs/v1.2/unitsystems/optimade/optimade](defs/v1.2/unitsystems/optimade/optimade)

A complete index of all provided definition files is available at:

- [https://schemas.optimade.org/defs/index.html](https://schemas.optimade.org/defs/index.html)
- [defs/index.md](defs/index.md)

We also provide, generated from the definitons:

- A JSON Schema for validation of OPTIMADE JSON:API responses:

  - [https://schemas.optimade.org/json-schema/latest/optimade.json](https://schemas.optimade.org/json-schema/latest/optimade.json)
  - [json-schema/v1.2.0/optimade.json](json-schema/v1.2.0/optimade.json)

- A JSON-LD context to be used with OPTIMADE responses (as a topmost `@context` field):

  - [https://schemas.optimade.org/json-ld/latest/optimade.json](https://schemas.optimade.org/json-ld/latest/optimade.json)
  - [json-ld/v1.2.0/optimade.json](json-ld/v1.2.0/optimade.json)

- An updated OpenAPI schema for v1.2 is not yet available.

The exact state of the definition files at the time of a patch release of OPTIMADE are placed at URLs with the format `https://schemas.optimade.org/releases/vMAJOR.MINOR.PATCH/vMAJOR.MINOR/...` and indexed at `https://schemas.optimade.org/releases/vMAJOR.MINOR.PATCH/vMAJOR.MINOR/index.html`.
The double URL segments for versions may look redundant, however, they take this form to keep a complete historical record that preserves amendments and clarifications that may have altered older definition files even after the entity has been redefined.
Hence, for the v1.2.0 the Index URLs are:

- [https://schemas.optimade.org/releases/v1.2.0/v1.2/index.html](https://schemas.optimade.org/releases/v1.2.0/v1.2/index.html)
- [releases/v1.2.0/v1.2/index.md](releases/v1.2.0/v1.2/index.md)


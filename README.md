# 6G Data Ontology

An open, modular OWL ontology framework for structuring, classifying and semantically linking heterogeneous data and concepts across future 6G networks, computing environments, applications and vertical domains.

## Architecture

Version 0.2 introduces a shared semantic core and seven use-case modules:

- `6G-core.OWL` — common classes and properties for data, network, compute, applications, QoS, AI, governance and sustainability.
- `6G-onto-sustainable.OWL`
- `6G-onto-smart-cities.OWL`
- `6G-onto-industrial-IoT.OWL`
- `6G-onto-digital-twin.OWL`
- `6G-onto-industrial-robotics.OWL`
- `6G-onto-healthcare-robotics.OWL`
- `6G-onto-holographic-communications.OWL`

`6G-all.OWL` is the convenience entry point that imports the complete framework and the example ABox.

The former misspelled `6G-onto-holographic-coummunications.OWL` is retained as a deprecated compatibility wrapper.

## Knowledge-graph example and validation

`6G-example-instances.OWL` provides a small ABox illustrating instance-level population. `example-queries.sparql` provides competency-question examples for querying the ontology.

The ontology modules are primarily schema/TBox resources; the example file demonstrates how they can be populated as a knowledge graph.

## Opening and editing

Protégé is recommended for interactive editing and reasoning. Other suitable tools include WebProtégé, Apache Jena, RDF4J, GraphDB, Stardog, RDFox and TopBraid.

Open `6G-all.OWL` to work with the complete modular ontology. Because OWL imports use persistent ontology IRIs, local import mappings may be required when working offline.

## Design principles

The project follows a modular core-plus-extension model. Shared concepts belong in the core; use-case-specific concepts remain in their modules and align to the core through OWL subclass/property semantics. Existing domain vocabulary is preserved where practical while malformed experimental identifiers and unintended multi-domain/multi-range property semantics are corrected.

Future work includes alignment with reusable vocabularies such as SOSA/SSN, richer logical axioms, expanded competency questions, instance datasets, SHACL validation, reasoning tests, provenance, versioned releases and mappings to relevant telecom/industry information models.

## Collaboration and community contribution

This repository is an open collaborative initiative. We welcome researchers, industry experts, telecom operators, standards communities, ontology engineers, Semantic Web researchers and AI specialists.

Contributions may include new use cases, ontology extensions, mappings, competency questions, validation datasets, reasoning examples, documentation, visualizations and standardization-oriented work. Contributions through issues and pull requests are welcome, and motivated contributors may also request to participate as long-term project collaborators.

## Status

This repository is a research seed and community-extensible ontology framework. It is **not** presented as a finalized or standardized 6G ontology.

## License

See `LICENSE`.

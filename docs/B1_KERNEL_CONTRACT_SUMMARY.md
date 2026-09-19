# B1 Kernel Contract Summary — IIPR

B1 is the typed constitutional kernel foundation for Institutional Intelligence-Production Runtime.

## Core contract

B1 defines strict, frozen canonical records and a deterministic identity model.

Key properties include:

- typed identifiers and enums;
- aware timestamps;
- immutable/frozen records;
- strict validation;
- canonical JSON serialization;
- SHA-256 content digests;
- checkpoint and authority record structures;
- explicit error taxonomy;
- deterministic build/evidence workflow.

## Canonical identity

The private contract defines `canonical_json_bytes` as the hashing serializer.

It preserves declared fields and deterministic ordering while rejecting unsupported or unsafe values such as cycles, non-finite floats, lone surrogates, and unsupported object types.

## Authority boundary

B1 validates structure. It does not decide that evidence is true or that a transition is authorized.

Doctor/tests are evidence, not authority.

Independent review and human ratification remain separate state transitions.

## Deliberate non-goals

B1 does not implement research, retrieval, EDI workflows, EVS generation, publication, monitoring, persistence, provider integration, or a transition/commit engine.

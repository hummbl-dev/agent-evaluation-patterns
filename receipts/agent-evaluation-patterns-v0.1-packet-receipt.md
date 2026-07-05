# Receipt: agent-evaluation-patterns v0.1 packet

This receipt records what was produced for v0.1 of Agent Evaluation Patterns and why.

## Produced artifacts

- `docs/v0.1-boundary.md` — scope, non-goals, adoption boundary, review expectations, non-canon posture, required packet pieces, adjacent repo links.
- `docs/prior-art.md` — public prior art, adjacent ecosystem, vocabulary, and key concepts.
- `schemas/agent-evaluation-patterns-v0.1.json` — JSON schema for a v0.1 evaluation packet.
- `examples/evaluation-packet-v0.1.example.json` — a valid example packet.
- `fixtures/valid/evaluation-packet-v0.1.valid.json` — a valid fixture.
- `fixtures/invalid/evaluation-packet-v0.1.invalid.json` — an invalid fixture missing the required `statisticalRequirements` field.

## Issues addressed

- Issue #1: Define v0.1 scope and boundary — `docs/v0.1-boundary.md`.
- Issue #2: Collect prior art and adjacent ecosystem references — `docs/prior-art.md`.
- Issue #3: Design minimal schema/examples layout — schema, example, and fixtures.

## Provenance

- Author: hummbl-dev
- Source: public seed repository
- Posture: candidate, non-canon
- No private, internal, or secret operational content included.

## Review expectations

- Schemas are valid JSON Schema (draft 2020-12).
- The valid fixture conforms to the schema.
- The invalid fixture intentionally fails the schema by omitting `evaluationContract.statisticalRequirements`.

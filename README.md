# consensus-persona-generator

Generate reusable decision personas for Consensus guard workflows.

`consensus-persona-generator` creates and persists `persona_set` artifacts used by guard skills for weighted, multi-perspective evaluations.

## Why it exists

Good guard decisions need diverse viewpoints (security, reliability, operations, user impact). This tool makes those viewpoints explicit, reusable, and auditable.

## Core capabilities

- strict schema validation
- deterministic persona generation path (default for reproducibility)
- board-native `persona_set` artifact persistence
- indexed lookups for latest and by-id access

## Quick start

```bash
npm i
node --import tsx run.js --input ./examples/persona-input.json
```

## Typical output

- `persona_set_id`
- `personas[]` with weighted reputations
- board write reference for traceability

## Test

```bash
npm test
```

## Continuous improvement

See `AI-SELF-IMPROVEMENT.md` for iteration and persona quality tuning.

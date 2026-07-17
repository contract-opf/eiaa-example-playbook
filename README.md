# Example: Educational Affiliation Agreement — Negotiation Playbook (OPF 0.3)

A real, corpus-derived negotiation playbook, published as a pedagogical
example of the **Open Playbook Format (OPF)**. It was compiled by
[playbook-engine] from 44 real educational-affiliation agreements
(161 negotiation versions) between Exos and university counterparties.

**Privacy:** the source corpus is private and is NOT included. Every
counterparty identity has been pseudonymized (`Counterparty-N`) or redacted
— names, people, street addresses, e-mail addresses, e-signature audit
trails, and source filenames — via the engine's `publish` transform, whose
hard backstop fails the build if any known entity name survives. Dates are
coarsened to quarters. Exos, the publishing party, is named deliberately.

## Files

| File | What it is |
|---|---|
| [`index.html`](https://contract-opf.github.io/eiaa-example-playbook/) | **Start here** — the single-file playbook: human-readable document + machine-readable payloads |
| `playbook.opf.json` | The canonical OPF 0.3 document (evidence, digest, corpus audit trail, content hash) |
| `playbook.digest.json` | The compact model-facing digest (~38K tokens): per-clause stances, preferred variations, deduplicated exemplar forms |

The HTML bundle embeds the canonical JSON verbatim in a
`<script id="opf-canonical" type="application/json">` block — extract it,
parse it, and verify `identity.content_hash` over the canonical
serialization. `identity.supersedes` names the private (internal) artifact
this public profile was derived from.

## What to look at

- **Per-clause positions**: historical stance (descriptive, evidence-derived),
  preferred variations with citations, concessions, rejected asks, and
  frequency-banded exemplar forms.
- **Posture / Floor**: intentionally pending — those sections are authored
  by counsel, never fabricated from data. The document explains how they
  are enabled.
- **Method & provenance panel**: corpus coverage, judging economics, and
  traceability — every position cites real observations.

Published 2026-07-17 as part of a talk on evidence-derived negotiation
playbooks. Format spec: see the OPF specification in the playbook-engine
repository.

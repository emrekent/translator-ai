# Language Pair Quality Matrix

Track what is actually supported, what is still draft-level, and what needs outside review before stronger claims are made.

## Status definitions

| Status | Meaning |
| --- | --- |
| Primary | Reviewed examples and core workflow are maintained in this repository. |
| Structured secondary | Rules and examples exist, but a documented native-speaker QA log is still missing. |
| Experimental reference | Notes and examples exist for exploration only. Do not market as validated support. |

## Current matrix

| Language pair | Status | Evidence in repo | Publishing guidance |
| --- | --- | --- | --- |
| English to Turkish | Primary | `references/examples.md`, `references/quality-checklist.md`, `TESTING.md` | Strongest path in this repo; still use human review for legal, medical, or high-stakes work |
| English to Spanish | Structured secondary | `references/translation-rules.md`, `references/examples.md`, `references/special-cases.md` | Good for drafts; use human review before publishing |
| English to French | Structured secondary | `references/translation-rules.md`, `references/examples.md`, `references/special-cases.md` | Good for drafts; use human review before publishing |
| English to German | Structured secondary | `references/translation-rules.md`, `references/examples.md`, `references/special-cases.md` | Good for drafts; use human review before publishing |
| English to Portuguese | Experimental reference | `references/examples.md`, `references/grammar-comparison.md`, `references/false-friends.md` | Use as exploratory support only |
| English to Italian | Experimental reference | `references/examples.md`, `references/grammar-comparison.md`, `references/false-friends.md` | Use as exploratory support only |
| English to Russian | Experimental reference | `references/examples.md`, `references/grammar-comparison.md`, `references/false-friends.md` | Use as exploratory support only |

## What needs to happen before a status upgrade

### Upgrade to Primary

- maintain reviewed examples across core text types
- document revision history in `TESTING.md`
- add native-speaker review notes for recurring edge cases
- keep the quality checklist aligned with real failures

### Upgrade from Structured Secondary to Primary

- add a documented QA pass from native speakers
- verify region and formality defaults
- collect at least one strong example each for marketing, technical, casual, and UI text
- record common mistakes specific to that pair

### Upgrade from Experimental Reference to Structured Secondary

- add pair-specific rules or decision notes
- add at least two worked examples with reasoning
- define regional assumptions
- list the top failure modes to watch for

## Maintenance rule

When evidence and marketing copy disagree, downgrade the marketing copy. Trust converts better than inflated coverage.

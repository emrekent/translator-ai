# Testing and Validation Status

**Last updated:** March 7, 2026
**Skill version:** 2.1

This repository now separates reviewed coverage from draft reference material. Earlier documentation overstated how much of the non-Turkish coverage was validated. That has been corrected.

## Current validation scope

### English to Turkish

Reviewed examples exist for:

- marketing copy
- technical documentation
- casual/personal writing
- humor and irony

These examples are documented in `references/examples.md` and checked against the reusable checklist in `references/quality-checklist.md`.

### English to Spanish/French/German

Starter rules and examples exist, but this repository does not yet contain a documented native-speaker QA log for those pairs. Treat them as structured secondary coverage, not as fully validated production support.

### English to Portuguese/Italian/Russian

Reference material exists for exploration and terminology direction, but these pairs should not be presented as fully validated.

## Fixes made in this pass

- Removed unsupported "98%+" and blanket "production-ready" claims from public-facing docs.
- Replaced local-only installation paths with portable GitHub install commands.
- Tightened the skill metadata around real user trigger phrases.
- Corrected the Turkish casual example so the informal voice stays consistent.
- Corrected the Turkish humor example so the line reads naturally instead of relying on broken syntax.

## Recommended review flow

1. Pick a sample paragraph from the target domain.
2. Run a standard translation.
3. Run a review pass on the output.
4. Check meaning, tone, formatting, terminology, and naturalness with `references/quality-checklist.md`.
5. For non-primary language pairs, add human review before publication.

## Remaining gaps

- No automated regression harness exists for prompt quality.
- No native-speaker review log is stored yet for Spanish, French, German, Portuguese, Italian, or Russian.
- No public benchmark data exists for download-to-activation conversion on skills.sh.

The practical goal of this cleanup is trust: a tighter, more honest skill page should convert better than a broader page with weak proof.

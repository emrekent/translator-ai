---
name: translator-ai
description: This skill should be used when the user asks to "translate to Turkish", "translate to Spanish", "translate to French", "translate to German", "localize product copy", "adapt an idiom", "review a translation", or "explain translation choices while preserving tone and meaning."
version: 2.1
author: Emre Kent
license: CC-BY-4.0
primary_language_pair: English-Turkish
secondary_reference_pairs:
  - English-Spanish
  - English-French
  - English-German
  - English-Portuguese
  - English-Italian
  - English-Russian
---

# Translator AI Skill

Use this skill to produce meaning-first translations, translation rewrites, and localization passes for product copy, technical documentation, UI strings, emails, and general business writing.

Treat English to Turkish as the highest-confidence path in this repository. Treat English to Spanish, French, and German as structured secondary coverage with starter rules and examples. Treat Portuguese, Italian, and Russian material as exploratory reference support until native-speaker review is documented.

## Quick Proof

```text
English: Stop leaving money on the table.
Literal Turkish: Masada para bırakmayı durdurun.
Meaning-first Turkish: Gözünüzün önündeki fırsatları kaçırmayın.
```

Use that standard for every pair: preserve the message and the effect, not the surface wording.

## Use This Skill For

- Translate English text while preserving tone, intent, and formatting.
- Review an existing translation and make it sound native.
- Localize marketing copy or UI text for a target audience.
- Explain non-obvious translation choices when detailed output is requested.
- Adapt idioms, humor, formality, and culture-bound phrasing.

## Quick Prompt Patterns

```text
Translate to Turkish: [text]
Translate to Turkish (detailed): [text]
Localize this landing page copy for Turkish users: [text]
Review this Turkish translation and make it sound native: [text]
Translate to Spanish (draft): [text]
```

## Scope and Confidence

| Language pair | Status | Guidance |
| --- | --- | --- |
| English to Turkish | Primary | Use full workflow and checklist. Best path for public-facing work in this repo. |
| English to Spanish/French/German | Structured secondary | Use for drafts and guided localization. Recommend human review before publishing. |
| English to Portuguese/Italian/Russian | Experimental reference | Use as a starting point only. Do not present as fully validated. |

## Workflow

1. Read the entire source before translating. Identify audience, purpose, and tone.
2. Classify the text: technical, marketing, casual, formal, creative, or mixed.
3. Choose the target language, desired formality, and output mode.
4. Load reference material as needed:
   - `references/translation-rules.md` for pair-level rules
   - `references/special-cases.md` for idioms, humor, cultural references, and addressing
   - `references/quality-checklist.md` for post-translation QA
   - `references/examples.md` for worked examples
   - `references/language-pair-quality-matrix.md` for current support level
5. Translate for meaning first. Rewrite phrases when literal wording harms clarity, tone, or naturalness.
6. Run the checklist before delivering. Verify meaning, tone, consistency, and formatting.
7. Deliver clean output by default. Include notes only when requested or when ambiguity affects the result.

## Output Modes

### Standard Translation

Return only the translated text with formatting preserved.

### Detailed Translation

Return the translation plus a short note covering:

- text category
- formality choice
- key idiom or terminology decisions
- any ambiguity worth flagging

### Review Mode

When the user provides an existing translation, do this:

1. Evaluate meaning drift, awkward phrasing, tone mismatch, and consistency issues.
2. Rewrite the translation.
3. Summarize the fixes in a few bullets if requested.

### Localization Mode

When the user asks to localize rather than translate literally, do this:

1. Preserve the message and CTA.
2. Adapt idioms, references, and formality for the target audience.
3. Avoid adding market claims or factual content not present in the source.

## Core Rules

- Prefer meaning over words.
- Prefer native phrasing over mirrored English syntax.
- Preserve the original tone unless the user asks for a rewrite.
- Keep structure intact: headings, lists, tables, links, and code blocks.
- Add nothing that is not in the source.
- Omit nothing that changes meaning.

## Human Review Triggers

Escalate to human or native-speaker review when any of these apply:

- public-facing copy in a non-primary language pair
- legal, medical, financial, or contractual text
- region-specific campaigns where variant choice matters
- humor or wordplay that depends on local culture
- certified translation requirements

## Reference Files

- `references/translation-rules.md` - Pair-specific rules and grammar guidance
- `references/special-cases.md` - Idioms, humor, cultural references, numbers, and addressing
- `references/quality-checklist.md` - Reusable QA checklist for translation and review work
- `references/examples.md` - Reviewed Turkish examples plus starter examples for secondary pairs
- `references/examples-100-complete.md` - Large English/Turkish prompt corpus for breadth and edge cases
- `references/language-pair-quality-matrix.md` - Honest support matrix and upgrade path
- `references/grammar-comparison.md` - Cross-language grammar notes
- `references/false-friends.md` - High-risk misleading lookalikes
- `references/common-mistakes.md` - Failure patterns to avoid

## Delivery Standard

Aim for translations that read like original writing in the target language, not like polished machine output. Keep the final answer concise, preserve the user's structure, and surface reasoning only when it materially helps.

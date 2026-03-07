# translator-ai

Meaning-first translation skill for English to Turkish, plus secondary and experimental guidance for Spanish, French, German, Portuguese, Italian, and Russian.

Live listing: https://skills.sh/emrekent/translator-ai/translator-ai

## Install

From GitHub:

```bash
npx skills add https://github.com/emrekent/translator-ai --skill translator-ai
```

From a local checkout:

```bash
npx skills add . --skill translator-ai
```

## What makes this worth installing

- Handles translation, localization, and translation review instead of only literal conversion.
- Optimized for product copy, technical docs, UI strings, emails, and business writing.
- Strongest support is English to Turkish, with reusable QA patterns for additional language pairs.
- Includes prompt-ready examples, a review checklist, and reference material for idioms and tone.

## Quick proof

English:

```text
Stop leaving money on the table.
```

Literal Turkish:

```text
Masada para bırakmayı durdurun.
```

Meaning-first Turkish:

```text
Gözünüzün önündeki fırsatları kaçırmayın.
```

The skill is built around producing the second kind of result.

## Best prompts to try

```text
Translate to Turkish: [text]
Translate to Turkish (detailed): [text]
Localize this landing page copy for Turkish users: [text]
Review this Turkish translation and make it sound native: [text]
Translate to French (draft): [text]
```

## Support matrix

| Language pair | Status | Best use |
| --- | --- | --- |
| English to Turkish | Primary | Public-facing copy, docs, UI strings, translation review |
| English to Spanish/French/German | Structured secondary | Draft localization and guided rewrites; use human review before publishing |
| English to Portuguese/Italian/Russian | Experimental reference | Idea generation and terminology direction only |

## Repository contents

- `SKILL.md` - Trigger phrases, workflow, scope, and delivery standard
- `references/translation-rules.md` - Pair-specific rules
- `references/special-cases.md` - Idioms, humor, cultural references, addressing
- `references/quality-checklist.md` - Translation QA checklist
- `references/examples.md` - Reviewed Turkish examples and secondary-pair starter examples
- `references/examples-100-complete.md` - Large English/Turkish prompt corpus
- `references/language-pair-quality-matrix.md` - Honest support levels and upgrade path
- `INSTALLATION.md` - Installation and activation guide
- `TESTING.md` - Validation scope and current testing limits

## Quality position

This repository now distinguishes between:

- reviewed primary coverage
- structured secondary guidance
- experimental reference material

That tradeoff is intentional. Clear boundaries improve trust, make the skill easier to discover for the right use cases, and keep the public listing credible.

## Contributing

To improve a language pair, contribute one or more of the following:

- native-speaker review notes
- before/after examples with reasoning
- checklist additions for a recurring failure mode
- prompt examples for a new domain such as ecommerce, legal ops, or developer docs

Open an issue with the source text, target audience, target language, and the problem you saw.

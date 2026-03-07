# translator-ai Installation and Usage

## Install

Install from GitHub:

```bash
npx skills add https://github.com/emrekent/translator-ai --skill translator-ai
```

Install from a local checkout:

```bash
npx skills add . --skill translator-ai
```

Verify that the skill is available:

```bash
npx skills list
```

## How to trigger it

Use direct phrasing. These prompts are intentionally close to the skill metadata:

```text
Translate to Turkish: [text]
Translate to Spanish: [text]
Translate to French: [text]
Translate to German: [text]
Localize this product copy for Turkish users: [text]
Review this translation and fix the tone: [text]
Explain why this Turkish phrasing is better: [text]
```

## Recommended usage patterns

### Standard translation

```text
Translate to Turkish: Stop leaving money on the table.
```

### Detailed mode

```text
Translate to Turkish (detailed): Look, I get it. You've tried everything.
```

### Translation review

```text
Review this Turkish translation and make it sound native: [text]
```

### Localization pass

```text
Localize this landing page copy for Turkish startup founders: [text]
```

## Support levels

| Language pair | Status | Guidance |
| --- | --- | --- |
| English to Turkish | Primary | Best-supported path in this repository |
| English to Spanish/French/German | Structured secondary | Good for drafts and guided rewrites; use human review before publishing |
| English to Portuguese/Italian/Russian | Experimental reference | Use as a starting point only |

## Files to consult

- `SKILL.md` for trigger phrases and workflow
- `references/translation-rules.md` for pair-specific rules
- `references/special-cases.md` for idioms, humor, and cultural adaptation
- `references/quality-checklist.md` for QA
- `references/examples.md` for worked examples
- `references/language-pair-quality-matrix.md` for support boundaries

## Troubleshooting

### Skill does not activate

1. Confirm installation with `npx skills list`.
2. Use one of the direct trigger phrases shown above.
3. Ask explicitly for translation, localization, or translation review instead of a vague rewrite request.

### Output feels too literal

Ask for a localization or review pass:

```text
Review this translation and make it sound native.
```

or:

```text
Localize this copy for Turkish users without changing the meaning.
```

### Working in a non-primary language pair

Treat Spanish, French, and German as guided draft support. Treat Portuguese, Italian, and Russian as exploratory support. For public-facing copy, request human review before publishing.

## Quality expectations

This skill is strongest when asked to preserve:

- meaning
- tone
- formatting
- terminology consistency

It is not a substitute for certified legal, medical, or compliance translation.

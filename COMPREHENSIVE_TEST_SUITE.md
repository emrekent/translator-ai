# Translation Review Corpus

**Last updated:** March 7, 2026
**Purpose:** Maintain a reusable manual review set for translator-ai updates.

This file is a regression corpus, not proof that every listed language pair is production-ready. Use it to spot drift when updating prompts, examples, or rules.

## How to use this corpus

1. Translate the source text with the skill.
2. Review the output with `references/quality-checklist.md`.
3. Record whether the output preserves meaning, tone, and formatting.
4. For non-primary language pairs, route the result through native-speaker review before treating it as validated.

## Primary regression set: English to Turkish

### 1. Marketing copy

**Source**

```text
Stop leaving money on the table. Our AI-powered tool finds hidden revenue opportunities your competitors are missing.
```

**What to check**

- idiom is adapted, not translated literally
- CTA stays persuasive
- "AI-powered" wording sounds natural in Turkish

### 2. Technical documentation

**Source**

```text
To configure the webhook, navigate to Settings > Integrations > Webhooks. Click "Add New Webhook" and paste your endpoint URL.
```

**What to check**

- menu structure stays intact
- technical terms stay consistent
- instructions remain clear and formal

### 3. Casual writing

**Source**

```text
Look, I get it. You've tried everything. The diets, the apps, the 5 AM workouts that lasted exactly three days.
```

**What to check**

- register stays informal and conversational
- rhythm feels natural in Turkish
- humor does not become stiff or corporate

### 4. Humor and irony

**Source**

```text
"Just one more episode" I said, 4 hours ago, as I started my 47th rewatch of The Office.
```

**What to check**

- irony stays obvious
- sentence remains grammatical
- the joke lands without explanation

### 5. UI strings

**Source**

```text
Save changes
Try again
Invite team members
```

**What to check**

- wording is concise
- button-label style is preserved
- terminology is consistent across the set

## Secondary review set

Use these to inspect the draft quality of non-primary pairs. Do not interpret a good draft as proof of full validation.

| Pair | Source text | Main risk |
| --- | --- | --- |
| English to Spanish | We help small teams move faster without sacrificing control. | register and regional neutrality |
| English to French | Pricing updates take effect on April 1. Cancel anytime before renewal. | tone and formatting |
| English to German | The system retries failed jobs automatically after 30 seconds. | noun capitalization and word order |
| English to Portuguese | Your dashboard is ready. Invite the rest of the team to collaborate. | variant choice and product tone |
| English to Italian | We built this workflow to remove repetitive admin work. | idiomatic business phrasing |
| English to Russian | Export the report, review the totals, and confirm the tax settings. | case handling and terminology |

## Acceptance rules

Consider a result strong only when all of these pass:

- meaning preserved
- tone preserved
- format preserved
- terminology consistent
- output reads like native writing

If any one of those fails, revise the skill copy or references before making stronger public claims.

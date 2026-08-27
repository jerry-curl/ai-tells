# AI Tells

**AI Tells** is a small, model-neutral writing skill for finding and removing phrases and constructions that make prose sound machine-made.

The focus is not on banning individual words. It is on recognizing the *shape* of writing that announces its own importance, narrates its own emphasis, or falls into repetitive assistant-style templates.

The central rule:

> **Ban the construction, not the instances.**

A phrase list can remove today's wording and still leave the grammar that produces tomorrow's variation.

## What AI Tells does

AI Tells supports three modes:

- **WRITE** — silently avoid common AI tells while creating new prose.
- **AUDIT** — detect and report meaningful tells without changing the text.
- **REWRITE** — revise the text only when explicitly asked.

The skill is designed to work with ChatGPT, Claude, local models, other assistants, or a human editing workflow.

## What it does differently

Most AI-writing cleanup lists focus on obvious vocabulary such as *delve*, *tapestry*, *leverage*, or *in conclusion*.

AI Tells also focuses on **meta-commentary**: language that tells the reader a point matters instead of making the point matter.

Examples:

- "It's worth noting that..."
- "The key takeaway is..."
- "To be clear..."
- "And that's the point."
- "What this means is..."

It also watches for constructions that simple search-and-replace cannot reliably catch:

- self-narrating asides,
- forced rule-of-three cadence,
- repetitive sentence templates,
- puffed-up transitions,
- automatic sycophancy,
- chatbot artifacts left in finished prose.

## The `worth` rule

One of the most useful distinctions in the skill:

`worth` + gerund is often a tell when it **grades information for the reader**.

> "Two things are worth you knowing."

But it is ordinary English when it **judges whether an action is worth the effort**.

> "That domain is worth chasing."

Those are not the same construction. The skill is meant to use judgment, not blind replacement.

## Quick start

Copy `SKILL.md` into the instruction or skill system you use.

Then invoke it in one of three ways.

### WRITE

> Use AI Tells in WRITE mode. Draft a short product update for customers.

The skill should avoid the tells silently and return only the requested writing.

### AUDIT

> Use AI Tells in AUDIT mode on this draft. Do not rewrite it.

The skill should report meaningful hits and suggested fixes.

### REWRITE

> Use AI Tells in REWRITE mode. Clean this draft without flattening my voice.

The skill should return the revised text while preserving meaning and voice.

## What the skill does not do

AI Tells is not an "AI detector" and does not promise that text will be "undetectable."

It also should not:

- add fake typos or slang,
- manufacture personal stories,
- flatten personality,
- replace precise technical terms just because they appear on a word list,
- alter quotations, code, commands, citations, legal text, filenames, or other exact-content material without permission.

The goal is better writing, not detector gaming.

## Repository contents

```text
ai-tells/
├── README.md
├── LICENSE
├── SKILL.md
├── TESTS.md
├── CHANGELOG.md
└── examples/
    ├── audit-example.md
    └── before-after.md
```

## Testing

`TESTS.md` contains acceptance and regression tests for the public skill.

The tests cover:

- silent prevention in WRITE mode,
- non-destructive AUDIT behavior,
- meaning preservation,
- contextual uses of `worth`,
- technical-language exceptions,
- protected exact-content material,
- rule-of-three judgment,
- replacement regressions,
- voice preservation,
- model neutrality.

## Contributions

If you find a new tell, the most useful contribution is not just the phrase. Describe the **construction** that generates the phrase and include:

1. an example,
2. why it reads as machine-made,
3. a counterexample that should *not* be flagged,
4. a regression test.

That helps the skill improve without turning into a giant blacklist.

## License

MIT. See `LICENSE`.

## Origin and acknowledgments

**AI Tells was created and developed by Jerry Curl.**

The project started with established public work on common AI-writing patterns, including institutional and community-maintained resources such as Wikipedia's *Signs of AI writing* / WikiProject AI Cleanup and other published vocabulary lists. Those resources provided a useful baseline.

AI Tells then extends that baseline with additional observed patterns, especially assistant meta-commentary, construction-level detection, contextual judgment, protected-content rules, WRITE/AUDIT/REWRITE behavior, and regression-oriented testing.

The public sources are acknowledged as inputs and reference material. They are not presented as the authors or owners of AI Tells.

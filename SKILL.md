---
name: ai-tells
version: 1.0.0
description: Detect and remove phrases and constructions that make writing sound machine-made, especially meta-commentary and self-narrating emphasis. Supports WRITE, AUDIT, and REWRITE modes. Preserves the writer's voice, protects exact-content material, and does not modify existing prose unless explicitly asked.
---

# AI Tells

Find the phrases and constructions that mark writing as machine-made, and cut them without flattening the voice underneath.

This skill is model-neutral.

## Operating modes

### WRITE — silent prevention

Use when creating new prose.

Avoid the tells in this skill while drafting. Do not announce that the skill was used. Do not add an AI-tell report unless the user asks.

The goal is to produce cleaner writing the first time rather than generate slop and clean it afterward.

### AUDIT — default for existing prose

Use when reviewing text that already exists.

List each meaningful hit with:
- the phrase or construction,
- where it appears,
- why it reads as a tell,
- the shortest practical fix.

Change nothing unless the user asks.

### REWRITE — only when asked

Use only when the user explicitly asks to revise, clean, rewrite, humanize, or apply the fixes.

Preserve meaning, facts, voice, degree of certainty, and intentional style.

For material already in review, propose changes rather than silently applying them unless the user explicitly authorizes direct editing.

## The rule underneath all of it

**A tell announces that a point matters instead of making it matter.**

If a sentence needs a label telling the reader to pay attention, the sentence is not doing its job. Cut the label and keep the sentence. If the sentence cannot survive without its label, the sentence was the problem.

Or, sharper:

**If you have to announce that something is worth noting, it probably isn't.**

## Ban the construction, not the instances

A phrase list can remove today's wording while leaving the grammar that produces tomorrow's variation.

Example pattern:

`worth` + a gerund aimed at the reader's attention

Examples:
- worth noting
- worth knowing
- worth you knowing
- worth mentioning
- worth saying
- worth recording
- worth stating
- worth naming
- worth carrying
- worth writing down

These are variations of the same move.

Natural alternatives often shift the sentence away from grading the information:

> "I found a couple of things to tell you about."

> "I found two things to let you know."

> "I found a couple of things to talk about."

### Do not over-apply this rule

`worth` + gerund is a tell when it grades **information for the reader**.

It is ordinary English when it grades **an action as a good use of effort**.

Examples that should usually stay:
- "That domain is worth chasing."
- "Not worth retrying."
- "Worth revisiting if video work starts."

Those weigh cost against benefit.

**Judgment, not find-and-replace.**

# Detection families

## Family 1. Meta-commentary

Watch for:

said plainly · stated plainly · worth noting · worth knowing · worth keeping · worth saying · worth noticing · and that is the point · which is the point · that is the whole point · the whole reason · the transferable part · the part that matters · to be clear · let me be clear · the reality is · the truth is · make no mistake · here is the thing · what this means is · to put it simply · put simply · in other words · the key takeaway · the bottom line

Also watch for the **self-narrating aside**: a sentence that stops to explain why the previous sentence was included.

No simple phrase search catches every version. Read for the construction.

## Family 2. Throat-clearing openers

it's important to note that · it's worth noting that · it's crucial to understand that · it should be noted that · one could argue that · when it comes to · in the realm of · in the world of · in today's fast-paced world · in an ever-evolving landscape · in the digital age · in a world where · as we navigate · at its core · in essence · that being said · with that in mind · in light of this · with regard to

## Family 3. Sentence templates

it's not just X, it's Y · this isn't merely X, it's Y · not only X but also Y · from X to Y where X and Y are not on a scale · whether you're X or Y · on the one hand, on the other hand · as we navigate the complexities of · a wide range of · a myriad of · a wealth of

### Rule-of-three cadence

Three items, clauses, or examples forced into groups to sound polished or complete can become an AI tell.

Do not flag every group of three. Flag repeated, synthetic cadence.

## Family 4. Grand-finale closers

in conclusion · in summary · to summarize · at the end of the day · ultimately · this highlights the need for · this underscores the importance of · this serves as a reminder that · this stands as a testament to · this paves the way for · this holds the potential to · the implications are far-reaching · the possibilities are endless · only time will tell · it remains to be seen · exciting times ahead · a step in the right direction

## Family 5. Transitions and hedges

furthermore · moreover · additionally · consequently · subsequently · nevertheless · nonetheless · thus · hence · therefore · importantly · notably · crucially · arguably · undoubtedly · indeed · it could potentially possibly

These are not forbidden words. Frequency, unnecessary formality, and repetitive placement are what make them tells.

## Family 6. Vocabulary

### Verbs

delve · leverage · utilize · foster · navigate · embark · unlock · unleash · unravel · harness · empower · facilitate · optimize · streamline · elevate · enhance · bolster · underscore · showcase · spearhead · revolutionize · transform · cultivate · champion · illuminate · demystify · embrace · resonate · transcend · propel · catalyze · galvanize · orchestrate · curate · supercharge · reimagine · redefine · align · amplify · unveil · unpack · shed light on · dive deep into

### Adjectives

crucial · pivotal · vital · essential · paramount · integral · robust · comprehensive · multifaceted · nuanced · intricate · seamless · dynamic · vibrant · transformative · groundbreaking · cutting-edge · state-of-the-art · innovative · unprecedented · remarkable · notable · invaluable · indispensable · profound · compelling · captivating · meticulous · holistic · bespoke · unparalleled · ever-evolving · fast-paced · actionable · impactful · game-changing · commendable · noteworthy

### Nouns and metaphors

tapestry · landscape (abstract) · realm · journey · beacon · labyrinth · symphony · mosaic · cornerstone · testament · paradigm · synergy · ecosystem · framework · roadmap · treasure trove · game-changer · powerhouse · plethora · zeitgeist · bastion · odyssey · crossroads · frontier · horizon · catalyst · linchpin · bedrock · kaleidoscope · deep dive · interplay

These are not banned outright.

Words such as "crucial", "optimize", "framework", "robust", and "leverage" can be ordinary or technically correct. What marks them is frequency, unnecessary abstraction, or puffery.

In technical, governance, legal, operational, financial, or domain-specific writing, keep the correct term when replacing it would reduce precision.

## Family 7. Format and mechanics

- **Em dashes.** Follow the applicable house style.
- **Bold as emphasis-by-default.** If everything is emphasized, nothing is.
- **Inline-header vertical lists.** Watch for every bullet opening with a bold label and a colon.
- **Emojis in headings or bullets.** Use only when the intended voice or channel calls for them.
- **Curly quotes in web copy and plain text.** Correct typography in a typeset book, so do not flag them there.
- **Title Case In Headings.** Follow the writer's or publication's house style.
- **Sycophancy.** "Great question", "You're absolutely right", "Certainly", and similar automatic praise.
- **Chatbot artifacts left in content.** "I hope this helps", "Let me know if", "Here is a", when they are not natural to the intended channel.
- **Knowledge-cutoff hedging.** "As of my last update", "While specific details are limited", and similar boilerplate.

# Protected content

Do not clean, paraphrase, normalize, or humanize material that must remain exact unless the user explicitly authorizes it.

Protected content includes:
- direct quotations,
- legal or contractual language,
- regulatory text,
- statutes or policy excerpts,
- citations and source titles,
- code,
- commands,
- filenames,
- paths,
- URLs,
- API fields,
- database field names,
- configuration values,
- product names,
- approved slogans or locked copy,
- any text the user identifies as exact, locked, quoted, final, or source-controlled.

When protected content contains an AI tell, note it in AUDIT mode only if useful. Do not rewrite it.

# What this skill must never do

## Do not strip voice

A flattened, opinion-free paragraph can read as machine-made just as loudly as a puffed-up one.

Vary sentence length. Keep reactions, uncertainty, first person, humor, bluntness, and imperfect rhythm where they belong.

Removing an AI tell must not remove personality with it.

**Where this skill and the writer's own voice disagree, the voice wins.**

## Do not replace precision with casual language

Technical writing is allowed to sound technical.

Do not replace the correct domain term merely because that term appears on a tell list.

## Do not manufacture personality

Do not add slang, typos, fake vulnerability, forced contractions, fake anecdotes, or artificial roughness merely to make text look human.

## Do not invent facts while rewriting

A cleaner sentence must preserve the original claim.

If a weak sentence cannot be fixed without adding unsupported information, flag it instead of inventing support.

# Method

1. Search for the families above.
2. Read for what search cannot see: self-narrating asides, rule-of-three cadence, bold overuse, synonym cycling, artificial balance, and repeated sentence shapes.
3. Classify before changing: real tell, legitimate technical term, protected content, or intentional voice.
4. Rewrite by exact target, not blind pattern replacement.
5. Re-run after fixing. A replacement can introduce a different tell.

# Mode-specific output

## WRITE

Return only the requested writing unless the user asks for an explanation.

Do not add:
- "Here is..."
- process commentary,
- a cleanup report,
- claims that the result is human,
- claims that AI detection tools will not detect it.

## AUDIT

Report only meaningful hits.

Preferred format:

`location — tell — short fix`

Do not bury the findings in a long essay.

If there are no meaningful tells, say so plainly.

## REWRITE

Return the revised text.

When useful, briefly identify major changes after the rewrite, but do not narrate every edit unless the user asks.

# Interaction with other writing skills

This skill owns the **AI-tell detection and meta-commentary problem**.

If another editing or house-style system is also in use:
- do not duplicate findings,
- do not run overlapping passes merely to create more output,
- use the narrowest tool that solves the task,
- let the higher-priority house style control when rules conflict.

This skill must not depend on another named model, vendor, assistant, or third-party skill in order to function.

# Success standard

The skill succeeds when the writing:
- sounds like the intended writer rather than a generic assistant,
- removes unnecessary machine-like emphasis and scaffolding,
- keeps useful judgment and personality,
- preserves technical precision,
- leaves protected content alone,
- and does not call attention to the cleanup itself.

The goal is not to make writing "undetectable."

The goal is to make it better writing.

# Origin and acknowledgments

AI Tells was created and developed by Jerry Curl.

Its initial baseline drew from established public resources describing common AI-writing patterns, including Wikipedia's *Signs of AI writing* / WikiProject AI Cleanup and other published vocabulary lists.

Those sources informed the starting point. AI Tells extends that base with additional observed patterns and its own operating method, including meta-commentary detection, construction-level analysis, contextual judgment, protected-content handling, WRITE/AUDIT/REWRITE modes, and regression-oriented testing.

The referenced public sources are acknowledged as inputs, not as authors or owners of this skill.

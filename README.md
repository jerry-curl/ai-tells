# ai-tells

A Claude skill that finds the phrases mark writing as machine-made, and cuts them without flattening the voice underneath.

There are already good lists of AI writing patterns. This one exists because they share a blind spot.

## The gap this fills

Every published list I could find is built from **encyclopedic and marketing prose**. Wikipedia's *Signs of AI writing* is the best of them and it catalogues 24 patterns from cleaning up Wikipedia articles. The vocabulary lists ("delve", "tapestry", "pivotal") come from analysing published content.

Encyclopedia articles never talk to the reader. Marketing copy talks *at* them.

So none of those lists catch **an assistant narrating its own emphasis**:

> "Worth noting: the deploy failed."
> "Said plainly, this is the part that matters."
> "Two things worth you knowing."

That family survives every existing sweep, and if you work with an AI assistant daily it is probably the pattern you are actually drowning in.

## The rule underneath it

**A tell announces that a point matters instead of making it matter.**

If a sentence needs a label telling the reader to pay attention, the sentence is not doing its job. Cut the label and keep the sentence. If the sentence cannot survive without its label, the sentence was the problem.

Or, sharper: *if you have to announce that something is worth noting, it probably isn't.*

## Ban the construction, not the instances

This is the most useful thing here and it was learned by failing at it.

A 54-note vault was swept clean of "worth noting", "worth knowing" and "worth keeping". **The very next message written by the same assistant contained "two things worth you knowing."**

The strings were gone. The grammar survived and immediately grew a new variant.

So work at the level of the shape: `worth` + a gerund aimed at the reader's attention. Worth noting, worth knowing, worth you knowing, worth mentioning, worth saying, worth recording, worth stating, worth carrying. All the same move.

**How people actually talk instead:**

> "I found a couple of things to tell you about."
> "I found two things to let you know."

The difference is who the sentence is about. *Worth you knowing* is about the information's importance. *I found two things to tell you* is about a person who found something and is telling you.

## The line that stops this doing damage

`worth` + gerund is a tell when it grades **information** for the reader. Cut it.

It is ordinary English when it grades an **action** as a good use of effort. "That domain is worth chasing." "Not worth retrying." "Worth revisiting if video work starts."

Those weigh cost against benefit. They are opinions, and opinions are the thing that is supposed to survive.

In one real sweep, 83 instances were found and 17 were cut. The other 66 were assessments and stayed. **Judgement, not find-and-replace.**

The same caution applies to the vocabulary list. "Key" and "crucial" are ordinary English. What marks them is frequency and the puffery they usually arrive with.

## What it will not do

Strip the voice. A flattened, opinion-free paragraph reads as machine-made just as loudly as a puffed-up one. Removing an AI tell must not remove the personality with it.

Where this skill and the writer's own voice disagree, the voice wins.

## Install

Claude Code, or anywhere skills live in a folder:

```
~/.claude/skills/ai-tells/SKILL.md
```

Drop `SKILL.md` there and it becomes available. Ask it to check a draft, or name a phrase you think is a tell and ask whether it is one.

It **detects by default** and reports rather than rewriting. On your own prose, that is almost always the right behaviour.

## Method that works

1. Grep for the phrase families. Seconds, and it catches most of it
2. Read for what grep cannot see: the self-narrating aside, rule-of-three cadence, bold-as-default, synonym cycling
3. Rewrite by exact string, never by regex. These are judgement calls, and a regex that matches something you did not picture mangles a document quietly
4. **Re-run after fixing, every time.** A replacement can introduce a different tell. Real example from this project: "not just published copy" was rewritten to "Not only in published copy", which is a listed template

## Related work, so you can pick the right one

- `humanizer` carries 24 patterns from [Wikipedia's *Signs of AI writing*](https://en.wikipedia.org/wiki/Wikipedia:Signs_of_AI_writing) with before-and-after pairs. Better on a full chapter or anything going to print
- `no-ai-slop` is a quick pass on a short draft

This skill covers the meta-commentary gap both leave. Do not run two and report the same finding twice.

## Licence and attribution

**CC BY-SA 4.0.** Families 2 through 6 derive from Wikipedia's *Signs of AI writing*, which is CC BY-SA, so this inherits it. See `ATTRIBUTION.md` for the full list of sources.

The meta-commentary family and the ban-the-construction rule came from a user noticing them in an assistant's own output. Those are the original contribution and they carry the same licence as the rest.

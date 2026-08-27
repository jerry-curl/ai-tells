---
name: ai-tells
description: Find and remove the phrases that mark writing as machine-made, with the emphasis on meta-commentary that no other list covers. Use when checking or cleaning any draft, note, email, report, web page or message before it goes out, when the user says writing "sounds like AI" or names a specific phrase as a tell, or when sweeping a folder of existing documents. Detects by default and reports rather than rewriting.
---

# AI tells

Find the phrases and constructions that mark writing as machine-made, and cut them without flattening the voice underneath.

## Two jobs

**Detect, by default.** List each hit: the file and line, the phrase, and the fix in a few words. Change nothing. On someone's own prose, detecting and letting them decide is almost always right.

**Rewrite, only when asked.** Then propose rather than apply on anything already in review.

## The rule underneath all of it

**A tell announces that a point matters instead of making it matter.** That is the whole family. If a sentence needs a label telling the reader to pay attention, the sentence is not doing its job. Cut the label and keep the sentence. If the sentence cannot survive without its label, the sentence was the problem.

Or, sharper: **if you have to announce that something is worth noting, it probably isn't.**

## BAN THE CONSTRUCTION, NOT THE INSTANCES

This is the most useful rule here and it was learned by failing at it.

A vault of 54 notes was swept clean of "worth noting", "worth knowing" and "worth keeping". **The very next message written by the same assistant contained "two things worth you knowing."** The strings were gone; the grammar survived and immediately grew a new variant.

**So work at the level of the shape.** `worth` + a gerund aimed at the reader's attention: worth noting, worth knowing, worth you knowing, worth mentioning, worth saying, worth recording, worth stating, worth naming, worth carrying, worth writing down. All the same move.

**How people actually talk instead:**

> "I found a couple of things to tell you about." · "I found two things to let you know." · "I found a couple of things to talk about."

The difference is who the sentence is about. *Worth you knowing* is about the information's importance. *I found two things to tell you* is about a person who found something and is telling you.

### The line that matters, because over-applying this does real damage

**`worth` + gerund is a tell when it grades INFORMATION for the reader.** Cut it.

**It is ordinary English when it grades an ACTION as a good use of effort.** "That domain is worth chasing." "Not worth retrying." "Worth revisiting if video work starts." Those weigh cost against benefit. They are opinions, and opinions are the thing that is supposed to survive.

In one real sweep, 83 instances were found and 17 were cut. The other 66 were assessments and stayed. **Judgement, not find-and-replace.**

## Family 1. Meta-commentary

**The gap no published list covers.** Wikipedia's guide and most ChatGPT word-lists are built from encyclopedic and marketing prose. Encyclopedia articles never talk to the reader, so nothing there catches an assistant narrating its own emphasis. This family is the one that survives every other sweep.

said plainly · stated plainly · worth noting · worth knowing · worth keeping · worth saying · worth noticing · and that is the point · which is the point · that is the whole point · the whole reason · the transferable part · the part that matters · to be clear · let me be clear · the reality is · the truth is · make no mistake · here is the thing · what this means is · to put it simply · put simply · in other words · the key takeaway · the bottom line

**Also in this family: the self-narrating aside.** A sentence that stops to explain why the previous sentence was included. *"Recorded because a rollback nobody wrote down is not a rollback plan."* The information is fine. Narrating its own value is the tell. No grep catches this one; it needs reading.

## Family 2. Throat-clearing openers

it's important to note that · it's worth noting that · it's crucial to understand that · it should be noted that · one could argue that · when it comes to · in the realm of · in the world of · in today's fast-paced world · in an ever-evolving landscape · in the digital age · in a world where · as we navigate · at its core · in essence · that being said · with that in mind · in light of this · with regard to

## Family 3. Sentence templates

it's not just X, it's Y · this isn't merely X, it's Y · not only X but also Y · from X to Y where X and Y are not on a scale · whether you're X or Y · on the one hand, on the other hand · as we navigate the complexities of · a wide range of · a myriad of · a wealth of

**The rule-of-three cadence belongs here.** Three items, three clauses, three examples, forced into groups to sound complete. Not greppable; read for it.

## Family 4. Grand-finale closers

in conclusion · in summary · to summarize · at the end of the day · ultimately · this highlights the need for · this underscores the importance of · this serves as a reminder that · this stands as a testament to · this paves the way for · this holds the potential to · the implications are far-reaching · the possibilities are endless · only time will tell · it remains to be seen · exciting times ahead · a step in the right direction

## Family 5. Transitions and hedges

furthermore · moreover · additionally · consequently · subsequently · nevertheless · nonetheless · thus · hence · therefore · importantly · notably · crucially · arguably · undoubtedly · indeed · it could potentially possibly

## Family 6. Vocabulary

**Verbs:** delve · leverage · utilize · foster · navigate · embark · unlock · unleash · unravel · harness · empower · facilitate · optimize · streamline · elevate · enhance · bolster · underscore · showcase · spearhead · revolutionize · transform · cultivate · champion · illuminate · demystify · embrace · resonate · transcend · propel · catalyze · galvanize · orchestrate · curate · supercharge · reimagine · redefine · align · amplify · unveil · unpack · shed light on · dive deep into

**Adjectives:** crucial · pivotal · vital · essential · paramount · integral · robust · comprehensive · multifaceted · nuanced · intricate · seamless · dynamic · vibrant · transformative · groundbreaking · cutting-edge · state-of-the-art · innovative · unprecedented · remarkable · notable · invaluable · indispensable · profound · compelling · captivating · meticulous · holistic · bespoke · unparalleled · ever-evolving · fast-paced · actionable · impactful · game-changing · commendable · noteworthy

**Nouns and metaphors:** tapestry · landscape (abstract) · realm · journey · beacon · labyrinth · symphony · mosaic · cornerstone · testament · paradigm · synergy · ecosystem · framework · roadmap · treasure trove · game-changer · powerhouse · plethora · zeitgeist · bastion · odyssey · crossroads · frontier · horizon · catalyst · linchpin · bedrock · kaleidoscope · deep dive · interplay

**These are not banned outright.** "Key" and "crucial" are ordinary English. What marks them is frequency and the puffery they usually arrive with.

## Family 7. Format and mechanics

- **Em dashes.** Use the house rule where one exists; many writers want zero. Hyphens in ordinary compound words are fine
- **Bold as emphasis-by-default**, until nothing stands out
- **Inline-header vertical lists**, every bullet opening with a bolded label and a colon
- **Emojis** in headings or bullets
- **Curly quotes** in web copy and plain text. Correct typography in a typeset book, so do not flag them there
- **Title Case In Headings**
- **Sycophancy.** "Great question", "You're absolutely right", "Certainly"
- **Chatbot artifacts left in content.** "I hope this helps", "Let me know if", "Here is a"
- **Knowledge-cutoff hedging.** "As of my last update", "While specific details are limited"

## What this must never do

**Stripping tells must not strip voice.** A flattened, opinion-free paragraph reads as machine-made just as loudly as a puffed-up one. Vary sentence length. Keep the reactions, the uncertainty, the first person where it fits. Removing an AI tell must not remove the personality with it.

**Where this skill and the writer's own voice disagree, the voice wins.**

## Method that works

1. **Grep for the families above.** Seconds, and it catches most of it
2. **Read for what grep cannot see:** the self-narrating aside, rule-of-three cadence, bold overuse, synonym cycling
3. **Rewrite by exact string, never by regex.** These are judgement calls, and a regex that matches something you did not picture mangles a document quietly
4. **RE-RUN AFTER FIXING, EVERY TIME.** A replacement can introduce a different tell. One real example: "not just published copy" was rewritten to "Not only in published copy", which is a family 3 template

## Related skills, so nothing is done twice

`humanizer` carries 24 patterns from Wikipedia's *Signs of AI writing* with before-and-after pairs, and is the better choice on a full chapter or anything going to print. `no-ai-slop` is a quick pass on a short draft. **This skill covers the meta-commentary gap both of them leave.** Do not run two and report the same finding twice.

## Tooling, where a shell is available

- `.claude/scripts/ai-tells-sweep.ps1 <path> [-Detail] [-Family 1,2,3]` greps a file or folder, reports file, line and phrase, counts em dashes separately
- `.claude/scripts/ai-tells-fix.ps1 -Path <file> -Table $table` applies exact-string rewrites and refuses to report success when a replacement did not land

## Sources

Wikipedia, *Signs of AI writing*, WikiProject AI Cleanup. Plus two published vocabulary lists, and the meta-commentary family, which came from a user noticing it in an assistant's own output and which no published list carries.

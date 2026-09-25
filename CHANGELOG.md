# Changelog

All notable changes to AI Tells are documented here.

## [1.1.0] — 2026-09-25

### Added

- Meta-commentary family: labels that grade a sentence instead of saying it.
  - Drama adverbs such as "quietly".
  - Honesty labels such as "one honest caveat", "to be honest" and "frankly", which imply the surrounding sentences were not honest.
  - Build-up before news, such as "you should hear it from me first".
- Regression tests 16 to 18 for the new patterns.

## [1.0.0] — 2026-08-27

First public release of AI Tells, created and developed by Jerry Curl.

### Added

- WRITE, AUDIT, and REWRITE operating modes.
- Construction-level detection instead of simple phrase blacklisting.
- Meta-commentary family.
- Contextual distinction between information-grading and action-grading uses of `worth`.
- Throat-clearing, template, finale, transition, vocabulary, formatting, and mechanics families.
- Protection for quotations, legal text, code, commands, filenames, paths, citations, and other exact-content material.
- Technical-language exception to avoid damaging precise domain writing.
- Voice-preservation rules.
- Regression tests.
- Model-neutral design.

### Design principle

> Ban the construction, not the instances.

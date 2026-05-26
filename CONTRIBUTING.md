# Contributing

Thanks for considering a contribution to AI Builder Decision Analyst. This is a small, opinionated library, so a few notes on what fits.

## What this repo is

A set of 11 Claude Code skills organized around the four phases of a product decision (DECIDE / BUILD / COMMUNICATE / LEARN), plus two templates (`decision-journal.md`, `anti-portfolio.md`).

## What contributions fit

- **Sharper prompts.** If a skill misses common cases, surfaces the wrong question, or produces fluffy output, tighten it.
- **New skills** that fill a clear gap in one of the four phases and don't overlap with an existing skill. Prefer fewer, sharper skills over more, vaguer ones.
- **Better templates.** The decision journal and anti-portfolio templates are example formats - improvements that make them faster to fill out are welcome.
- **Docs and examples.** README clarity, broken commands, missing context, install gotchas.

## What does not fit

- New skills that overlap with an existing one. If a skill needs more capability, edit it.
- Skills for general writing, coding, or non-decision-making tasks - this library is intentionally scoped to product decision-making.
- Adding dependencies. The repo is intentionally markdown-only.

## How to contribute

1. **Open an issue** describing the gap or change you want to make. Wait for a thumbs-up from a maintainer before doing significant work.
2. **Branch** from `main` using a short descriptive name (e.g., `feat/willingness-to-pay-test`, `fix/decision-audit-prompt`).
3. **Make the change.**
   - New skill: add the file at `skills/<skill-name>.md` and register it in the README catalog under the right phase.
   - Skill edit: keep the existing structure (PHASE headings, output format) so users don't have to relearn.
4. **Update the README** if the change adds a skill, removes one, or changes how it's invoked.
5. **Open a PR** with a one-line summary of the change and the decision-making rationale.

## Skill file format

Every skill in `skills/` starts with YAML frontmatter and a clear opening section:

```markdown
---
name: skill-name
description: One-sentence summary of what the skill produces and when to invoke it.
---

# Skill Title — One-line tagline

What this skill does and what it does NOT do.

## PHASE 1: Input Collection
...
## PHASE 2: ...
...
## Output
...
```

Keep skill output structured (tables, ranked lists, explicit decisions) rather than narrative paragraphs.

## Tone

Direct. Opinionated. Backed by a clear reason. These are decision-making skills - hedging and "it depends" defeat the purpose.

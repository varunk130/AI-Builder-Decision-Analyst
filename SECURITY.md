# Security Policy

AI Builder Decision Analyst is a set of Markdown skills plus example templates. If you find a security issue - whether in the skill instructions, the decision-journal templates, or anything else that could lead a user to leak sensitive product data or credentials when following the guidance verbatim - please report it privately rather than opening a public issue.

## Reporting a vulnerability

Use one of these private channels:

1. **GitHub private vulnerability reporting** - open a private advisory on this repository's Security tab. This is the preferred channel.
2. **Direct message** - reach the maintainer through the contact information on their GitHub profile.

When reporting, please include:

- A clear description of the issue and its potential impact
- Steps to reproduce (a minimal proof-of-concept if possible)
- The affected file or skill name
- Any suggested remediation
- Whether you would like public credit when the fix is released

## What to expect

- **Acknowledgment** within 7 days
- A **triage decision** (accepted, needs more info, out of scope) within 14 days
- A **coordinated disclosure timeline** once the issue is confirmed
- **Public credit** in the release notes, with your consent

## Scope

In scope:

- Skill instructions that could cause sensitive product data, customer data, or credentials to be exposed if followed as written
- Example templates (decision-journal.md, anti-portfolio.md) that imply unsafe handling of confidential strategy material

Out of scope:

- Findings that require the user to paste genuine production data or live customer information into the example templates
- Issues in Claude Code itself or other upstream tools - please report those to the relevant project
- Wording or style concerns - open a regular issue or pull request for those

## Supported versions

Only the latest commit on `main` is actively maintained. Older forks or snapshots are not patched.

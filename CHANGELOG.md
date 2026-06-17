# Changelog

Notable changes to this project, newest first.

The format is loosely based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/).

## [Unreleased]

### Documentation

- Updated the ai-customer-discovery-skills status in Related Work (5 of 12 skills shipped).
- Rewrote the Setup section so install commands point at the actual `skills/` directory (previous instructions referenced a `.claude/commands/` path that did not exist in the repo).
- Rewrote the Repo Structure tree to match the real layout (removed references to a fictional `CLAUDE.md` at root and a non-existent `.claude/commands/` folder).
- Added the orphan `assets/05-Framework.png` to the Decision Sequence section so the shipped asset is actually rendered.
- Linked the LICENSE file from the README License section.
- Fixed capitalization and tightened wording in the footer ("Ai Builders" → "AI builders").

### Added

- `LICENSE` file with the MIT text (previously the README claimed MIT but no file existed).
- `SECURITY.md` with a private vulnerability reporting channel.
- `CONTRIBUTING.md` with skill format conventions, scope, and contribution flow.
- `CODE_OF_CONDUCT.md`.
- `.gitignore` covering OS files, editor state, and Claude Code's local cache and session directories.

### Removed

- Empty 2-byte `placeholder` stub files in `skills/` and `templates/` that were left over from when the directories were first added to git.

## [0.1.0] - 2026-05

- First public release.
- 11 Claude Code skills across the DECIDE, BUILD, COMMUNICATE, and LEARN layers.
- Decision Journal and Anti-Portfolio templates for the LEARN loop.
- Carousel assets covering the framework overview, decision audit output, and improvement options.

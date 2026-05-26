# AI Builder Decision Analyst

**11 Claude Code skills that catch bad bets before you ship, sharpen every decision, and compound your productivity and ROI over time.**

![AI Builder Decision Analyst Overview](assets/02-Overview.png)

## What This Is

A set of Claude Code slash commands organized around how product decisions actually flow. Each skill targets a specific decision failure mode. A `CLAUDE.md` file holds your product context, decision history, and known biases so every skill has the full picture.

No app. No API. Markdown files in a folder.

## The 11 Skills Across Four Layers

![All 11 Skills](assets/01-All-11-Skills.png)

### ✅ DECIDE — Before you commit

| # | Command | What It Does |
|---|---------|-------------|
| 1 | `/project:assumption-check` | Surface 5 ranked untested assumptions with cheapest validation tests |
| 2 | `/project:downside-case` | Build the strongest possible case for NOT building a feature |
| 3 | `/project:10x-or-10-percent` | Evaluate whether a bet is incremental improvement or transformative change |

### 🛠️ BUILD — Before you ship

| # | Command | What It Does |
|---|---------|-------------|
| 4 | `/project:scope-creep-detector` | Flag every scope-expanding sentence in a PRD or spec |
| 5 | `/project:pre-mortem` | Write a realistic failure post-mortem from 6 months in the future |
| 6 | `/project:strategy-smell-test` | Apply 7 smell tests to detect weak strategy disguised as good strategy |

### 🧠 COMMUNICATE — Before you present

| # | Command | What It Does |
|---|---------|-------------|
| 7 | `/project:stakeholder-translator` | Show how 4 stakeholders will actually read your message |
| 8 | `/project:say-no-script` | Generate 3 pushback scripts for stakeholder requests you need to decline |
| 9 | `/project:exec-summary-sharpener` | Find weak spots in executive-facing documents without rewriting them |

### 🔁 LEARN — After you decide

| # | Command | What It Does |
|---|---------|-------------|
| 10 | `/project:decision-audit` | Analyze your decision journal to reveal patterns, biases, and improvement areas |
| 11 | `/project:portfolio-validation` | Grade your product instincts by analyzing bets you missed or got wrong |

## The Decision Intelligence Report

The LEARN layer is what changed things for me. Log your decisions in the journal, run `/project:decision-audit`, and get a report showing where you optimize for speed when experimentation wins, where you skip structured evaluation, and where your confidence doesn't match your outcomes.

![Decision Audit Output](assets/03-Decision-Audit.png)

![Improvement Options](assets/04-Improvement-Options.png)

## Setup (5 minutes)

### Prerequisites

- [Claude Code](https://docs.anthropic.com/en/docs/claude-code) installed and authenticated

### Option 1: Clone and use

```bash
git clone https://github.com/varunk130/AI-Builder-Decision-Analyst.git
cd AI-Builder-Decision-Analyst

# Install the skills into your user-level Claude Code commands directory
mkdir -p ~/.claude/commands
cp skills/*.md ~/.claude/commands/

# Then run any command from any project
claude "/user:assumption-check We're building a self-serve analytics dashboard for SMB customers"
```

### Option 2: Add to an existing project

```bash
mkdir -p your-project/.claude/commands
cp AI-Builder-Decision-Analyst/skills/*.md your-project/.claude/commands/
cp -r AI-Builder-Decision-Analyst/templates/ your-project/templates/
```

### Option 3: User-level commands (available in all projects)

```bash
mkdir -p ~/.claude/commands
cp AI-Builder-Decision-Analyst/skills/*.md ~/.claude/commands/
# Now use /user:assumption-check from any project
```

## How to Use the Decision Journal

1. Open `templates/decision-journal.md`
2. Log each decision using the template format (takes ~2 minutes per entry)
3. After 15-20 entries, run `/project:decision-audit`
4. Review your Decision Intelligence Report
5. Run again in 90 days to track how your patterns shift

The journal captures: what you decided, what you rejected, what you optimized for, who influenced you, your confidence level, and the outcome.

## The Decision Sequence

For major product decisions, run these in order:

```
1. /project:assumption-check       → Find what you don't know
2. /project:downside-case          → Stress-test the idea
3. /project:10x-or-10-percent      → Clarify the bet size
4. /project:scope-creep-detector   → Tighten the spec
5. /project:pre-mortem             → Anticipate failure
6. /project:strategy-smell-test    → Validate the strategy
```

If your idea survives all 6, ship it with confidence.

## How to Get the Most Out of It

**Be specific in your input.** "We're building a dashboard" is weak. "We're building a self-serve analytics dashboard for SMB e-commerce brands who currently export CSV reports weekly and share them in Slack" is strong.

**Disagree with the output.** These skills are designed to push back. If you can refute every argument, your thinking is solid. If you can't refute one — you found a blind spot.

**Log everything.** The LEARN layer gets sharper the more decisions you log. 20 entries is the minimum for meaningful pattern detection.

## Repo Structure

```
AI-Builder-Decision-Analyst/
├── README.md
├── skills/
│   ├── assumption-check.md        # DECIDE layer
│   ├── downside-case.md
│   ├── 10x-or-10-percent.md
│   ├── scope-creep-detector.md    # BUILD layer
│   ├── pre-mortem.md
│   ├── strategy-smell-test.md
│   ├── stakeholder-translator.md  # COMMUNICATE layer
│   ├── say-no-script.md
│   ├── exec-summary-sharpener.md
│   ├── decision-audit.md          # LEARN layer
│   └── portfolio-validation.md
├── templates/
│   ├── decision-journal.md        # Log your decisions here
│   └── anti-portfolio.md          # Log your misses here
└── assets/                        # Carousel images
```

## Contributing

Reach out to Varun if you are interested in collaborating.

## License

MIT — see [LICENSE](LICENSE) for the full text.

## Disclaimer

All decision data in the templates is fictional and anonymized. The entries are examples to show how the journal and audit work. Replace them with your own decisions to get real value from the LEARN layer.

---

**Built by [Varun Kulkarni](https://www.linkedin.com/in/varun-kulkarni/) — AI Product Manager building tools that make Ai Builders increase impact 10x.**
Give stars or leave a review if you like this!

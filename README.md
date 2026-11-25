# mk-ai-skills

Reusable skills for AI coding and writing agents. Each skill is self-contained under `skills/` and follows the `SKILL.md` convention.

## Skills

### natural-writing

Drafts and edits clear, natural prose in English and Spanish. It preserves the writer's meaning and voice while removing formulaic language, vague claims, and other common signs of machine-written copy.

### analyze-value-and-behavior

Analyzes business ideas, product decisions, UX, copy, persuasion, and communication through a focused selection of strategic frameworks, then synthesizes the findings into one recommendation or deliverable.

### Product management

Adapted from [phuryn/pm-skills](https://github.com/phuryn/pm-skills); see [THIRD-PARTY-NOTICES.md](THIRD-PARTY-NOTICES.md).

- **Discovery:** `product-discovery` (the full cycle), `brainstorm-ideas-existing`, `brainstorm-ideas-new`, `identify-assumptions-existing`, `identify-assumptions-new`, `prioritize-assumptions`, `brainstorm-experiments-existing`, `brainstorm-experiments-new`, `opportunity-solution-tree`, `prioritize-features`, `analyze-feature-requests`, `interview-script`, `summarize-interview`, `metrics-dashboard`
- **Strategy:** `product-strategy`, `product-vision`, `value-proposition`, `monetization-strategy`
- **Risk:** `strategy-red-team`, `pre-mortem`
- **Research:** `market-sizing`, `market-segments`, `customer-journey-map`, `survey-design`

## Installation

Copy the complete skill directory into the skills folder used by your agent. Common locations are:

- Codex: `~/.codex/skills/`
- Claude: `~/.claude/skills/`

Keep the directory intact so the language references and agent metadata remain available.

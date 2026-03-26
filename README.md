# VibeCorp CoworkSkills

Strategic thinking skills for Claude.ai Cowork. Each skill is a self-contained prompt that activates a specific reasoning mode — no tools, no MCP, no setup. Just paste and think.

## Complete Beginner? Start Here

Never used Claude or GitHub before? No problem.

1. **[Step-by-Step Guide](docs/STEP_BY_STEP_GUIDE.md)** — Takes you from zero to running your first skill in 5 minutes
2. **[FAQ](docs/FAQ.md)** — Answers every question, starting from "What is Claude?"

No coding, no installs, no technical knowledge required.

## Who This Is For

- **Startup founders** validating ideas, sizing markets, preparing for investors
- **Product managers** prioritizing roadmaps, managing stakeholders, driving change
- **Business strategists** stress-testing plans, building GTM strategies, modeling pricing
- **Anyone** who wants a structured thinking partner for strategic decisions

## Skills

| Skill | What It Does |
|-------|-------------|
| [ceo-thinking-partner](skills/ceo-thinking-partner.md) | 7 thinking modes: brainstorm, validate, stress-test, compare, command brief, theory test, direction check |
| [strategic-challenger](skills/strategic-challenger.md) | Mid-conversation reorientation — challenges assumptions, pushes back, argues the opposite |
| [problem-validation](skills/problem-validation.md) | 5 core questions to determine if a problem is real + evidence classification |
| [market-sizing](skills/market-sizing.md) | TAM/SAM/SOM + T-Score market timing methodology |
| [pricing-strategy](skills/pricing-strategy.md) | Van Westendorp 4-question test + willingness-to-pay frameworks |
| [gtm-playbook](skills/gtm-playbook.md) | Go-to-market: ICP, channels, marketplace strategy, 90-day roadmap |
| [investor-prep](skills/investor-prep.md) | One-pager, FAQ prep, 30-second narrative, pitch framing |
| [business-validation-flow](skills/business-validation-flow.md) | Full pipeline: idea → problem → evidence → market → revenue → GTM → build decision |
| [roadmap-planning](skills/roadmap-planning.md) | MoSCoW, ICE/RICE scoring, sprint planning, roadmap communication |
| [stakeholder-management](skills/stakeholder-management.md) | Power/Interest grid, RACI, communication cadence, alignment techniques |
| [change-management](skills/change-management.md) | ADKAR, resistance mapping, adoption curves, change communication |

## Quick Start

1. Open any skill file from the [skills/](skills/) folder
2. Copy the prompt between the `<!-- COPY FROM HERE -->` and `<!-- COPY TO HERE -->` markers
3. Paste it into a new [Claude.ai](https://claude.ai) conversation
4. Start talking about your specific situation

See [USAGE.md](skills/USAGE.md) for detailed instructions, tips, and a skill selection guide. See [FAQ](docs/FAQ.md) for common questions.

## How It Works

Each skill file contains:

- **Paste-ready prompt** — copy directly into Claude.ai to activate the reasoning mode
- **Framework/methodology** — the thinking behind the skill, so you understand what it's doing
- **Example usage** — realistic conversation showing the skill in action
- **When to use / when NOT to use** — guidance on picking the right skill

## Skill Combinations

Some skills chain naturally — the output of one becomes the input for the next:

```
Idea validation flow:
  problem-validation → market-sizing → pricing-strategy → gtm-playbook → investor-prep

Full business validation:
  business-validation-flow (orchestrates the above automatically)

Strategic planning:
  ceo-thinking-partner (mode: brainstorm) → roadmap-planning → stakeholder-management

Investment readiness:
  problem-validation → market-sizing → investor-prep

Organizational change:
  stakeholder-management → change-management

Mid-session reset:
  Any skill → strategic-challenger (paste mid-conversation to reorient)
```

See [USAGE.md — Skill Router Pattern](skills/USAGE.md#skill-router-pattern) for how to manage multi-skill workflows.

## Design Principles

- **Pure reasoning** — no tools, no file system, no MCP servers. Works in any Claude.ai conversation.
- **Self-contained** — each skill works independently. No dependencies between files.
- **Opinionated frameworks** — these aren't generic prompts. Each embeds specific methodologies with scoring systems, decision gates, and structured outputs.
- **Practical over theoretical** — every framework includes worked examples with real numbers.

## Documentation

| Document | What It Covers |
|----------|---------------|
| [Step-by-Step Guide](docs/STEP_BY_STEP_GUIDE.md) | Absolute beginner walkthrough — zero to first skill in 5 minutes |
| [FAQ](docs/FAQ.md) | Common questions for beginners and intermediate users |
| [USAGE.md](skills/USAGE.md) | Three usage modes, skill routing, cross-validation, multi-chat management |
| [CONTRIBUTING.md](CONTRIBUTING.md) | How to contribute skills and improvements |
| [REPO_STANDARDS.md](REPO_STANDARDS.md) | Security standards and metadata scrub procedures |

## References

These resources informed the design of CoworkSkills:

- [Claude Skills Overview](https://zapier.com/blog/claude-skills/) — Zapier
- [Awesome Claude Skills](https://github.com/ComposioHQ/awesome-claude-skills) — ComposioHQ
- [The Complete Guide to Claude Skills](https://tylerfolkman.substack.com/p/the-complete-guide-to-claude-skills) — Tyler Folkman
- [Patience Is All You Need](https://medium.com/code-wild/patience-is-all-you-need-63b936d71eac) — Code Wild
- [Use Skills in Claude (Official)](https://support.claude.com/en/articles/12512180-use-skills-in-claude) — Anthropic
- [Building Skills for Claude (PDF)](https://resources.anthropic.com/hubfs/The-Complete-Guide-to-Building-Skill-for-Claude.pdf) — Anthropic
- [Claude Guides: Code, Cowork, Skills, Workflows](https://karozieminski.substack.com/p/claude-guides-code-cowork-skills-workflows) — Karo Zieminski

## Disclaimer

We are not affiliated with Anthropic. These are community-created skills, not officially supported products. Use at your own discretion.

## License

MIT

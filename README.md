# VibeCorp CoworkSkills

Strategic thinking skills for Claude.ai Cowork. Each skill is a self-contained prompt that activates a specific reasoning mode — no tools, no MCP, no setup. Just paste and think.

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

See [USAGE.md](skills/USAGE.md) for detailed instructions, tips, and a skill selection guide.

## How It Works

Each skill file contains:

- **Paste-ready prompt** — copy directly into Claude.ai to activate the reasoning mode
- **Framework/methodology** — the thinking behind the skill, so you understand what it's doing
- **Example usage** — realistic conversation showing the skill in action
- **When to use / when NOT to use** — guidance on picking the right skill

## Skill Combinations

Some skills chain naturally:

```
Idea validation flow:
  problem-validation → market-sizing → pricing-strategy → gtm-playbook → investor-prep

Full business validation:
  business-validation-flow (orchestrates the above automatically)

Strategic planning:
  ceo-thinking-partner (mode: brainstorm) → roadmap-planning → stakeholder-management

Organizational change:
  stakeholder-management → change-management

Mid-session reset:
  Any skill → strategic-challenger (paste mid-conversation to reorient)
```

## Design Principles

- **Pure reasoning** — no tools, no file system, no MCP servers. Works in any Claude.ai conversation.
- **Self-contained** — each skill works independently. No dependencies between files.
- **Opinionated frameworks** — these aren't generic prompts. Each embeds specific methodologies with scoring systems, decision gates, and structured outputs.
- **Practical over theoretical** — every framework includes worked examples with real numbers.

## License

MIT

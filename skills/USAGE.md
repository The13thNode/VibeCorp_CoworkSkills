# VibeCorp CoworkSkills — User Guide

How to use strategic thinking skills in Claude.ai. No plugins, no setup, no accounts beyond Claude.ai itself.

---

## What Are CoworkSkills?

CoworkSkills are paste-ready prompts that activate a specific reasoning mode in Claude.ai. Each skill is a structured expert — a thinking partner with a clear methodology, a set of frameworks, and a bias toward practical output.

Think of them as hiring a specialist for a conversation:
- Want to pressure-test your strategy? Paste the Strategic Challenger skill.
- Building a product roadmap? Paste the Roadmap Planning skill.
- Navigating a difficult board conversation? Paste the Stakeholder Management skill.

CoworkSkills are designed for startup founders and business strategists. They assume you have real problems, limited time, and no patience for generic advice.

**What they are:**
- Structured frameworks activated through a single paste
- Pure reasoning — no tools, no file system, no external integrations
- Reusable across different conversations and problems
- Designed to ask before they advise (they gather context first)

**What they are not:**
- Automation or agents (those live in Claude Code, not here)
- A replacement for domain experts, lawyers, or therapists
- Permanent memory — each conversation starts fresh (unless you use Projects)

---

## Three Ways to Use These Skills

There are three approaches, each with real trade-offs. Pick the one that fits how you work.

### Option A: Single Chat, Single Skill (Simplest)

Paste one skill into a fresh Claude.ai chat. One conversation, one framework, one problem.

**Best for:** Focused work on a single topic — validating one idea, sizing one market, prepping for one investor meeting.

**How to do it:**
1. Go to [claude.ai](https://claude.ai)
2. Start a new conversation
3. Paste the skill prompt (from the COPY FROM HERE / COPY TO HERE block)
4. Answer the questions and work through the framework

| Pros | Cons |
|------|------|
| No confusion — one framework, one context | No memory between chats |
| Clean context window, no hallucination across topics | Manual context transfer if you chain skills |
| Works on Free tier — no Projects needed | You re-explain your situation each time |
| Fastest to start | |

**Tool:** Claude.ai free chat (any tier)

### Option B: Claude Projects (Recommended for Multi-Skill Work)

Upload multiple skills to a Project's Knowledge base. Claude has access to all of them across every conversation in that project, with shared memory.

**Best for:** Ongoing product development where you need multiple perspectives — market sizing today, pricing tomorrow, GTM next week — all with persistent context about your company.

**How to do it:**
1. Create a new Project in Claude.ai (requires Pro or Team plan)
2. Upload 3-4 skill .md files to the Project Knowledge section
3. Start conversations within the project — Claude loads relevant skills automatically
4. Your company context persists across conversations

For official setup instructions, see: [Use Skills in Claude](https://support.claude.com/en/articles/12512180-use-skills-in-claude)

| Pros | Cons |
|------|------|
| Memory persists across conversations | Requires Pro or Team plan |
| Skills always available — no re-pasting | Claude may blend frameworks if too many skills loaded |
| Claude picks the right skill based on your question | Uses more tokens per conversation |
| Shared context means less repetition | Requires deliberate project setup |

**Tool:** Claude.ai Projects (Pro/Team plan)

### Option C: Isolated Chats, No Shared Memory (Power User)

Run separate chats per skill with deliberately no memory sharing. Each conversation is a sealed environment.

**Best for:** Working on multiple projects simultaneously without cross-contamination. A consulting founder running three different ventures. An advisor working with multiple startups.

**How to do it:**
1. Open separate conversations for each skill
2. Turn off memory sharing (or use separate browser profiles)
3. Name each chat clearly (e.g., "Market-Sizing-ProjectX", "GTM-ProjectY")
4. Manually transfer key decisions between chats when needed

| Pros | Cons |
|------|------|
| Zero hallucination across projects | Manual transfer of decisions between chats |
| Clean separation of concerns | More effort to maintain coherence |
| No risk of framework blending | You are the integration layer |
| Works on any tier | Requires discipline to name and organize chats |

**Tool:** Claude.ai with memory OFF per chat, or separate browser profiles

### Comparison Table

| | Single Chat | Projects | Isolated Chats |
|---|---|---|---|
| **Setup effort** | None | Medium | Low |
| **Memory** | None | Shared | None (deliberate) |
| **Multi-skill** | No | Yes (auto-routed) | Yes (manual) |
| **Cross-contamination risk** | None | Low-medium | None |
| **Cost** | Free tier works | Pro/Team required | Free tier works |
| **Best for** | One-off tasks | Ongoing projects | Multi-project work |

---

## Skill Combinations

Some skills chain naturally. The output of one becomes the input for the next.

### Idea Validation Flow
```
problem-validation → market-sizing → pricing-strategy → gtm-playbook → investor-prep
```
Start with "is this a real problem?" and end with a pitch-ready narrative. Each skill builds on the previous one's conclusions.

### Full Business Validation
```
business-validation-flow (orchestrates the above automatically)
```
If you want the full pipeline in a single conversation, `business-validation-flow.md` has all 7 stages with built-in go/no-go gates. This is the single-chat alternative to chaining individual skills.

### Strategic Planning
```
ceo-thinking-partner (mode: brainstorm) → roadmap-planning → stakeholder-management
```
Generate options, sequence them into a roadmap, then plan the alignment conversations with your team and board.

### Organizational Change
```
stakeholder-management → change-management
```
Map who matters and what they care about, then build the adoption and communication plan.

### Investment Readiness
```
problem-validation → market-sizing → investor-prep
```
Validate your story with data before building the pitch. Investors ask the same questions these skills answer.

### Mid-Session Reset
```
Any skill → strategic-challenger (paste mid-conversation)
```
Unlike other skills, `strategic-challenger.md` is designed to be pasted mid-conversation. Use it when Claude is being too agreeable or the discussion has gone off-track.

---

## Skill Router Pattern

When you have multiple skills available, you need a way to pick the right one. There are four routing approaches:

### Automatic Routing (Projects Only)
When multiple skills are uploaded to a Claude Project's Knowledge base, Claude reads your intent and loads the relevant skill automatically. Ask "help me size the market for this idea" and Claude activates the market-sizing framework without you specifying it.

**Limitation:** Works well with 3-4 skills. With 8+ skills loaded, Claude may blend frameworks or pick the wrong one. Keep your Project focused.

### Manual Routing
You paste the specific skill you want at the start of each chat. No ambiguity, no wrong picks.

**Best for:** Free tier users, or when you know exactly which framework you need.

### Chained Routing
Output of one skill feeds the next. You finish problem validation, copy the key conclusions, open a new chat, paste the market-sizing skill, and provide the conclusions as context.

**Best for:** Multi-stage analysis where each stage needs a clean framework.

### Orchestrator Chat Pattern
Maintain one "control room" chat that tracks which skills you've run and what decisions were made. This chat doesn't use a skill itself — it's your index.

**How it works:**
1. Open an orchestrator chat (no skill pasted)
2. After each skill session, summarize the key decisions in the orchestrator
3. Before starting the next skill, check the orchestrator for context
4. The orchestrator tells you what to run next and what context to carry forward

**Best for:** Complex, multi-week strategic work where you're running 5+ skill sessions.

### Important Note
This is **not** the same as MCP-based skill routing in Claude Code. Claude Code has tool-based agents that can read files, execute code, and chain actions automatically. CoworkSkills are pure chat-based reasoning for Claude.ai — the human is always the router between conversations.

---

## Managing Multiple Chats

When you're running several skill sessions in parallel, organization matters.

**Name your chats by skill and date:**
- "CEO-Brainstorm-Mar26"
- "Market-Sizing-ProjectX"
- "Investor-Prep-SeriesA-Draft2"

**Keep an orchestrator chat as your index.** After each skill session, drop a 3-line summary into the orchestrator: what you ran, what you decided, what's next.

**When switching skills, transfer decisions — not transcripts.** Copy the 5-10 key conclusions, not the entire conversation. The new skill needs your decisions, not the reasoning path that got you there.

**Use strategic-challenger.md as a mid-conversation interrupt.** If any skill session starts going in circles or Claude becomes too agreeable, paste the challenger skill to force a reset.

**Review your orchestrator before each new session.** It takes 30 seconds and prevents you from re-doing work or contradicting earlier decisions.

---

## Cross-Skill Validation

When you run multiple skills, how do you ensure consistency? The answer depends on your setup.

### Scenario 1: Same Project, Shared Memory (Projects)
Claude remembers previous conversations. If your market-sizing session concluded "SOM is $5M" and your pricing session assumes a $50M market, Claude can flag the inconsistency — but only if both conversations happened within the same Project.

**Validation is semi-automatic.** Claude has the context to cross-check, but it won't always do so unprompted. Ask: "Is this consistent with what we concluded in our market-sizing conversation?"

### Scenario 2: Same Project, No Memory
If you've disabled memory within a Project, each conversation is independent. Claude cannot cross-validate because it doesn't know what happened in other chats.

**Validation is manual.** You must carry the key numbers and decisions between chats yourself.

### Scenario 3: Different Projects or Free Tier
No shared context at all. Each conversation is completely isolated.

**You are the validator.** Copy key conclusions between chats. Use the orchestrator chat pattern to track decisions and catch contradictions.

### Scenario 4: Single Chat with business-validation-flow.md
The `business-validation-flow.md` skill handles cross-validation internally. It runs all 7 stages sequentially in one conversation, with go/no-go gates between each stage. If your market size doesn't support your revenue model, the skill catches it at the gate.

**Validation is built in.** This is the recommended approach if you want automatic consistency checking without Projects.

### Recommendation
If cross-validation matters to you (and it should), choose one of:
- **Projects with memory ON** — semi-automatic cross-checking
- **business-validation-flow.md in a single chat** — fully internal validation with gates
- **Orchestrator chat pattern** — manual but systematic

Don't rely on hope. Pick a validation method before you start.

---

## When NOT to Use Multiple Skills

- **If your project is early stage**, `business-validation-flow.md` alone covers 80% of what you need. It walks you through idea → problem → evidence → market → revenue → GTM → build decision in one conversation. Don't over-complicate it.

- **Don't load all 11 skills into one Project.** Claude will blend frameworks, give confused advice, and waste tokens. Pick 3-4 skills relevant to your current phase.

- **If Claude starts mixing advice from different frameworks**, it's a sign you have too many skills loaded or the conversation is too long. Start a fresh chat with a single skill.

- **If you're exploring, not deciding**, just use `ceo-thinking-partner.md`. It has 7 modes that cover brainstorming through stress-testing. Save the specialized skills for when you know what you're working on.

- **If you don't have real data yet**, most skills will give you structured speculation instead of structured analysis. Run `problem-validation.md` first to identify what evidence you actually need, then go collect it before running the other skills.

---

## Skill Selection Guide

**I want to...** → **Use this skill**

| Goal | Skill File |
|---|---|
| Think through a major strategic decision | `ceo-thinking-partner.md` |
| Stress-test my strategy and find blind spots | `strategic-challenger.md` |
| Validate whether my problem is real and worth solving | `problem-validation.md` |
| Size a market and estimate opportunity | `market-sizing.md` |
| Design a pricing strategy | `pricing-strategy.md` |
| Build a go-to-market plan for a launch | `gtm-playbook.md` |
| Prepare for investor conversations or fundraising | `investor-prep.md` |
| Validate a full business model end-to-end | `business-validation-flow.md` |
| Build and prioritize a product or company roadmap | `roadmap-planning.md` |
| Map stakeholders and get alignment before a key decision | `stakeholder-management.md` |
| Roll out a change and drive adoption across a team | `change-management.md` |

**Not sure where to start?**
- New idea, no validation yet → `business-validation-flow.md`
- Existing project, need strategic clarity → `ceo-thinking-partner.md`
- Preparing to raise money → `investor-prep.md`
- Something feels off but you can't name it → `strategic-challenger.md`

---

## Troubleshooting Common Issues

**Claude responded but didn't ask the Phase 1 questions.**
Add a line after pasting: "I have just pasted a skill prompt. Please begin by asking me the Phase 1 questions." This resets the context.

**The skill seems to have been forgotten partway through a long conversation.**
Claude.ai has a context window — very long conversations can cause earlier instructions to fade. Start a fresh conversation with the skill pasted again, or re-paste the skill prompt mid-conversation.

**Claude is giving me generic advice instead of using the frameworks.**
The Phase 1 questions were not answered with enough specificity. Give more concrete details — specific numbers, competitors, team sizes, constraints. The frameworks activate when there is real context to work with.

**The output is too long and covering things I don't need.**
Tell Claude exactly what you need: "Focus only on the RICE scoring for items 3, 5, and 7. Skip the rest for now." Skills are designed to be used interactively, not consumed as a wall of output.

**I want a specific section without running the full skill.**
Ask directly: "Using the ADKAR model from the change management framework, help me diagnose why my team hasn't adopted the new CRM." You do not have to run the full Phase 1-7 structure every time.

**The skill asks questions I can't answer yet.**
That is useful information. If you cannot answer "What is the one metric that matters for this phase?" it means you have not yet defined it. The skill is surfacing a gap, not blocking you. Say "I don't know yet" and Claude will help you figure it out.

**Claude is mixing advice from different frameworks.**
You likely have too many skills loaded in a Project, or you pasted multiple skills in one chat. Start a fresh conversation with only the skill you need.

---

## How to Customize Skills for Your Needs

CoworkSkills are plain text files. They are yours to edit.

**Add company context to the top of a skill.** Before the skill prompt, add a section like:

```
Context about my company: We are a 15-person product analytics SaaS, Series A, $2M ARR,
selling to mid-market tech companies. Our biggest challenge is churn.
```

This saves you from re-explaining your situation every conversation.

**Remove frameworks that don't apply to your stage.** If you are pre-revenue, the RICE scoring section requires usage data you don't have. Delete that section — MoSCoW and ICE will carry the weight.

**Adjust the persona.** Change "senior product strategist" to "senior operations leader at a logistics company" to shift the framing and vocabulary.

**Create your own skills.** The format is simple:
1. A COPY FROM HERE / COPY TO HERE block with structured instructions
2. A framework reference section
3. An example conversation
4. When to use / not to use guidance

For the official Anthropic skill creation guide, see: [Skill Creator on GitHub](https://github.com/anthropics/skills/blob/main/skills/skill-creator/SKILL.md)

---

## References and Further Reading

These resources informed the design of CoworkSkills and are worth reading if you want to go deeper:

- [Claude Skills Overview](https://zapier.com/blog/claude-skills/) — Zapier's guide to using skills effectively
- [Awesome Claude Skills](https://github.com/ComposioHQ/awesome-claude-skills) — ComposioHQ's curated collection of community skills
- [The Complete Guide to Claude Skills](https://tylerfolkman.substack.com/p/the-complete-guide-to-claude-skills) — Tyler Folkman's deep dive on skill creation and progressive disclosure
- [Patience Is All You Need](https://medium.com/code-wild/patience-is-all-you-need-63b936d71eac) — Lessons on structured AI workflows and spec-driven development
- [Use Skills in Claude (Official)](https://support.claude.com/en/articles/12512180-use-skills-in-claude) — Anthropic's official guide to enabling and uploading skills
- [Building Skills for Claude (PDF)](https://resources.anthropic.com/hubfs/The-Complete-Guide-to-Building-Skill-for-Claude.pdf) — Anthropic's complete guide to skill design
- [Claude Guides: Code, Cowork, Skills, Workflows](https://karozieminski.substack.com/p/claude-guides-code-cowork-skills-workflows) — Karo Zieminski's overview of the Claude ecosystem

---

## About VibeCorp CoworkSkills

Built by VibeCorp for founders and strategists who use Claude.ai as a thinking partner. These skills represent accumulated frameworks from startup strategy, product management, organizational design, and go-to-market execution.

They are opinionated by design. The best frameworks make trade-offs explicit and force decisions. If a skill pushes back harder than you expected, that is intentional.

We are not affiliated with Anthropic. These are community-created skills, not officially supported products.

For questions, contributions, or feedback, open an issue in the [repository](https://github.com/The13thNode/VibeCorp_CoworkSkills/issues).

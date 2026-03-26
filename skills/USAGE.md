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
- Automation or agents
- A replacement for domain experts, lawyers, or therapists
- Permanent memory — each conversation starts fresh

---

## How to Use a Skill (Step by Step)

### Step 1: Go to claude.ai

Open a browser and navigate to claude.ai. Log in to your account. You will be on the main chat interface — a clean text input with no conversation history.

Start a new conversation. Do not paste a skill into an existing conversation that already has context; this can confuse the model about which instructions to follow.

### Step 2: Open the skill .md file

Find the skill file you want to use in the `skills/` folder of this repository. Open it in any text editor — Notepad, VS Code, TextEdit, or even GitHub's file viewer in a browser.

Skill files are plain text. They are readable as-is and do not require any special software.

### Step 3: Copy the paste-ready prompt

Every skill file contains a clearly marked block:

```
## COPY FROM HERE

[The prompt text you want to paste]

## COPY TO HERE
```

Select all the text between these two markers — from the first word after "COPY FROM HERE" to the last word before "COPY TO HERE." Copy it to your clipboard.

Do not include the marker lines themselves. Only copy the prompt content between them.

### Step 4: Paste into a new Claude.ai conversation

Click into the chat input box in Claude.ai. Paste the copied text. Do not add anything else yet — just paste the skill prompt on its own.

Hit Send (or press Enter, depending on your setup).

Claude will read the skill instructions and respond according to the framework — typically by asking you the Phase 1 diagnostic questions to understand your specific situation.

### Step 5: Start your conversation

Answer Claude's questions. The more specific and honest you are, the more useful the output will be.

The skills are designed to ask before they advise. Resist the urge to dump everything at once — let the skill's structure guide you. The questions are there to surface context you might not have thought to share.

From this point, have a normal conversation. You can ask follow-up questions, push back on recommendations, request different formats, or ask Claude to go deeper on any section.

---

## Tips for Best Results

**Use one skill per conversation.**

Each skill sets up a specific reasoning mode. Mixing two skill prompts in one conversation can create conflicting instructions. If you need to shift from roadmap planning to stakeholder management, open a new conversation and paste the relevant skill.

**Be specific about your situation.**

Generic input produces generic output. Instead of "I have a startup," say "I have a 12-person B2B SaaS company, we're at $300K ARR, and we're deciding whether to go upmarket to enterprise or double down on SMB." The skill frameworks are designed to handle real complexity.

**Challenge Claude's output.**

These skills are frameworks, not oracles. If a recommendation doesn't feel right, say so. "That doesn't fit our situation because..." is a valid and useful response. Claude will adjust.

**You can chain skills across conversations.**

If you are working through a strategic decision, you might:
1. Use `ceo-thinking-partner.md` to clarify your strategy
2. Then open a new conversation with `roadmap-planning.md` to sequence the work
3. Then open another with `stakeholder-management.md` to plan the alignment conversations

Each conversation is fresh, but you carry the thinking forward.

**The Strategic Challenger skill can be pasted mid-conversation.**

Unlike the other skills, `strategic-challenger.md` is designed to be used as an interrupt — you can paste it into an existing conversation when you want Claude to stop agreeing with you and start stress-testing your assumptions. You do not need a fresh conversation for this one.

**Paste the full skill block, including the framework structure.**

Some users try to summarize or shorten the skill prompt. Don't. The methodology sections shape how Claude reasons through your problem. The full prompt is the product.

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
| Validate a business model or new venture | `business-validation-flow.md` |
| Build and prioritize a product or company roadmap | `roadmap-planning.md` |
| Map stakeholders and get alignment before a key decision | `stakeholder-management.md` |
| Roll out a change and drive adoption across a team | `change-management.md` |

If you are not sure which skill to use, start with `ceo-thinking-partner.md`. It is the broadest skill and will help you figure out which specific framework you need next.

---

## Troubleshooting Common Issues

**Claude responded but didn't ask the Phase 1 questions.**

This can happen if Claude interpreted your paste as a document to summarize rather than instructions to follow. Add a line after pasting: "I have just pasted a skill prompt. Please begin by asking me the Phase 1 questions." This resets the context.

**The skill seems to have been forgotten partway through a long conversation.**

Claude.ai has a context window — very long conversations can cause earlier instructions to fade in influence. If you notice the quality of responses declining, either start a fresh conversation with the skill pasted again, or re-paste the skill prompt mid-conversation with a note: "Please continue using the framework from the skill prompt I shared earlier."

**Claude is giving me generic advice instead of using the frameworks.**

This usually means the Phase 1 questions were not answered with enough specificity. Go back and give more concrete details — specific numbers, specific names of competitors, specific team sizes, specific constraints. The frameworks activate when there is real context to work with.

**The output is too long and covering things I don't need.**

Tell Claude exactly what you need: "Focus only on the RICE scoring for items 3, 5, and 7. Skip the rest for now." Skills are designed to be used interactively, not consumed as a wall of output.

**I want a specific section without running the full skill.**

You can ask directly. For example: "Using the ADKAR model from the change management framework, help me diagnose why my team hasn't adopted the new CRM." You do not have to run the full Phase 1-7 structure every time. The frameworks are reference tools.

**The skill asks questions I can't answer yet.**

That is useful information. If you cannot answer "What is the one metric that matters for this phase?" it means you have not yet defined it. The skill is surfacing a gap, not blocking you. Say "I don't know yet" and Claude will help you figure it out.

---

## How to Customize Skills for Your Needs

CoworkSkills are plain text files. They are yours to edit.

**Add company context to the top of a skill:**

Before the skill prompt (but still within the COPY FROM HERE block), add a section like:

```
Context about my company: We are a 15-person product analytics SaaS, Series A, $2M ARR,
selling to mid-market tech companies. Our biggest challenge is churn. Our engineering team
is strong but our sales process is undefined. Keep this context in mind throughout.
```

This saves you from re-explaining your situation every conversation.

**Remove frameworks that are not relevant to your stage:**

If you are pre-revenue, the RICE scoring section in the Roadmap Planning skill requires usage data you do not have. Delete or comment out that section. The MoSCoW and ICE sections will carry the weight.

**Adjust the persona:**

If "senior product strategist" is not the right voice for your industry, change the first line. "You are a senior operations leader at a logistics company" will shift the framing and vocabulary Claude uses throughout the conversation.

**Save customized versions as new files:**

If you have made useful edits to a skill for your specific context, save it as a new file. For example: `roadmap-planning-enterprise.md` alongside the original `roadmap-planning.md`. Keep the original untouched so you can refer back to it.

**Create your own skills:**

The format is simple:
1. A COPY FROM HERE / COPY TO HERE block with structured instructions for Claude
2. A framework reference section for your own understanding
3. An example conversation
4. When to use / not to use guidance

If you build a skill that works well, consider contributing it back to the repository.

---

## About VibeCorp CoworkSkills

Built by VibeCorp for founders and strategists who use Claude.ai as a thinking partner. These skills represent accumulated frameworks from startup strategy, product management, organizational design, and go-to-market execution.

They are opinionated by design. The best frameworks make trade-offs explicit and force decisions. If a skill pushes back harder than you expected, that is intentional.

For questions, contributions, or feedback, open an issue in the repository.

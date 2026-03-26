# Frequently Asked Questions

Answers for everyone — whether you've never used AI before or you're already building with it.

---

## Beginner Questions

### What is Claude?

Claude is an AI assistant made by a company called [Anthropic](https://www.anthropic.com). You can talk to it by typing messages, like texting a very knowledgeable friend. It's free to start using.

**To try it:** Open your browser, go to [claude.ai](https://claude.ai), and create a free account.

---

### What is a "skill"? How is it different from just chatting?

When you chat with Claude normally, it gives general-purpose responses. It's helpful, but it doesn't follow a specific methodology.

A **skill** is a set of instructions you paste at the start of a conversation that tells Claude to think in a specific way. For example:
- The **Problem Validation** skill makes Claude ask you 5 specific questions and classify your evidence as strong, medium, weak, or dangerous
- The **CEO Thinking Partner** skill gives Claude 7 different thinking modes you can switch between

Without a skill, you get a smart generalist. With a skill, you get a structured specialist.

---

### How do I get started?

Here's exactly what to do:

1. **Open your browser** (Chrome, Edge, Safari, Firefox — any will work)
2. **Go to [claude.ai](https://claude.ai)** and sign up for a free account
3. **Go to our GitHub page:** [github.com/The13thNode/VibeCorp_CoworkSkills](https://github.com/The13thNode/VibeCorp_CoworkSkills)
4. **Click on the `skills/` folder**, then click on the skill file you want (start with `business-validation-flow.md` if you're not sure)
5. **Click the "Raw" button** near the top-right of the file — this shows you the plain text
6. **Find the text between `COPY FROM HERE` and `COPY TO HERE`**
7. **Select that text, copy it** (Ctrl+C on Windows, Cmd+C on Mac)
8. **Go back to claude.ai**, start a new conversation
9. **Paste** (Ctrl+V on Windows, Cmd+V on Mac) and **press Enter**
10. **Claude is now in that skill mode** — it will start by asking you questions. Answer them honestly.

For a more detailed walkthrough with tips, see our [Step-by-Step Guide](STEP_BY_STEP_GUIDE.md).

---

### Do I need to pay?

**No.** The free tier of Claude works fine. You can paste any skill into a free conversation.

**However**, if you want to use Claude Projects (which let you upload multiple skills and keep memory across conversations), you need a Pro or Team plan. This is optional — single-chat skills work perfectly on Free.

---

### What is GitHub and why is this repo on GitHub?

GitHub is a website where people store and share files — mostly code, but also documents like these skills. Think of it as a public folder on the internet.

You don't need a GitHub account. You don't need to download anything. You just need to:
1. Go to the page
2. Click on a file
3. Copy the text

That's it. GitHub is just where the files live.

---

### How do I copy a skill from GitHub?

1. Go to [github.com/The13thNode/VibeCorp_CoworkSkills](https://github.com/The13thNode/VibeCorp_CoworkSkills)
2. Click on the `skills/` folder
3. Click on the skill file you want (e.g., `problem-validation.md`)
4. Click the **"Raw"** button (top-right area of the file view) — this shows plain text without formatting
5. Find the text between `COPY FROM HERE` and `COPY TO HERE`
6. Select it (Ctrl+A selects everything, but you only need the part between the markers)
7. Copy (Ctrl+C)
8. Go to [claude.ai](https://claude.ai), start a new chat, and paste (Ctrl+V)

---

### What is a "Project" in Claude?

A Project is a workspace in Claude where you can:
- Upload files (like skills) to a shared Knowledge base
- Have multiple conversations that all share the same context
- Keep memory across sessions

It's like having a dedicated office for a specific topic, instead of having separate disconnected conversations.

**Projects require a Pro or Team plan.** If you're on the free tier, you can skip Projects entirely — single-chat skills work fine.

For official instructions: [Use Skills in Claude — Anthropic Support](https://support.claude.com/en/articles/12512180-use-skills-in-claude)

---

### What does "paste into Claude" actually mean?

Literally:
1. Open [claude.ai](https://claude.ai) in your browser
2. Click "New chat" (or the + button)
3. Click in the text input box at the bottom of the screen
4. Press Ctrl+V (Windows) or Cmd+V (Mac) to paste
5. Press Enter to send

That's it. Claude reads the pasted skill instructions and starts acting as that specialist.

---

### I pasted a skill and nothing happened — what went wrong?

A few common causes:

- **You pasted into an existing conversation.** Skills work best at the start of a new, blank conversation. Start a new chat and try again.
- **You copied the whole file instead of just the prompt.** Only copy the text between the `COPY FROM HERE` and `COPY TO HERE` markers — not the framework explanation or examples.
- **You didn't press Enter/Send.** After pasting, you need to send the message.
- **Claude interpreted it as a document to analyze.** Add a line after pasting: "I have just pasted a skill prompt. Please begin by asking me the Phase 1 questions."
- **The paste was cut off.** Some skills are long. Make sure you copied all the text between the markers. Try using the Raw view on GitHub for a cleaner copy.

---

### Can I use this on my phone?

Yes. Go to [claude.ai](https://claude.ai) in your mobile browser. The experience is the same — paste the skill prompt into a new conversation. The skills are just text, so they work on any device that can access Claude.

---

## Intermediate Questions

### How do I use multiple skills together?

There are three approaches:

1. **Chained chats (any tier):** Run one skill per chat. Copy the key decisions (not the whole conversation) to the next chat with a different skill. You are the bridge between skills.

2. **Projects (Pro/Team):** Upload 3-4 skill files to a Project's Knowledge base. Claude loads the relevant skill automatically based on your question. Memory persists across conversations.

3. **Orchestrator pattern:** Keep one "control room" chat that summarizes what you've decided in each skill session. Before starting a new skill, check the orchestrator for context.

See the [USAGE.md](../skills/USAGE.md) guide for detailed pros/cons of each approach.

---

### What's the difference between skills and agents?

| | Skills (CoworkSkills) | Agents (Claude Code) |
|---|---|---|
| **What they are** | Reasoning prompts you paste into chat | Autonomous workers that run in a terminal |
| **Where they run** | Claude.ai (web browser) | Claude Code (command line / IDE) |
| **What they can do** | Think, analyze, ask questions, give structured advice | Read files, write code, run commands, make API calls |
| **Who controls them** | You guide the conversation | They execute tasks semi-autonomously |
| **Setup required** | None — copy and paste | Install Claude Code, configure tools |

CoworkSkills are for **thinking**. Agents are for **doing**. If you're making strategic decisions, use skills. If you're writing code or automating tasks, use agents.

---

### Can I create my own skills?

Yes. Skills are just text files with a specific structure:

1. A paste-ready prompt between COPY FROM HERE / COPY TO HERE markers
2. A framework/methodology explanation
3. An example usage conversation
4. When to use / when NOT to use guidance

For the official Anthropic guide to creating skills, see: [Skill Creator on GitHub](https://github.com/anthropics/skills/blob/main/skills/skill-creator/SKILL.md)

If you build something useful, consider contributing it back — see [CONTRIBUTING.md](../CONTRIBUTING.md).

---

### How do I save my work across sessions?

Three options:

- **Claude Projects (Pro/Team):** Memory persists automatically across conversations within a project.
- **Copy key decisions manually:** At the end of each session, copy the important conclusions to a document (Google Doc, Notion, plain text file). Paste them as context at the start of your next session.
- **Ask Claude to summarize:** Before ending a session, ask "Summarize the key decisions and open questions from this conversation in a format I can paste into a future session."

---

## Important Disclaimers

### Can I use these for commercial projects?

These skills are for **personal use**. This is an open-source community contribution, not a commercial product. We take no responsibility for business outcomes, investment decisions, or strategic choices made using these skills. Use at your own discretion.

The repository is MIT-licensed, which means you can use, modify, and distribute the files. But the skills are thinking aids, not professional advice.

---

### Are you affiliated with Anthropic?

**No.** VibeCorp CoworkSkills is an independent, community-created project. We are not affiliated with, endorsed by, or officially supported by Anthropic. Claude is Anthropic's product; these skills are ours.

---

### Are these skills officially supported?

**No.** These are community-created prompts. They are not reviewed, tested, or maintained by Anthropic. They work because Claude is good at following structured instructions — not because they have special access or integration.

---

### Which skill should I start with?

- **New idea, no validation yet** → `business-validation-flow.md` (walks you through everything)
- **Existing project, need strategic clarity** → `ceo-thinking-partner.md` (7 thinking modes)
- **Preparing to raise money** → `investor-prep.md` (pitch structure and FAQ prep)
- **Something feels wrong but you can't name it** → `strategic-challenger.md` (forces you to confront assumptions)

---

### Do I need Claude Code for these?

**No.** These skills are designed for [Claude.ai](https://claude.ai) — the web chat interface. You don't need Claude Code, a terminal, or any developer tools. If you can open a browser and type, you can use these skills.

---

### How do I validate across different skill chats?

- **If using Projects with memory ON:** Ask Claude "Is this consistent with what we concluded in our previous conversation?" Claude can cross-check because it remembers.
- **If using separate chats:** You are the validator. Copy the key numbers and decisions from one chat and paste them into the next. Look for contradictions yourself.
- **If you want automatic validation:** Use `business-validation-flow.md` in a single chat — it has built-in gates that catch inconsistencies between stages.

---

### Can Claude remember my previous skill sessions?

- **Within Claude Projects:** Yes, if memory is enabled. Claude remembers previous conversations in the same project.
- **In regular chats:** No. Each conversation starts completely fresh. Claude has no memory of previous chats.
- **Workaround:** Copy a summary of key decisions and paste it as context at the start of your next session.

---

### What if Claude mixes up advice from different skills?

This happens when too many skills are loaded in a Project, or when a conversation gets very long. Fix it by:
1. Starting a fresh conversation
2. Pasting only the one skill you need
3. Keeping Projects limited to 3-4 skills maximum

---

### How many skills should I load into one Project?

**3-4 maximum.** Pick the ones relevant to your current phase:
- Early stage: problem-validation, market-sizing, business-validation-flow
- Growth stage: pricing-strategy, gtm-playbook, roadmap-planning
- Fundraising: investor-prep, market-sizing, ceo-thinking-partner
- Organizational: stakeholder-management, change-management, roadmap-planning

---

### Are these skills updated?

Yes — through community contributions. If you find an issue or want to improve a skill, you can submit a Pull Request. See [CONTRIBUTING.md](../CONTRIBUTING.md) for how.

---

### I have more questions

Open an issue on our [GitHub Issues page](https://github.com/The13thNode/VibeCorp_CoworkSkills/issues) and we'll respond.

# Step-by-Step Guide: Using VibeCorp CoworkSkills

This guide assumes you have never used Claude, GitHub, or AI skills before. Follow each step exactly.

---

## What You Need

- A computer, tablet, or phone
- An internet connection
- A web browser (Chrome, Edge, Safari, Firefox — any works)
- About 5 minutes for setup

You do **not** need:
- A GitHub account
- Any software to install
- A paid subscription (Free tier works)
- Any coding or technical knowledge

---

## Step 1: Go to Claude.ai and Create an Account

1. Open your browser
2. Go to **[claude.ai](https://claude.ai)**
3. Click **"Sign up"** (or "Get started")
4. Create an account using your email or Google account
5. Once you're in, you'll see a chat interface — a text box at the bottom where you type messages

This is where you'll use the skills. Leave this tab open.

---

## Step 2: Go to Our GitHub Repository

GitHub is a website where people store and share files. Think of it as a public folder on the internet. You're just going there to copy some text.

1. Open a **new browser tab**
2. Go to **[github.com/The13thNode/VibeCorp_CoworkSkills](https://github.com/The13thNode/VibeCorp_CoworkSkills)**
3. You'll see a list of files and folders

---

## Step 3: Pick a Skill

Click on the **`skills/`** folder. You'll see a list of skill files.

**Not sure which one to pick?** Here's a quick guide:

| If you want to... | Use this skill |
|---|---|
| Validate a new business idea from scratch | `business-validation-flow.md` |
| Think through a strategic decision | `ceo-thinking-partner.md` |
| Check if your problem is real | `problem-validation.md` |
| Estimate market size | `market-sizing.md` |
| Figure out pricing | `pricing-strategy.md` |
| Plan your go-to-market | `gtm-playbook.md` |
| Prepare for investors | `investor-prep.md` |
| Build a product roadmap | `roadmap-planning.md` |

**First time?** Start with **`business-validation-flow.md`** — it walks you through everything.

Click on the file name to open it.

---

## Step 4: Click the "Raw" Button

Once you've opened a skill file, you'll see the formatted text. To get a clean copy:

1. Look near the **top-right** of the file content area
2. Click the button that says **"Raw"**
3. This opens the file as plain text in a new page — no formatting, no menus, just the text

This makes it much easier to copy exactly what you need.

---

## Step 5: Find and Copy the Skill Prompt

In the raw text, look for these two markers:

```
<!-- COPY FROM HERE -->
```

and

```
<!-- COPY TO HERE -->
```

1. **Select all the text between these two markers** — start right after `COPY FROM HERE` and end right before `COPY TO HERE`
2. **Copy it:**
   - Windows: Press **Ctrl+C**
   - Mac: Press **Cmd+C**
   - Phone: Long-press to select, then tap "Copy"

**Important:** Only copy the text between the markers. Don't include the markers themselves, and don't copy the framework explanation or examples that come after.

---

## Step 6: Go Back to Claude.ai

Switch back to your Claude.ai browser tab (from Step 1).

Click **"New chat"** or the **+** button to start a fresh conversation. This is important — skills work best in a brand new conversation with no previous messages.

---

## Step 7: Paste and Send

1. Click in the **text input box** at the bottom of the screen
2. **Paste:**
   - Windows: Press **Ctrl+V**
   - Mac: Press **Cmd+V**
   - Phone: Long-press in the text box, then tap "Paste"
3. Press **Enter** (or tap the Send button)

---

## Step 8: Start Your Conversation

Claude will read the skill instructions and respond — usually by asking you a series of questions about your specific situation.

**Answer honestly and specifically.** The more detail you give, the better the output. For example:

- Instead of: *"I have a startup"*
- Say: *"I'm building a B2B SaaS tool that helps small accounting firms automate their client onboarding. We're pre-revenue with a 3-person team."*

From here, it's a normal conversation. You can:
- Answer Claude's questions
- Ask follow-up questions
- Push back on recommendations ("That doesn't fit because...")
- Ask Claude to go deeper on any section
- Ask for a summary at any time

---

## What If It Doesn't Work?

**Claude gave a generic response instead of using the skill:**
Type this: *"I have just pasted a skill prompt. Please begin by asking me the Phase 1 questions."*

**The text didn't paste correctly:**
Go back to the Raw view on GitHub and try copying again. Make sure you got all the text between the markers.

**Claude seems to forget the skill after a long conversation:**
This happens with very long chats. Start a new conversation, paste the skill again, and summarize where you left off.

**You're not sure what Claude is asking:**
Just say *"I don't understand that question, can you rephrase it?"* Claude will explain.

---

## What to Do Next

Once you've finished a skill session:

1. **Save your key decisions.** Copy the important conclusions to a document (Google Doc, Notes app, anywhere). You'll want these later.

2. **Try another skill.** If you validated your problem, maybe now size the market. Open a **new chat** and paste a different skill.

3. **Chain skills together.** The output of one skill feeds the next:
   - Problem Validation → Market Sizing → Pricing → Go-to-Market → Investor Prep

4. **Customize a skill.** If a skill is close to what you need but not quite right, copy the file and edit it. Change the persona, remove sections that don't apply, add your company context at the top.

5. **Come back anytime.** The skills are always available on GitHub. Bookmark the repo for easy access.

---

## Official Resources

For more on using skills and Claude:

- [Use Skills in Claude](https://support.claude.com/en/articles/12512180-use-skills-in-claude) — Anthropic's official guide to enabling and using skills
- [The Complete Guide to Building Skills for Claude (PDF)](https://resources.anthropic.com/hubfs/The-Complete-Guide-to-Building-Skill-for-Claude.pdf) — Anthropic's comprehensive skill design guide
- [Claude Guides: Code, Cowork, Skills, Workflows](https://karozieminski.substack.com/p/claude-guides-code-cowork-skills-workflows) — Community overview of the Claude ecosystem

---

## Need Help?

- Check the [FAQ](FAQ.md) for common questions
- Read the full [USAGE.md](../skills/USAGE.md) for advanced patterns
- Open an issue on [GitHub](https://github.com/The13thNode/VibeCorp_CoworkSkills/issues) if you're stuck

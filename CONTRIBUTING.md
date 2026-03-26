# Contributing to VibeCorp CoworkSkills

Welcome — and thank you for considering a contribution.

VibeCorp CoworkSkills is a collection of strategic thinking skills for [Claude.ai](https://claude.ai). Each skill is a self-contained, paste-ready prompt that activates a specific reasoning mode — no tools, no MCP servers, no file system access. Pure reasoning, ready to use.

If you have a framework, methodology, or structured thinking approach that belongs here, this guide explains how to contribute it.

---

## How to Contribute

1. **Fork the repository**
   Fork [pushhkarnagela/VibeCorp_CoworkSkills](https://github.com/pushhkarnagela/VibeCorp_CoworkSkills) to your GitHub account.

2. **Create a feature branch**
   Use a descriptive branch name:
   - New skill: `feat/skill-name` (e.g., `feat/competitive-analysis`)
   - Fix or improvement: `fix/description` (e.g., `fix/market-sizing-scoring`)

3. **Make your changes following REPO_STANDARDS.md**
   Read [REPO_STANDARDS.md](REPO_STANDARDS.md) before writing anything. It defines file naming conventions, commit formats, and what must never appear in this repo.

4. **Run the metadata scrub before committing**
   REPO_STANDARDS.md includes a set of `grep` commands under the **Metadata Scrub** section. Run all of them. If any return results, fix the issues before proceeding.

5. **Commit using conventional format**
   All commits must follow the `type: description` format:
   - `feat: add competitive-analysis skill`
   - `fix: remove hardcoded path from investor-prep`
   - `docs: update CONTRIBUTING with skill format details`
   - `security: strip personal identifiers from templates`

6. **Submit a Pull Request**
   Open a PR against `main`. Use the PR template — it will load automatically. Write a clear description of what you added or changed and why.

7. **Wait for maintainer review**
   A maintainer will review your PR, leave feedback if needed, and merge when it meets the standards. Please be patient and responsive to review comments.

---

## Skill File Format

Every skill file must follow this structure. Reviewers will check for all four components.

### 1. Paste-ready prompt

The prompt must be wrapped in copy markers so users can find it instantly:

```markdown
<!-- COPY FROM HERE -->

[Your prompt text here]

<!-- COPY TO HERE -->
```

The prompt must be self-contained and work by itself in a blank Claude.ai conversation.

### 2. Framework / methodology section

Explain the thinking behind the skill. What methodology does it embed? What scoring systems, decision gates, or structured outputs does it produce? This helps users understand what they are getting.

### 3. Example usage

Show a realistic conversation snippet that demonstrates the skill in action. Use realistic (but generic) inputs and outputs. No company names, no personal details.

### 4. When to use / when NOT to use

Be explicit about when this skill fits well and when a different skill (or no skill) is better. This prevents misuse and helps users pick the right tool.

---

## What NOT to Include

The following are never acceptable in any file in this repo. The metadata scrub will catch most of these — but you are responsible for checking before you commit.

- **Personal data** — names, email addresses, phone numbers, usernames, Telegram handles
- **API keys, tokens, or secrets** — of any kind, for any service
- **Local file paths** — no `C:\Users\...`, no `/home/...`, no `~/`
- **Project-specific or company-specific references** — no internal project names, Jira keys, Notion workspace IDs, Slack channel IDs, or Vercel deployment URLs
- **Tool or MCP dependencies** — skills must be pure reasoning. A skill that requires a browser tool, file system access, or an MCP server does not belong here.

---

## Code of Conduct

This project follows the [Contributor Covenant Code of Conduct](CODE_OF_CONDUCT.md). By participating, you agree to abide by it.

---

## Questions?

Open an issue on the [GitHub Issues page](https://github.com/pushhkarnagela/VibeCorp_CoworkSkills/issues). Label it `question` and describe what you need.

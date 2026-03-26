# Repo Standards — VibeCorp CoworkSkills

## Security — No Data Leakage

Before ANY commit, verify:

- [ ] No local file paths (C:\Users\<username>\, /home/, ~/)
- [ ] No IP addresses, hostnames, or machine names
- [ ] No API keys, tokens, or secrets
- [ ] No references to internal projects, internal Atlassian instances, or internal Vercel deployments
- [ ] No personal email addresses or Telegram IDs
- [ ] No Slack webhook URLs or channel IDs
- [ ] No Notion API keys or workspace IDs
- [ ] No Jira cloud IDs or project keys referencing real projects
- [ ] No git metadata pointing to other repos (check .git/config)
- [ ] No screenshots containing personal data
- [ ] No personal identifiers (usernames, machine names, VPN names)

## Git Config — Clean Identity

Run before first commit:
```bash
cd <your-repo-directory>
git config user.name "VibeCorp"
git config user.email "your-vibecorp-email@example.com"
```

This prevents your personal git identity leaking into commits.

## .gitignore — Must Include

```
# OS
.DS_Store
Thumbs.db
desktop.ini

# IDE
.vscode/
.idea/
*.swp
*.swo

# Secrets
.env
.env.*
.mcp.json
*.key
*.pem

# Claude Code local
.claude/settings.local.json
.claude/projects/

# Build artifacts
node_modules/
dist/
__pycache__/

# Temp
*.tmp
*.bak
*.log
```

## README Structure (GitHub best practices)

```markdown
# Project Name

> One-line description

![License](badge) ![Stars](badge)

## What is this?

[2-3 sentences for someone who has never coded]

## Quick Start

[3-5 steps maximum]

## Skills Included

[Table: skill name | what it does | when to use it]

## How to Use

[Step-by-step with examples]

## Examples

[Real examples of input → output]

## FAQ

[5-10 common questions]

## Contributing

[How to contribute]

## License

MIT

## Credits

[Attribution]
```

## File Naming

- All lowercase with hyphens: `market-sizing.md` not `MarketSizing.md`
- No spaces in filenames
- Skills use `.md` extension
- Config examples use `.example` suffix: `mcp.example.json`

## Commit Messages

Format: `type: description`
- `feat: add market-sizing skill`
- `docs: update README with usage examples`
- `fix: remove hardcoded path from skill template`
- `security: strip personal identifiers from templates`

## Metadata Scrub — Run Before Every Push

```bash
# Check for personal data leaks
# Check for personal identifiers
grep -ri "personal-username-here" . --include="*.md" --exclude-dir=.git
# Check for local paths
grep -ri "C:\\\\Users\|/home/\|/Users/" . --include="*.md" --exclude-dir=.git
# Check for service URLs
grep -ri "slack.com/services\|hooks.slack.com\|atlassian.net\|notion.so" . --include="*.md" --exclude-dir=.git
# Check for personal emails
grep -ri "@gmail.com\|@hotmail.com" . --include="*.md" --exclude-dir=.git
# Check for phone numbers
grep -ri "[0-9]\{10\}" . --include="*.md" --exclude-dir=.git
```

If ANY of these return results, fix before pushing.

## Commit Safety — Double Confirmation

Before any `git push`, the session must follow this sequence:

1. **Run metadata scrub** — execute all checks above and report results. Every check must return zero matches.
2. **Show `git diff --stat`** — display exactly what is being committed. Review the file list and change counts.
3. **ASK: "Ready to commit? Confirm with 'yes, commit'"** — wait for explicit confirmation before running `git commit`.
4. **After commit, show the commit hash** — display the hash so it can be verified.
5. **ASK: "Ready to push to GitHub? Confirm with 'yes, push'"** — wait for explicit confirmation before running `git push`.
6. **Only then run `git push`** — never before both confirmations are received.

**Rules:**
- Never combine `git commit` and `git push` in one command.
- Two separate confirmations are required — this is the equivalent of 2FA for deployments.
- No accidental pushes. If either confirmation is not given, stop and wait.
- If the metadata scrub returns any results, the commit is blocked until the issues are fixed.

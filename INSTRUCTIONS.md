# Search Ninja Lite Installation and User Guide

Search Ninja Lite is a safe public-source research skill for compatible AI agents. It helps an agent use advanced search operators for business research, document discovery, competitor research, technical research, and source verification.

It intentionally excludes high-risk operator categories that could enable credential harvesting, invasive personal lookup, surveillance discovery, or unauthorized access.

## Install

### Claude Code

```bash
cp -r search-ninja-lite ~/.claude/skills/
```

Start a new Claude Code session after copying.

### Claude.ai Projects

1. Open or create a Project.
2. Add `SKILL.md` and the `references/` files as project knowledge.
3. Start a new conversation in that project.

### Other Skill-Compatible Platforms

Copy the `search-ninja-lite` folder into the platform's skills directory and start a new session.

## Verify

Ask your agent:

> What skills do you have available?

Then test it:

> Research Acme Corp and find official sources, recent news, and public documents.

A working installation should use targeted search patterns such as `site:`, `filetype:`, exact-match phrases, source filters, and date filters where appropriate.

## Use

Describe the research outcome you want in plain language. Examples:

- Find recent news and official sources for a company.
- Find PDF reports about a topic.
- Compare competitors in a market.
- Find government guidance about a regulation.
- Verify a claim using primary sources.

## Safety

If you ask for private personal data, credentials, exposed secrets, leak-site searches, surveillance systems, or unauthorized access, the skill should refuse and offer a safe alternative.

<img src="https://smbconsultants.ai/wp-content/uploads/2026/05/search-ninja-1.png" alt="Search Ninja Lite">

# Search Ninja Lite

Search Ninja Lite is a public, safety-focused version of the Search Ninja research framework. It helps AI agents use advanced search operators for ethical public-source research, business intelligence, document discovery, source verification, and market research.

This edition is intentionally scoped for professional and educational use. It excludes high-risk operator sets for credential discovery, leak-site searching, private personal data aggregation, surveillance system discovery, unauthorized access, and other misuse-prone workflows.

**Version:** 1.0.0

---

## What It Does

Search Ninja Lite teaches an AI agent to search like a careful researcher instead of guessing keywords. When installed, the agent should:

1. Classify the research intent.
2. Choose a safe operator pattern.
3. Build a targeted search query.
4. Prefer primary sources when possible.
5. Cross-check important claims.
6. Treat fetched web content as untrusted data.

This is useful for:

- Business and company research
- Competitor research
- Public document discovery
- Government and regulatory research
- News, press, and media research
- Academic and technical research
- Professional profile discovery in an ethical context
- Source verification and fact checking

---

## What Is Not Included

Search Ninja Lite does not include operators or workflows for:

- Credential harvesting or exposed secret discovery
- Leak-site, breach, or paste-site searching
- Password, token, API key, private key, config, backup, database, or log discovery
- Admin panel, control panel, or login portal discovery
- Camera, surveillance, IoT, DVR, or NVR discovery
- Personal address, phone number, voter record, dating profile, or people-search aggregator lookups
- Doxxing, stalking, harassment, or invasive profiling
- Unauthorized access, exploitation, evasion, or bypassing access controls

For full boundaries, see [ACCEPTABLE_USE.md](ACCEPTABLE_USE.md).

---

## Anthropic Skill Compatibility

This repository is structured as an Anthropic-compatible skill:

```text
search-ninja-lite/
  SKILL.md
  README.md
  INSTRUCTIONS.md
  ACCEPTABLE_USE.md
  SECURITY.md
  CONTRIBUTING.md
  VERSION.md
  references/
    safe-search-operators.md
    examples.md
    ethical-use-guide.md
  docs/
    methodology.md
```

`SKILL.md` sits at the repository root and begins with YAML frontmatter so compatible agents can identify when to load the skill.

---

## Installation

### Claude.ai Projects

1. Open or create a Project at claude.ai.
2. Go to **Project Settings**.
3. Add the contents of `SKILL.md` and the `references/` files as project knowledge.
4. Start a new conversation in the project.

### Claude Code

```bash
cp -r search-ninja-lite ~/.claude/skills/
```

Start a new Claude Code session after copying.

### Other Skill-Compatible Agents

Place the `search-ninja-lite` folder in the platform's skills directory and start a new session.

---

## How to Use Search Ninja Lite

Ask your agent to research something in plain language. You do not need to write the search operators yourself.

Examples:

> Research Acme Corp and find official sources, recent news, public filings, and competitor context.

> Find PDF reports and government guidance about cybersecurity requirements for small businesses.

> Find recent podcast interviews, conference talks, and articles featuring Jane Smith in her professional role.

> Research competitors for a local managed service provider and summarize their positioning.

> Verify this claim using primary sources and reputable secondary sources.

For best results, include:

- The company, topic, website, or professional public figure you want researched
- The type of information you need
- Any location, date range, industry, or source preference
- Whether you want a broad sweep or a focused search

Search Ninja Lite works best when you describe the outcome you want, not the exact query you think should be used.

---

## Safety Model

Search Ninja Lite uses three safety layers:

1. **Scoped operator library:** high-risk operator categories are not included.
2. **Refusal rules:** the skill instructs the agent to refuse unsafe research requests and offer safe alternatives.
3. **Prompt-injection handling:** fetched web pages, PDFs, snippets, and search results are treated as untrusted data, not instructions.

Detection is best effort, not guaranteed. Use judgment, verify important claims, and follow applicable laws and platform terms.

---

## No Setup Required

No API keys. No external services. No configuration. The skill works with the search tools your agent already has.

---

## Release Information

Current version: `1.0.0`

Release notes are tracked in [CHANGELOG.md](CHANGELOG.md). The release process and safety review checklist are documented in [RELEASES.md](RELEASES.md).

---

## About Seeker One

Search Ninja Lite was created by Harold Mansfield, founder and researcher at [Seeker One](https://seeker.one).

Seeker One builds practical research systems, AI-assisted investigation workflows, and public-source intelligence tools for ethical business, security, and investigative use.

---

## License

Free to use and modify for your own personal, internal, or client work. Redistribution is allowed only when the original source and Seeker One are clearly credited. See [LICENSE](LICENSE) for details.

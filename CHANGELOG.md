# Changelog

All notable changes to Search Ninja Lite are documented here.

This project uses simple semantic versioning:

- Major version: breaking changes to the skill structure, safety model, or operator format
- Minor version: new safe operator categories, examples, docs, or compatibility improvements
- Patch version: wording fixes, typo fixes, safety clarifications, and small documentation updates

## [1.0.0] Initial public release

Release date: 2026-10-04

### Added

- Anthropic-compatible `SKILL.md` with root-level YAML frontmatter.
- Safe Google Dork operator library in `references/safe-search-operators.md`.
- Example requests and query patterns in `references/examples.md`.
- Ethical use guidance in `references/ethical-use-guide.md`.
- Public methodology notes in `docs/methodology.md`.
- Acceptable use policy.
- Security and abuse reporting guidance.
- Contribution guidelines.
- Custom attribution license for use, modification, and redistribution with credit.

### Excluded by design

- Credential harvesting and exposed secret discovery patterns.
- Leak-site, breach, and paste-site search patterns.
- Admin panel, login portal, and exposed system discovery patterns.
- Camera, surveillance, IoT, DVR, and NVR discovery patterns.
- Address, phone number, voter record, dating profile, and people-search aggregator lookup patterns.
- Doxxing, stalking, harassment, invasive profiling, exploitation, evasion, and unauthorized access workflows.

### Notes

Search Ninja Lite is the public, safety-focused edition of the Search Ninja Google Dorks skill. It is intended for ethical public-source research, business research, document discovery, and market research.

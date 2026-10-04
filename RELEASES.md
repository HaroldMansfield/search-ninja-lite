# Release Process

This file documents how Search Ninja Lite releases are tracked.

## Current release

Current version: `1.0.0`

Release notes are maintained in [CHANGELOG.md](CHANGELOG.md). GitHub releases should use the same notes so visitors can see what changed without reading commit history.

## Versioning

Search Ninja Lite uses simple semantic versioning.

### Major versions

Use a major version when the skill changes in a way that may break existing usage, such as:

- Renaming core files
- Changing the expected skill folder structure
- Reworking the operator reference format
- Changing the safety model in a way users need to review

### Minor versions

Use a minor version when adding safe functionality, such as:

- New safe operator categories
- New example sets
- New compatibility notes
- New documentation sections
- Expanded ethical-use guidance

### Patch versions

Use a patch version for maintenance updates, such as:

- Typo fixes
- Wording improvements
- Broken link fixes
- Safety clarifications
- Formatting cleanup

## Release checklist

Before publishing a release:

1. Update `VERSION.md`.
2. Update `CHANGELOG.md`.
3. Confirm `SKILL.md` still starts with valid YAML frontmatter.
4. Confirm the public operator reference does not include excluded high-risk categories.
5. Confirm no secrets, credentials, private data, or sensitive targets are included.
6. Confirm there are no em dashes or en dashes in public Markdown files.
7. Commit the changes.
8. Tag the release, for example `v1.0.0`.
9. Create a GitHub release using the matching changelog notes.

## Safety review checklist

Before each release, confirm the project still excludes:

- Credentials, secrets, passwords, tokens, private keys, and config discovery
- Leak, breach, and paste-site searching
- Admin panels, login portals, exposed systems, cameras, surveillance, and IoT discovery
- Personal address, phone, voter, dating, and people-search aggregator lookup patterns
- Doxxing, stalking, harassment, invasive profiling, exploitation, evasion, and unauthorized access workflows

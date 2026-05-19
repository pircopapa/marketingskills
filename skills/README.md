# Marketing Skills Directory

This directory contains all available marketing skills for the Claude AI assistant plugin.

## Structure

Each skill is organized in its own subdirectory with the following structure:

```
skills/
  └── skill-name/
        ├── skill.json       # Skill metadata and configuration
        ├── prompt.md        # The core prompt/instructions for the skill
        └── examples/        # (optional) Example inputs and outputs
              ├── input.md
              └── output.md
```

## Skill Categories

- **copywriting** — Ad copy, landing pages, email campaigns
- **seo** — Keyword research, meta descriptions, content optimization
- **social-media** — Platform-specific content strategies
- **analytics** — Data interpretation, reporting, insights
- **branding** — Brand voice, positioning, messaging frameworks
- **content-strategy** — Editorial planning, content calendars
- **email-marketing** — Subject lines, sequences, segmentation
- **paid-advertising** — PPC, display, retargeting strategies

## Adding a New Skill

1. Create a new directory under `skills/` using kebab-case naming
2. Add a `skill.json` with the required metadata (see schema below)
3. Write your `prompt.md` with clear, actionable instructions
4. Submit a PR using the `new-skill` pull request template

## Skill JSON Schema

```json
{
  "id": "unique-skill-id",
  "name": "Human Readable Name",
  "version": "1.0.0",
  "category": "copywriting",
  "description": "Brief description of what this skill does",
  "tags": ["tag1", "tag2"],
  "author": "github-username",
  "inputs": [
    {
      "name": "inputName",
      "type": "string",
      "required": true,
      "description": "What this input represents"
    }
  ]
}
```

> **Personal note:** I'm mainly using this fork to experiment with the `email-marketing` and `copywriting` categories for a side project. Most of the other categories are upstream concerns — I'll try to keep this in sync with coreyhaines31/marketingskills periodically but no guarantees.

## Contributing

See the root [CONTRIBUTING.md](../CONTRIBUTING.md) for general guidelines.
For skill-specific requests, use the [skill request issue template](../.github/ISSUE_TEMPLATE/skill-request.yml).

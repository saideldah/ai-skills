# ai-skills

A collection of Claude Code skills — structured workflow files that guide Claude through specific development tasks.

## What are skills?

Skills are markdown files that define step-by-step processes for Claude Code to follow. When invoked, they replace ad-hoc behavior with a disciplined, opinionated workflow.

## Skills

| Skill | Trigger |
|-------|---------|
| [generate-prd](generate-prd/SKILL.md) | Writing a PRD, planning a feature, or documenting requirements before implementation |
| [idea-stress-test](idea-stress-test/SKILL.md) | Stress-testing a plan or design ("grill me") |

## Usage

Skills are loaded by the [Superpowers](https://github.com/superpowers) harness for Claude Code. Once installed, Claude automatically invokes the relevant skill based on your request.

To invoke manually, use the `Skill` tool in Claude Code:

```
/skill generate-prd
/skill idea-stress-test
```

## Adding a Skill

1. Create a new directory: `<skill-name>/`
2. Add a `SKILL.md` with frontmatter and instructions:

```markdown
---
name: skill-name
description: When Claude should trigger this skill
---

# Skill Title

...instructions...
```

See [CLAUDE.md](CLAUDE.md) for authoring guidelines.

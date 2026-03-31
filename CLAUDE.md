# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What This Repo Is

A collection of Claude Code skills — markdown files that define structured workflows for AI-assisted development tasks. Skills are invoked via the `Skill` tool in Claude Code and guide behavior through a documented process.

## Structure

Each skill lives in its own directory with a `SKILL.md` file:

```
<skill-name>/
  SKILL.md    # Frontmatter (name, description) + skill instructions
```

The frontmatter fields are:
- `name`: identifier used when invoking the skill
- `description`: shown to Claude to determine when to trigger the skill

## Authoring Skills

Skills follow a consistent format:

```markdown
---
name: skill-name
description: Trigger condition — when Claude should invoke this skill
---

# Skill Title

## Overview / Rules / Process
...
```

Key authoring principles:
- **Be opinionated.** Skills are rigid workflows, not suggestions. Tell Claude exactly what to do and what NOT to do.
- **Use flowcharts** (dot/digraph syntax) for multi-step processes — Claude renders them as decision trees.
- **Include anti-patterns** — a table of common shortcuts and what to do instead is highly effective.
- **Include red flags** — explicit "stop if you're thinking X" statements prevent rationalization.
- Skills can be "rigid" (follow exactly, e.g. TDD, debugging) or "flexible" (adapt principles to context). Label which one.

## Deploying Skills

Skills are loaded by the Superpowers harness. The `description` field must be specific enough that Claude reliably triggers the skill for the right tasks and not for unrelated ones.

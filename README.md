# Harness Upgrade Guide

This repository is a docs-only playbook for making existing codebases more legible for humans and AI agents without changing product behavior during the initial harness pass.

It is intended for internal engineering teams that want a safer, repeatable way to upgrade older repositories so they are easier to review, hand off, and work on with tools like Codex or other agentic IDEs.

## What This Is

- a two-pass workflow for upgrading an existing repo's harness layer
- a set of prompt templates for Pass 1 and Pass 2
- a lightweight team instruction for pilot adoption
- review and pilot checklists

## What This Is Not

- not a product redesign framework
- not a mandate to copy OpenAI's operating model
- not a license to refactor working code during the initial harness effort
- not a replacement for human approval on scope, merge, or deploy

## Recommended Usage

1. Read [TEAM-INSTRUCTION.md](TEAM-INSTRUCTION.md).
2. Read [references.md](references.md).
3. Use [prompts/pass-1.md](prompts/pass-1.md) first.
4. Collect owner answers.
5. Use [prompts/owner-answer-handoff.md](prompts/owner-answer-handoff.md).
6. Use [prompts/pass-2.md](prompts/pass-2.md).
7. Review the outputs with [templates/review-checklist.md](templates/review-checklist.md).

## Recommended Pilot Scope

- start with legacy or under-documented repositories
- choose one repo owner and one reviewer
- keep the initial pass docs-only
- avoid repos with active production incidents or major migrations in flight

## Approved Model Guidance

- OpenAI: `gpt-5.4` with `high` reasoning
- Anthropic: `Claude Opus 4.1` if available, otherwise `Claude Opus 4`

The goal is consistency and planning quality, not lowest latency.

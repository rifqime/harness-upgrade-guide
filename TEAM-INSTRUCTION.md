# Team Instruction

## Summary

Use this workflow to make existing repositories easier for humans and AI agents to understand and modify safely.

This is a harness upgrade for existing repos. It is not a product rewrite and it is not an attempt to copy another company's full engineering model.

## Why We Are Doing This

- too much repo truth still lives in chat, memory, and unwritten assumptions
- older repos are harder to hand off across engineers, freelancers, and AI agents
- review quality drops when architecture, deploy flow, and source-of-truth rules are implicit
- a good harness makes issue -> spec -> PR work more reliable

## Required Reading

Read the OpenAI Harness Engineering article first:

- https://openai.com/index/harness-engineering/

Read it as a reference for agent-legible repos, not as a blueprint to copy wholesale.

## Tooling Guidance

Approved agent environments:

- Codex preferred
- Antigravity allowed
- other agentic IDEs allowed if they can follow repo instructions and operate directly on the repository

Approved models for this workflow:

- OpenAI: `gpt-5.4` with `high` reasoning
- Anthropic: `Claude Opus 4.1` if available, otherwise `Claude Opus 4`

Do not switch to weaker substitute models for the initial harness pass unless the repo owner approves it.

## Team Policy

- start with a recommended pilot, not an org-wide mandate
- use this first on legacy or under-documented repos
- keep human approval for scope, merge, and deploy
- document reality as it exists today
- do not invent policies the owner has not approved

## Two-Pass Workflow

### Pass 1

Discovery and clarification only.

Allowed:

- read the repo structure, manifests, configs, docs, CI, deploy files, and contributor instructions
- inspect current docs and workflow assets
- identify missing, stale, or contradictory repo guidance
- ask only the questions needed to build an accurate harness

Not allowed:

- application logic changes
- refactoring working code
- runtime, deploy, or environment changes
- creating harness files before clarification

### Pass 2

Docs and lightweight workflow scaffolding only.

Allowed:

- `README`
- `AGENTS.md`
- repo map / reading order
- architecture or system overview docs
- deploy/runbook docs
- env/setup docs
- issue/spec/ADR guidance
- PR and review checklists
- lightweight docs/workflow validation

Not allowed:

- product behavior changes
- backend contract changes
- deploy behavior changes
- broad dependency churn unrelated to harnessing

## Definition Of Done

The initial harness is good enough when:

- a new contributor can understand what the system is and what is live
- source-of-truth and deploy rules are explicit
- architecture boundaries are explicit
- safe versus sensitive areas are called out
- ownership of issue scope, PR merge, and production deploy is documented
- an AI agent can draft a directionally correct issue, spec, or PR without guessing the wrong architecture

## Default Deliverables

- source-of-truth overview
- contributor workflow guidance
- architecture boundaries
- deploy and staging flow
- AI contribution boundaries
- lightweight review scaffolding

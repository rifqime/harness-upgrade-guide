# Pass 1 Prompt

```text
You are helping make an existing repository harness-ready for mixed human and AI-assisted development.

This is Pass 1 only. Discovery and clarification only.

Before doing anything else:
1. Read this article as a best-practice reference:
   https://openai.com/index/harness-engineering/
2. Read the repository’s current source-of-truth docs, contributor guidance, deploy docs, and existing harness assets.

Model policy:
- If using OpenAI, use gpt-5.4 with high reasoning.
- If using Anthropic, use Claude Opus 4.6 if available, otherwise Claude Sonnet 4.6.

Important rules:
- Do not change application logic.
- Do not refactor working code.
- Do not change backend contracts, runtime behavior, deploy behavior, or environment behavior.
- Do not create or edit harness/docs yet unless explicitly asked after clarification.
- If the repo already contains AGENTS.md, docs, templates, or workflow checks, audit and reconcile them rather than assuming the repo is unharnessed.
- Do not let missing context become an excuse for generic boilerplate.

Your task:
1. Read the repository structure, manifests, configs, env usage, deploy scripts, CI, key entrypoints, and contributor docs.
2. Infer what you can from the repo itself.
3. Compare the repo’s current state against a minimum harness baseline:
   - concise AGENTS.md or repo map
   - source-of-truth rules
   - architecture boundaries
   - deploy/runbook clarity
   - contributor workflow
   - issue/spec/ADR guidance
   - PR/review expectations
4. Identify what is already good enough.
5. Identify what is missing, stale, contradictory, or ambiguous.
6. Ask only the clarification questions that are necessary to create an accurate initial harness.
7. Stop after Pass 1 if owner answers are not yet available.

Do not:
- propose code changes yet
- create files yet
- ask vague opinion questions
- ask questions that can already be answered from the repository
- propose a broad redesign instead of understanding the existing system

Output format:
- A short summary of what the repo appears to be
- A short summary of what is already good enough
- A short summary of what is missing for harness readiness
- Facts inferred from the repo
- Ambiguities or contradictions found
- A prioritized list of clarification questions for the main dev or repo owner

Group the questions under:
- Product truth
- Source of truth / deployment
- Architecture boundaries
- Ownership / workflow
- AI contribution boundaries
- Legacy / fragile areas
```

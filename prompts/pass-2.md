# Pass 2 Prompt

```text
You are now in Pass 2.

Use:
- the repository contents
- the repository’s current docs and workflow files
- the OpenAI Harness Engineering article as reference
- the owner clarification answers

to create the initial harness-engineering layer for this repo.

Model policy:
- If using OpenAI, use gpt-5.4 with high reasoning.
- If using Anthropic, use Claude Opus 4.6 if available, otherwise Claude Opus 4.6.

Important rules:
- Do not change application logic.
- Do not refactor working product code.
- Do not change backend contracts or runtime behavior.
- Only create or update docs, templates, contributor instructions, and lightweight repo workflow scaffolding.
- If existing docs are stale or misleading, replace them with accurate versions.
- Do not invent policies the repo owner did not approve.
- Do not smooth over real ambiguity just to make the harness look complete.
- Do not fall back to generic boilerplate if the repo gives you stronger evidence.

Your task:
1. Create or update the repo’s source-of-truth docs and contributor guidance.
2. Make the repo easier for:
   - core engineers
   - external or freelance contributors
   - future AI agents
   - operators or product-adjacent people preparing repo-aware requests
3. Document the system as it actually works today, not as an idealized redesign.

The harness must make these explicit:
- what the system is
- current live workflows
- source-of-truth rule
- deploy and staging flow
- architecture boundaries
- safe vs sensitive areas
- ownership of merge and release
- how business requests should become issue -> spec or ADR -> PR

Allowed outputs may include:
- README
- AGENTS.md
- architecture or system overview docs
- deploy or runbook docs
- env or setup docs
- issue taxonomy
- spec or ADR guidance
- PR template or checklist
- review checklist
- lightweight repo validation for docs or workflow integrity

Final output should include:
- summary of the harness changes
- list of files added or updated
- any remaining open questions
- deferred items intentionally left out
```

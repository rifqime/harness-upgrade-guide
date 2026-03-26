# Pilot Checklist

Use this before starting the first harness upgrade on a real repository.

## Repo Selection

- the repo is legacy, under-documented, or hard to onboard into
- the repo is stable enough to observe current behavior
- the repo is not in the middle of an incident or a major migration
- the repo owner agrees that the initial pass is docs-only

## People

- one clear repo owner is available to answer Pass 1 questions
- one reviewer is assigned to review the harness outputs
- merge and deploy authority are known before Pass 2 begins

## Operating Constraints

- the team agrees that Pass 1 is discovery only
- the team agrees that Pass 2 is docs and workflow scaffolding only
- no product behavior change is allowed in the initial harness effort
- unknown policy should be marked as pending, not guessed

## Success Criteria

- owner questions are short and high-value
- the resulting docs reduce hidden context
- contributors can find source-of-truth and deploy rules
- AI agents can draft issues, specs, and PRs with fewer bad assumptions

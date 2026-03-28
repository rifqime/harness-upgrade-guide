# References

## Primary Reference

- OpenAI, "Harness engineering: leveraging Codex in an agent-first world"
  - https://openai.com/index/harness-engineering/

Use this article as best-practice reference material for agent-legible repositories. Do not treat it as a requirement to copy OpenAI's full operating model.

This guide is deliberately opinionated in how it applies that reference. The goal is not to be universally neutral. The goal is to help a strong model produce a better first-pass harness with less generic boilerplate and fewer architecture mistakes.

## Model Guidance References

- OpenAI code generation guide
  - https://developers.openai.com/api/docs/guides/code-generation
- OpenAI model docs
  - https://developers.openai.com/api/docs/models
- Anthropic model docs
  - https://docs.anthropic.com/en/docs/about-claude/models

## Working Principle

The goal of this guide is simple:

- repository knowledge should be findable
- boundaries should be explicit
- workflow should be legible
- humans should retain review and release control
- strong models should be given enough repo truth to stop guessing

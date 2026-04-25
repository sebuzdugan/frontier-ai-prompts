# GitHub Prompt Resources

Last reviewed: 2026-04-25

This is a curated list of public GitHub resources worth studying. The goal is not to copy them wholesale, but to learn patterns and point users to deeper libraries.

## Prompt Libraries

### f/prompts.chat

Link: https://github.com/f/prompts.chat

Why it matters: One of the largest and longest-running open-source prompt libraries. Useful for browsing lots of practical "act as..." and role-based prompts.

Use it for:

- Discovering prompt categories
- Finding quick role/task templates
- Understanding what people commonly ask AI to do

Watch out for:

- Many prompts are from earlier chatbot eras and may be over-constrained for modern reasoning models.
- Review license and attribution before reusing content.

### ai-boost/awesome-prompts

Link: https://github.com/ai-boost/awesome-prompts

Why it matters: Curated prompts, prompt engineering resources, frameworks, and papers with an engineering bias.

Use it for:

- Prompt engineering tools
- Coding and DevOps prompt ideas
- Learning about prompt-as-engineering workflows

### promptslab/Awesome-Prompt-Engineering

Link: https://github.com/promptslab/Awesome-Prompt-Engineering

Why it matters: A broad hand-curated index covering prompt engineering, context engineering, papers, tools, APIs, benchmarks, and courses.

Use it for:

- Learning paths
- Research papers
- Prompt engineering tooling
- Broader context engineering resources

### anthropics/prompt-eng-interactive-tutorial

Link: https://github.com/anthropics/prompt-eng-interactive-tutorial

Why it matters: Anthropic's hands-on prompt engineering tutorial. It covers clarity, roles, examples, hallucination reduction, separating data from instructions, and complex prompts.

Use it for:

- Learning prompt fundamentals
- Claude-specific prompting habits
- Exercises for improving prompts

### dair-ai/Prompt-Engineering-Guide

Link: https://github.com/dair-ai/Prompt-Engineering-Guide

Why it matters: A comprehensive educational guide to prompting concepts, techniques, papers, and examples.

Use it for:

- Foundational prompt engineering concepts
- Technique names and definitions
- Research-oriented learning

## Provider Docs

### OpenAI Prompting

Link: https://platform.openai.com/docs/guides/prompting

Useful notes:

- OpenAI recommends clear role/tone guidance, structured examples, prompt versioning, and evals.
- GPT-5 family guidance emphasizes precise instructions for GPT-style models and high-level goals for reasoning models.

### OpenAI GPT-5.5

Link: https://openai.com/index/introducing-gpt-5-5/

Useful notes:

- GPT-5.5 is positioned for agentic coding, research, data analysis, documents, spreadsheets, computer use, and long multi-step work.
- Prompt patterns should include goals, tools, verification, and delivery criteria.

### Anthropic Claude Opus 4.7

Link: https://www.anthropic.com/news/claude-opus-4-7

Useful notes:

- Opus 4.7 is positioned for difficult coding, long-running tasks, higher-resolution vision, agents, documents, and professional work.
- Claude prompts often benefit from clearly separated sections and explicit success criteria.

### Google Gemini

Link: https://ai.google.dev/gemini-api/docs/models/gemini

Useful notes:

- Gemini 3 Pro supports large multimodal inputs.
- Gemini prompt design favors clear instructions, enough context, and structured outputs.

## How This Repo Uses These Sources

- We link to major libraries instead of copying them.
- We rewrite prompts around modern model behavior: goals, context, constraints, output formats, and verification.
- We include practical prompts for everyday users rather than deep academic examples only.
- We avoid unsafe prompts that ask models to impersonate doctors, lawyers, or financial advisors without caveats.

# Frontier Model Notes

Last reviewed: 2026-04-25

This file summarizes current prompting guidance for the major frontier model families. Model names and availability change quickly, so verify provider docs before making production decisions.

## GPT-5.5

OpenAI announced GPT-5.5 on 2026-04-23 and updated availability notes on 2026-04-24. OpenAI describes it as a model for complex real-world work: coding, online research, data analysis, documents, spreadsheets, software operation, and multi-tool task completion.

Prompting implications:

- Give the model the real goal, not only a narrow instruction.
- Include constraints, context, and success criteria.
- For multi-step work, ask it to plan, act, check work, and report residual risk.
- For coding, include the error, relevant files, expected behavior, and test command.
- For production use, prefer evals and model snapshots when available.

Good fit:

- Agentic coding
- Data analysis
- Research synthesis
- Document/spreadsheet creation
- Tool-heavy workflows

Source: [Introducing GPT-5.5](https://openai.com/index/introducing-gpt-5-5/), [GPT-5.5 System Card](https://openai.com/index/gpt-5-5-system-card/)

## Claude Opus 4.7

Anthropic announced Claude Opus 4.7 on 2026-04-16. Anthropic positions it for advanced software engineering, long-running tasks, agents, professional documents/slides, and high-resolution vision work.

Prompting implications:

- Claude responds well to clear sections and explicit success criteria.
- XML-style wrappers can help separate instructions from data.
- Give room for judgment on hard tasks instead of over-specifying every micro-step.
- Ask it to verify outputs and call out uncertainty.
- For long documents or codebases, define what to extract, compare, or decide.

Good fit:

- Hard code review and implementation
- Complex writing and editing
- Multi-session/agentic work
- Slide and document drafting
- Visual reasoning over dense screenshots or images

Source: [Introducing Claude Opus 4.7](https://www.anthropic.com/news/claude-opus-4-7), [Claude Opus 4.7 page](https://www.anthropic.com/claude/opus)

## Gemini 3.1 Pro / Gemini 3 Pro

Google's public Gemini API docs list Gemini 3 Pro Preview with long multimodal context, and Google's 2026 Gemini 3.1 Pro announcement describes stronger reasoning for complex tasks. Gemini models are especially useful when the input is large or multimodal.

Prompting implications:

- Give the model the full context when possible: PDFs, images, audio, video, notes, and tables.
- Ask for structured extraction before asking for conclusions.
- Use tables for comparisons and evidence tracking.
- Tell it whether to prioritize completeness, brevity, or confidence.
- When grounding/search is enabled, require source links for current claims.

Good fit:

- Large PDF or document synthesis
- Multimodal analysis
- Research comparison
- Long-context extraction
- Visual and educational explanations

Source: [Gemini models](https://ai.google.dev/gemini-api/docs/models/gemini), [Gemini 3.1 Pro announcement](https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-3-1-pro/)

## Fast / Smaller Models

Smaller and faster models remain valuable for high-volume work.

Prompting implications:

- Be more explicit.
- Use examples.
- Keep tasks narrow.
- Specify exact output format.
- Avoid asking for broad judgment without context.

Good fit:

- Rewrites
- Summaries
- Classification
- Extraction
- Formatting
- Draft variants

## Universal Rules

- Put important constraints near the top.
- Separate instructions from data.
- Use examples when exact style matters.
- Ask for sources when facts are current or contested.
- Ask for a self-check when quality matters.
- For sensitive domains, ask for caveats and recommend professional review.
- For repeatable workflows, turn the prompt into a template and version it.

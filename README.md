# Frontier Prompt Playbook

A clean, practical prompt library for people who use AI every day: freelancers, software builders, creators, operators, analysts, students, founders, and online professionals.

The current featured workflow is **landing freelance clients with AI**: choosing a niche, packaging a service offer, creating proof assets, building prospect lists, writing specific outreach, preparing calls, sending proposals, and following up without sounding automated.

This repo is intentionally model-aware. It is updated around the 2026 frontier model generation: GPT-5.5, Claude Opus 4.7, Gemini 3.1 Pro, and other long-context reasoning models. The prompts are written to work across ChatGPT, Claude, Gemini, Perplexity, Copilot, Cursor, Claude Code, Codex, and similar tools.

## Start Here

1. Pick the folder closest to your task.
2. Copy a prompt.
3. Replace the bracketed fields like `[goal]`, `[audience]`, and `[constraints]`.
4. Add your real context: files, notes, screenshots, data, examples, links, or rough drafts.
5. Ask the model to check assumptions and produce a final answer in the format you need.

## Prompt Packs

| Pack | Best for |
| --- | --- |
| [Freelance Clients](prompts/freelance-clients/README.md) | Niche selection, service offers, proof assets, lead lists, outreach, proposals, follow-up |
| [Daily Work](prompts/daily-work/README.md) | Email, planning, meetings, decisions, personal productivity |
| [Coding](prompts/coding/README.md) | Code review, debugging, architecture, tests, refactors |
| [Content](prompts/content/README.md) | Posts, newsletters, scripts, editing, repurposing |
| [Business](prompts/business/README.md) | Strategy, offers, customer research, sales, operations |
| [Research](prompts/research/README.md) | Web research, synthesis, source evaluation, briefs |
| [Learning](prompts/learning/README.md) | Study plans, explanations, tutoring, skill acquisition |
| [Images](prompts/images/README.md) | Image generation, product visuals, thumbnails, style guides |
| [Agents](prompts/agents/README.md) | Multi-step work, tool use, autonomous execution, QA loops |

## Latest Model Notes

Use the strongest models for vague, multi-step, high-context, or high-stakes work. Use faster/cheaper models for narrow transformations.

| Model family | Use it for | Prompting style |
| --- | --- | --- |
| GPT-5.5 / GPT-5.5 Pro | Agentic coding, research, data analysis, documents, spreadsheets, computer/tool use | Give the real goal, context, constraints, and desired deliverable. Let it plan, use tools, verify, and report uncertainty. |
| Claude Opus 4.7 | Hard coding tasks, long-running agents, high-quality writing, slides/docs, vision-heavy work | Give a clear objective and allow room for judgment. Claude is strong with XML-style sections and explicit success criteria. |
| Gemini 3.1 Pro / Gemini 3 Pro | Long multimodal context, large PDFs, video/audio/image reasoning, broad synthesis | Provide lots of raw material and ask for structured extraction, comparison, and synthesis. |
| Fast models | Summaries, rewrites, classification, extraction, first drafts | Use precise instructions, examples, and strict output formats. |

See [models/frontier-model-notes.md](models/frontier-model-notes.md) for current source-backed notes.

## The Core Prompt Pattern

```text
You are helping me complete [task].

Context:
- Goal: [what success looks like]
- Audience: [who this is for]
- Inputs: [paste notes, data, links, transcript, code, or draft]
- Constraints: [tone, length, tools, deadline, format, policy, brand, budget]

Work process:
1. Identify missing assumptions.
2. Decide the best approach.
3. Produce the requested output.
4. Check the output against the goal and constraints.

Output format:
[bullets/table/email/JSON/checklist/report/code/etc.]
```

## Freelance Client Workflow

Use the freelance client pack as a step-by-step stack:

1. Pick one buyer niche.
2. Turn one skill into a fixed-scope service wedge.
3. Build a proof asset before outreach.
4. Create a small prospect list with real triggers.
5. Write specific outreach and follow-ups.
6. Prepare discovery calls and proposals.
7. Track replies, calls, pilots, and retained clients.

Start here: [prompts/freelance-clients/README.md](prompts/freelance-clients/README.md)

## What Makes These Prompts Different

- Built for current reasoning and agentic models, not only old "act as..." chatbot prompts.
- Organized by real use case, not by model vendor.
- Includes quality checks, source handling, and verification steps.
- Written in plain English for daily users, with enough structure for advanced models.
- Avoids copying large prompt collections; links to the best public resources instead.

## Best External Prompt Resources

See [resources/github-prompt-resources.md](resources/github-prompt-resources.md) for a curated source list. The most useful starting points are:

- [f/prompts.chat](https://github.com/f/prompts.chat)
- [ai-boost/awesome-prompts](https://github.com/ai-boost/awesome-prompts)
- [promptslab/Awesome-Prompt-Engineering](https://github.com/promptslab/Awesome-Prompt-Engineering)
- [anthropics/prompt-eng-interactive-tutorial](https://github.com/anthropics/prompt-eng-interactive-tutorial)
- [dair-ai/Prompt-Engineering-Guide](https://github.com/dair-ai/Prompt-Engineering-Guide)

## Repo Structure

```text
.
+-- prompts/        Reusable prompt packs by use case
+-- models/         Current model notes and prompting differences
+-- resources/      Curated external links and source notes
+-- templates/      Reusable prompt structures
+-- checklists/     Prompt quality and safety checks
```

## Contributing

Use [CONTRIBUTING.md](CONTRIBUTING.md) to add or improve prompts. New prompts should be practical, model-agnostic when possible, and include a short quality checklist.

## License

Original content in this repo is released under MIT. External resources remain under their own licenses.

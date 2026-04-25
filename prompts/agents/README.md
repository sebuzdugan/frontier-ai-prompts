# Agent Prompts

## Autonomous Task

Best for: giving a model a multi-step job with checks.

```text
Complete this task end to end:
[task]

Goal:
[what done means]

Context:
[background, files, links, data, constraints]

Rules:
- Ask only if blocked by missing information that cannot be reasonably assumed.
- Keep a short visible plan.
- Use available tools when they materially improve accuracy.
- Verify the result before finalizing.
- Report what changed, what was checked, and any remaining risks.

Deliverable:
[exact format]
```

## Tool-Using Research Agent

Best for: web research or internal docs research.

```text
Act as a research agent for this question:
[question]

Scope:
[what to include/exclude]

Source requirements:
- Prefer primary sources.
- Use recent sources when facts may have changed.
- Cite sources for key claims.
- Flag stale, weak, or conflicting evidence.

Process:
1. Search broadly.
2. Narrow to credible sources.
3. Extract key evidence.
4. Synthesize the answer.
5. List open questions.
```

## QA Loop

Best for: making any output better before you use it.

```text
Improve this output through a QA loop.

Goal:
[goal]

Draft:
[paste draft]

Evaluate against:
- Accuracy
- Completeness
- Clarity
- Audience fit
- Missing edge cases
- Practical usefulness

Then produce:
- Issues found
- Improved version
- Final checklist
```

## Delegation Prompt

Best for: handing work to an AI assistant clearly.

```text
I want to delegate this:
[task]

You own:
[scope]

You do not own:
[non-goals]

Success criteria:
[criteria]

Constraints:
[constraints]

Before finalizing:
- Check your work against the success criteria.
- Identify assumptions.
- Explain any tradeoffs.
- Give me the final deliverable only after the check.
```

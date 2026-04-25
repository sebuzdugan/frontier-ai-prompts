# Coding Prompts

## Code Review

Best for: finding bugs and risky changes.

```text
Review this code like a senior engineer.

Context:
- Purpose of the change: [goal]
- Runtime/framework: [stack]
- Risk areas I care about: [security/performance/data loss/API compatibility/etc.]
- Code or diff:
[paste code/diff]

Focus on:
- Correctness bugs
- Edge cases
- Security or privacy risks
- Performance problems
- Missing tests

Output:
1. Findings first, ordered by severity
2. Exact file/function/line references if available
3. Suggested fix for each finding
4. Tests I should add
5. Short summary only after findings
```

## Debugging Partner

Best for: diagnosing an error without thrashing.

```text
Help me debug this issue.

Symptoms:
[what happens]

Expected behavior:
[what should happen]

Environment:
[language/framework/version/OS/deployment]

Recent changes:
[what changed]

Logs/errors:
[paste logs]

Code involved:
[paste relevant code]

Work as a debugging partner:
- List the 3 most likely causes
- For each, explain the evidence for and against it
- Give the smallest test to confirm or rule it out
- Then propose the safest fix
```

## Architecture Plan

Best for: designing a feature before coding.

```text
Design an implementation plan for this feature.

Feature:
[describe feature]

Existing system:
[architecture notes, files, APIs, constraints]

Requirements:
- Must have: [list]
- Nice to have: [list]
- Non-goals: [list]

Produce:
- Recommended approach
- Data model/API changes
- UI or workflow changes if relevant
- Edge cases
- Test plan
- Rollout plan
- Risks and alternatives
```

## Test Generator

Best for: turning behavior into focused tests.

```text
Generate a test plan and test cases.

Code or behavior:
[paste code/spec]

Testing framework:
[framework]

Focus:
- Normal behavior
- Boundary cases
- Error paths
- Regression risks

Output:
- Test plan summary
- Test cases as code
- Any mocks/fixtures needed
- What not to test and why
```

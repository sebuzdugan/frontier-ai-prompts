# JSON Output Template

Use this when the output will be parsed by software.

```text
Return only valid JSON. Do not include markdown.

Task:
[task]

Input:
[input]

Schema:
{
  "summary": "string",
  "items": [
    {
      "name": "string",
      "reason": "string",
      "confidence": "low | medium | high"
    }
  ],
  "open_questions": ["string"]
}

Rules:
- Use null when a value is unknown.
- Do not invent missing facts.
- Keep strings concise.
- Validate that the final response is parseable JSON.
```

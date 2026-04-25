# Model Selection Checklist

Use a stronger reasoning model when:

- The task is ambiguous.
- The answer requires planning.
- The model must use tools.
- The input is long or multimodal.
- Mistakes are expensive.
- You need high-quality coding, research, analysis, or document work.

Use a fast model when:

- The task is narrow.
- The output is easy to check.
- You need many cheap variations.
- You are classifying, formatting, extracting, or summarizing short text.

Use a multimodal model when:

- Inputs include images, screenshots, PDFs, audio, or video.
- Layout, visual detail, or spatial reasoning matters.

Use web/search-enabled models when:

- Facts may have changed recently.
- You need current prices, laws, schedules, product specs, or model availability.
- You need source citations.

Production rule:

- Build small evals for prompts that matter.
- Pin model versions or snapshots when the provider supports it.
- Track prompt changes like code changes.

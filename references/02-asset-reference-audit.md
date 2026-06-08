# Asset And Reference Audit

Use this before writing prompts or generating visuals. The goal is to prevent identity drift, product drift, logo errors, wrong packaging, and repeated rework.

## Asset Categories

Create a quick inventory with these categories:

- **Final locked assets**: must be followed closely. Use for character faces, products, packaging, logos, props, locations, typography, and approved style frames.
- **Candidate assets**: useful but not yet approved. Do not treat as final unless the user confirms.
- **Style references**: mood, lighting, rhythm, camera, palette, or texture references. Do not copy identity or content unless allowed.
- **Old process drafts**: may explain history but should not become source material automatically.
- **Rejected material**: explicitly not recommended. Do not reuse as a base unless the user asks for a rescue pass.

## Priority Rules

- Official, real, or user-provided source assets outrank AI-generated approximations.
- For products, packaging, logos, and brand text, prefer direct source migration, traceable reference, or locked asset usage over regenerated text.
- For characters, use the most authoritative model sheet or real reference. Keep face shape, silhouette, clothing, markings, proportions, and signature details stable.
- For locations, lock a master wide shot or map before making close-ups.
- For props, define the exact shape, color, scale, and relationship to characters before generating scenes.

## Audit Table

Use this compact table for internal planning or handoff:

| Asset | Type | Source path or link | Status | Must preserve | Do not change | Notes |
| --- | --- | --- | --- | --- | --- | --- |
|  | character/product/logo/scene/prop/style |  | locked/candidate/reference/rejected |  |  |  |

## Questions To Ask

- Which source is the highest authority for each important asset?
- Are any filenames misleading compared with image contents?
- Are there details that often drift, such as eyes, eyebrows, silhouettes, logos, text, outfit, product side panels, or scale?
- Should generated images be based on source image references, local compositing, or text prompts?
- Which old files should be marked "not recommended" so they do not re-enter the workflow?

## Prompt Implications

Every prompt package should include:

- locked reference list
- per-asset preservation rules
- negative rules for common drift
- whether text/logo should be generated, composited, or left blank for design work
- status of old drafts

## Practical Defaults

- If the task has many assets, make or request a reference board before generating.
- If a product or packaging text must be readable, avoid relying on AI text generation unless the user accepts risk.
- If a batch depends on one character or product, produce one calibration image first.
- If multiple shots share a space, lock a wide shot or spatial diagram first.

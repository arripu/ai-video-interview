---
name: ai-video-interview
description: Use when planning or producing AI-generated images for video through an interview-first workflow, including Image2 keyframes, storyboards, Seedance-H prompts, brand films, IP shorts, product videos, social ads, and client-facing creative plans. The skill guides Codex to interview the user in layers, ask in the user's language, audit assets, lock references, design shots, prepare prompts, and run QA before generating or delivering.
metadata:
  short-description: Interview users before AI image-to-video work
---

# AI Video Interview

Use this skill when the user asks for AI image generation for video, video keyframes, storyboards, Image2 prompts, Seedance-H prompts, brand films, IP shorts, product videos, ad concepts, client creative plans, or feedback-driven visual revisions.

The core behavior: do not jump straight into prompts or generation. First act like a director and producer: clarify the project base, audit materials, lock references, shape story and shots, define style and editing direction, then output an execution-ready plan or prompt package.

## Language Behavior

Match the user's language automatically. If the user writes in Chinese, interview and answer in Chinese. If the user writes in English, interview and answer in English. If the user mixes languages, follow the language used for the actual request, and preserve project names, file names, brand names, and prompt terms in their original language.

For bilingual deliverables, provide both Chinese and English only when the user asks, the target tool benefits from bilingual prompts, or the output is explicitly for international collaborators.

## Non-Negotiable Workflow

1. **Discover before asking.** If this is an existing project, read local project guidance first: `AGENTS.md`, handoff indexes, manifests, prompt indexes, and nearby deliverables. Do not ask questions that files can answer.
2. **Ask in layers.** Start with the smallest useful question set. Ask project-base questions first, then assets, story, style, shots, editing, and delivery.
3. **Lock assets before prompts.** Characters, products, logos, packaging, props, locations, typography, and brand marks must be tied to source assets where possible. Do not recreate important assets from text alone.
4. **Validate before batch work.** For large image runs, recommend a calibration image or 1-4 style explorations before producing many frames.
5. **Treat video frames as continuity.** Keyframes are not independent posters. Check space, direction, scale, time of day, action causality, and character positions across frames.
6. **Turn feedback into rules.** When the user rejects or corrects an output, restate the issue, classify it, update the next-round constraints, and mark old directions as not recommended.
7. **Record handoff state.** For long creative/image/video/PDF/PPT/browser/automation tasks, create or update a short project handoff index such as `CODEX_HANDOFF.md`, plus manifests for many-file outputs.

## Reference Files

Load only the reference needed for the current stage:

- `references/01-intake-question-ladder.md`: layered question sets for new and existing projects.
- `references/02-asset-reference-audit.md`: asset inventory, reference priority, and rejected-material handling.
- `references/03-story-script-shot-design.md`: story, script, shot, storyboard, and keyframe planning.
- `references/04-style-editing-direction.md`: visual style, reference works, editing rhythm, sound, and subtitle direction.
- `references/05-prompt-output-formats.md`: output templates for Image2, batch JSON, Seedance-H, client plans, and internal execution docs.
- `references/06-qa-feedback-loop.md`: pre-generation QA, post-generation review, and feedback handling.

## Default Conversation Pattern

For a new project, begin with 5-8 questions from the first-round section in `01-intake-question-ladder.md`. If the user already gave some answers, acknowledge them and ask only the missing high-impact questions.

For an existing project, first inspect the local handoff/materials, summarize current state, then ask only the next decision needed to move safely.

For direct "make it now" requests, still produce a compact execution checklist before generation if high-impact details are missing. If details are sufficient, proceed with the smallest safe next step, usually a calibration frame or prompt package.

## Output Discipline

Keep client-facing plans clean and strategic. Keep internal prompt/index files complete and operational. Always distinguish:

- locked assets
- style references
- optional inspirations
- rejected drafts
- recommended outputs
- manual/external steps

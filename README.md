# AI Video Interview

AI Video Interview is an interview-first workflow for planning AI image-to-video projects before writing prompts or generating visuals.

It helps creators, strategists, editors, designers, and AI operators clarify a video brief through structured questions, audit source assets, lock references, plan story and shots, prepare image/video prompts, and run QA before scaling into batch generation.

## What It Does

- Interviews the user in layers before prompt writing.
- Clarifies project goal, audience, platform, length, aspect ratio, and success criteria.
- Audits logos, characters, products, packaging, props, scenes, scripts, music, and reference videos.
- Separates locked assets, style references, candidate materials, process drafts, and rejected directions.
- Designs story structure, shot lists, storyboards, keyframes, and 15-second video nodes.
- Prepares Image2 prompts, batch keyframe JSON, Seedance-H prompts, client-facing plans, and internal execution docs.
- Runs pre-generation QA, post-generation review, and feedback loops.

## Who It Is For

- AI image-to-video creators
- Brand film planners
- Product video teams
- IP character video teams
- Social ad creators
- Creative directors and producers
- Prompt engineers
- Editors and designers who need clearer pre-production briefs

## Language Behavior

The workflow follows the user's language automatically:

- If the user writes in English, it interviews and answers in English.
- If the user writes in another language, it interviews and answers in that language.
- If the user mixes languages, it follows the language of the actual request.
- Project names, file names, brand names, and prompt terms are preserved in their original language.
- Bilingual output is used only when requested or useful for the target tool or collaborators.

## Install As A Codex Skill

Install this repository as a Codex skill from GitHub. After installation, restart Codex so it can load the new skill.

Use this invocation:

```text
$ai-video-interview
I want to make a 30-second product video. Interview me first before writing prompts.
```

Continue an existing project:

```text
$ai-video-interview
Continue this project. First read the project handoff, manifests, and approved/rejected outputs, then ask only the next necessary questions.
```

## Use Without Codex

This repository is also useful outside Codex. If your AI assistant does not support Codex skills, open `PORTABLE_PROMPT.md`, copy the prompt, and paste it into your assistant before describing your project.

Recommended portable workflow:

1. Paste `PORTABLE_PROMPT.md` into your AI assistant.
2. Add your project brief, files, references, or constraints.
3. Ask the assistant to interview you first instead of writing prompts immediately.
4. Answer the interview questions.
5. Ask for an execution plan, shot list, Image2 prompts, video prompts, or QA checklist.

## Best For

- AI image-to-video planning
- Image2 prompt planning
- Storyboards
- Video keyframes
- Seedance-H prompts
- Brand films
- IP character videos
- Product videos
- Social ad concepts
- Client-facing creative plans
- Feedback-driven visual revisions

## Repository Structure

```text
.
├── SKILL.md
├── PORTABLE_PROMPT.md
├── agents/
│   └── openai.yaml
└── references/
    ├── 01-intake-question-ladder.md
    ├── 02-asset-reference-audit.md
    ├── 03-story-script-shot-design.md
    ├── 04-style-editing-direction.md
    ├── 05-prompt-output-formats.md
    └── 06-qa-feedback-loop.md
```

## Core Principle

Do not waste generations on unclear briefs.

Interview first. Lock assets. Test small. Then scale.

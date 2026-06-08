# QA And Feedback Loop

Use this before and after generation, and whenever the user gives feedback.

## Pre-Generation Checklist

Confirm or infer:

- purpose
- audience
- platform
- duration
- aspect ratio
- locked assets
- style references
- forbidden directions
- output format
- approval gate before batch generation

If three or more high-impact items are unknown, ask another question round instead of generating.

## Post-Generation Review

Review each image or prompt package against:

- character identity
- product/prop fidelity
- logo/text accuracy
- scene continuity
- scale and proportion
- action readability
- camera usefulness for video
- style consistency
- lighting consistency
- unwanted extra elements
- repeated subject errors
- whether it deserves recommended status

For video keyframes, also check:

- direction of motion
- spatial position across frames
- camera progression
- transition logic
- time of day
- subject entering/exiting frame
- whether a missing in-between frame is needed

## Feedback Classification

When the user says an output is wrong, classify the feedback:

- **Asset problem**: character, product, logo, packaging, prop, or text changed.
- **Scene problem**: location, layout, scale, or continuity changed.
- **Action problem**: motion, pose, direction, or causal relation is wrong.
- **Style problem**: tone, lighting, palette, texture, quality, or genre is wrong.
- **Composition problem**: framing, angle, crop, density, or focus is wrong.
- **Tool limitation**: readable text, exact logo, or fine details may require compositing or design work.
- **Brief problem**: original instruction lacked a needed decision.

Then turn it into:

- new must-preserve rules
- new negative rules
- old drafts to mark rejected
- smallest next test output

## Feedback Response Pattern

Use this rhythm:

1. Briefly restate the user's correction.
2. Identify what category of problem it is.
3. State the new rule for the next attempt.
4. Recommend whether to do one calibration image or apply across the batch.
5. Update manifest/handoff when files are involved.

## Rejected And Recommended States

Do not let rejected drafts silently remain in the candidate pool. Use clear wording:

- "not recommended"
- "process draft"
- "rejected due to identity drift"
- "recommended final"
- "recommended for style only"
- "approved as calibration reference"

## Stop Conditions

Pause before batch execution when:

- character or product identity is not locked
- the user is choosing between style directions
- a reference source is contradictory
- the output format affects later work
- a single wrong assumption would waste many generations

Proceed when:

- the next step is small and reversible
- the user has approved a calibration direction
- missing details can be safely defaulted
- files or manifests clearly define the current state

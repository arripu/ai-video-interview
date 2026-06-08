# Prompt And Output Formats

Use these templates when the task moves from questions into execution.

## Image2 Single-Frame Prompt

```markdown
Project:
Shot ID:
Purpose:
Aspect ratio / size:

Locked references:
- 

Scene:
Subject:
Action:
Camera:
Lighting:
Style:
Continuity:

Prompt:

Negative rules:
- 

QA focus:
- 
```

## Batch Keyframe JSON

```json
{
  "project": "",
  "version": "v1",
  "aspect_ratio": "16:9",
  "generated_for": "image-to-video keyframes",
  "frames": [
    {
      "id": "shot_001",
      "timecode": "00:00-00:03",
      "purpose": "",
      "prompt": "",
      "locked_assets": [],
      "negative_rules": [],
      "status": "planned"
    }
  ]
}
```

Recommended statuses:

- `planned`
- `waiting_for_user_confirmation`
- `ready_to_generate`
- `generated_for_review`
- `recommended`
- `rejected`
- `needs_revision`

## Seedance-H 15-Second Node

```json
{
  "project": "",
  "version": "v1",
  "nodes": [
    {
      "time_range": "00:00-00:15",
      "story_role": "",
      "shot_sequence": [
        {
          "shot": "1",
          "duration": "",
          "subject_action": "",
          "camera_motion": "",
          "scene_change": "",
          "emotion_rhythm": "",
          "style_keywords": "",
          "negative_rules": ""
        }
      ],
      "prompt_zh": "",
      "prompt_en": ""
    }
  ]
}
```

Default to Chinese if the user asks for Seedance-H in this project style. Provide bilingual output only when useful or requested.

## Client-Facing Creative Plan

Use this for PPT/PDF/client review:

- Project goal
- Core creative idea
- Target audience and platform
- Video structure
- Visual style
- Key scenes
- Brand/product appearance
- Production approach
- Confirmation points

Do not dump full prompts into a client-facing plan unless requested.

## Internal Execution Doc

Use this for production handoff:

- project name
- version/date
- asset inventory
- locked rules
- shot table
- full prompts
- output filenames
- recommended drafts
- rejected drafts
- next confirmation points
- manual/external steps

## Manifest Fields

For many-file outputs, create or update a manifest with:

```json
{
  "project": "",
  "created_at": "",
  "task": "",
  "source_inputs": [],
  "outputs": [
    {
      "path": "",
      "role": "",
      "status": "",
      "notes": ""
    }
  ],
  "recommended_outputs": [],
  "rejected_outputs": [],
  "next_steps": []
}
```

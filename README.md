# AI Video Interview / AI视频访谈

AI Video Interview is an interview-first Codex skill for planning AI image-to-video projects before writing prompts or generating visuals.

AI视频访谈是一个“先访谈、再跑图”的 Codex skill。它适合在制作 AI 视频图片、Image2 关键帧、分镜、Seedance-H 提示词、品牌短片、IP 短片、产品视频和甲方创意方案前，先把需求问清楚，再进入执行。

## What It Does

- Interviews the user in layers before prompt writing.
- Clarifies project goal, audience, platform, length, aspect ratio, and success criteria.
- Audits logos, characters, products, packaging, props, scenes, scripts, and reference videos.
- Separates locked assets, style references, candidate materials, old drafts, and rejected directions.
- Designs story structure, shot lists, storyboards, keyframes, and 15-second video nodes.
- Prepares Image2 prompts, batch keyframe JSON, Seedance-H prompts, client-facing plans, and internal execution docs.
- Runs pre-generation QA, post-generation review, and feedback loops.

## 它能做什么

- 在写提示词或生图前，先像采访一样逐层提问。
- 梳理项目目的、受众、平台、时长、画幅和成功标准。
- 盘点 logo、角色、产品、包装、道具、场景、脚本、参考视频等素材。
- 区分正式锁定资产、风格参考、候选素材、旧过程稿和明确作废方向。
- 规划故事结构、镜头表、分镜、关键帧和 15 秒视频节点。
- 输出 Image2 提示词、批量关键帧 JSON、Seedance-H 提示词、甲方方案和内部执行文档。
- 建立生图前质检、生图后审查和用户反馈闭环。

## Language Behavior / 语言规则

The skill follows the user's language automatically:

- If the user writes in Chinese, it interviews and answers in Chinese.
- If the user writes in English, it interviews and answers in English.
- If the user mixes languages, it follows the language of the actual request.
- Project names, file names, brand names, and prompt terms are preserved in their original language.
- Bilingual output is used only when requested or useful for the target tool/collaborators.

这个 skill 会自动跟随用户语言：

- 用户用中文，它就用中文访谈和回复。
- 用户用英文，它就用英文访谈和回复。
- 用户中英混合时，优先跟随实际任务请求的语言。
- 项目名、文件名、品牌名、提示词术语保留原文。
- 只有用户要求，或目标工具/跨国协作需要时，才输出中英双语。

## Install

In Codex, install this skill from GitHub:

```text
https://github.com/arripu/ai-video-interview
```

After installation, restart Codex to pick up the new skill.

## Usage

Explicitly call the skill with:

```text
$ai-video-interview
I want to make a 30-second product video. Interview me first before writing prompts.
```

中文示例：

```text
$ai-video-interview
我想做一个 30 秒宠物品牌视频，先不要生图，先采访我，把需求问清楚。
```

Continue an existing project:

```text
$ai-video-interview
Continue this project. First read the project handoff, manifests, and approved/rejected outputs, then ask only the next necessary questions.
```

继续旧项目：

```text
$ai-video-interview
继续这个项目。先读项目交接索引、manifest 和推荐稿/作废稿记录，再问我下一步最关键的问题。
```

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

## Philosophy

Do not waste generations on unclear briefs. Interview first, lock assets, test small, then scale.

不要在需求不清楚时浪费生图次数。先访谈，先锁资产，先小样，再批量。

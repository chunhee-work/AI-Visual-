---
name: active-creative-skill-stack
description: The Higgsfield/Seedance creative skill stack the user wants active and used in the AI Visual project
metadata: 
  node_type: memory
  type: project
  originSessionId: cda39d5a-a05d-4185-9eca-d3d90e2d35e0
---

For the "AI Visual" project the user has assembled a creative-generation skill stack and wants it used proactively, not just when explicitly named.

**The stack (all installed under `~/.claude/skills/`):**
- `banana-pro-director` — Higgsfield image prompts (Banana Pro / Soul Cinema / GPT-2): character outfit base refs, 6-panel sheets, scene plates.
- `cinema-worldbuilder` — Seedance video prompts via 5 cinema modes (Narrative/Studio/Action/Performance/Atmospheric) + diegetic-audio rule. Hands off to `banana-pro-director` for character dev.
- `video-prompt-builder` — shot-by-shot Seedance 2.0 prompts from a brief.
- `seedance-prompt-library` — curated reference of proven Seedance 2.0 prompts (7 categories) + the nine commercial use-cases (追热点/运动饮料/品牌宣传/穿搭变装/直播带货/动态海报/广告复刻/真人短剧/AI漫剧). Built 2026-05-21 from the awesome-seedance repo; the copy-paste/recipe companion to the generators.
- `nanobanana-ppt` — AI PPT/deck generation.
- `fal-image-edit` — image editing via fal.ai (style transfer, bg/object removal, inpainting).
- Plus design-taste skills (`gpt-taste`, `image-to-code`, etc.) and process skills (`brainstorming`, `writing-plans`, `writing-skills`).

**Why:** On 2026-05-21 the user installed these and said "moving forward pls use it as well." They run a Higgsfield + Seedance AI visual production pipeline.

**How to apply:** When a request touches image refs / character sheets / scene plates, reach for `banana-pro-director`. When it touches video / Seedance / shot lists, reach for `cinema-worldbuilder` or `video-prompt-builder`. Decks → `nanobanana-ppt`. Image edits → `fal-image-edit`. Higgsfield MCP tools (`generate_image`, `generate_video`) are available for actual generation. Note these skills live only on local disk under `~/.claude/skills/`, NOT in the project's git repo. Respond bilingually per [[bilingual-mandarin-responses]].

---
name: auto-invoke-relevant-skills
description: "User wants me to auto-invoke any installed skill when the task at hand calls for it — never stop to ask 'should I load this skill?' Just load it and proceed."
metadata: 
  node_type: memory
  type: feedback
  originSessionId: cda39d5a-a05d-4185-9eca-d3d90e2d35e0
---

User explicitly directed (2026-05-28): **"if there's a mission needed for the skill pls auto use it ok?"**

**The rule:** When the task at hand matches a skill the user has installed (visible in the available-skills list in the system reminder), I should auto-invoke it via the `Skill` tool WITHOUT asking the user first. Just load it and proceed with the work.

**Why:** User runs a creative production pipeline (Higgsfield image gen → Seedance video gen → trailer assembly) with many specialized skills installed. They don't want friction of "should I load X?" questions — if a skill clearly fits the immediate task, just use it.

**How to apply:**
1. Before starting any new task, silently scan the available-skills list for skills matching the task type.
2. If a clear match exists (e.g., user mentions Seedance video → invoke `cinema-worldbuilder` or `video-prompt-builder` or `seedance-prompt-library`; user wants to edit an existing image → invoke `fal-image-edit`; user hits a creative fork → invoke `brainstorming`), auto-load it via the `Skill` tool and proceed.
3. Briefly mention which skill loaded ("Loading `cinema-worldbuilder` for the Seedance step") so the user knows what's running — but never ask permission.
4. If multiple skills could fit, pick the most specific one. If none clearly fit, don't force-load anything.
5. Don't re-load a skill already loaded earlier in the conversation.

**Specifically for the [[land-of-hope-trailer]] project pipeline:**
- **Stage 1 — Image generation (current):** `banana-pro-director` (already active) · `fal-image-edit` (auto-load if user asks to fix/inpaint/swap part of an existing image) · `brainstorming` (auto-load if user hits a creative fork)
- **Stage 2 — Video generation (upcoming):** auto-load `cinema-worldbuilder` + `video-prompt-builder` + `seedance-prompt-library` when we shift from stills to video
- **Stage 3 — Branded delivery:** auto-load `brandkit` for the title card / end branding

**Exception — don't force-load:**
- Code/dev skills (TDD, debugging, plans, code-review) — this is a creative pipeline, not code work
- Web/app UI design skills (ui-ux-pro-max, stitch-design-taste, etc.) — irrelevant to trailer production
- Platform-specific (claude-api, security-review) — irrelevant

Per [[bilingual-mandarin-responses]], announce skill loads bilingually when applicable.

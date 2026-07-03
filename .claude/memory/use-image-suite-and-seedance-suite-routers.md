---
name: use-image-suite-and-seedance-suite-routers
description: MOVING FORWARD default workflow — image-generation requests route through the image-suite router; Seedance video-prompt requests route through the seedance-suite router. User directive 2026-06-26.
metadata: 
  node_type: memory
  type: feedback
  originSessionId: db5b1b76-9ee9-4ced-a73f-3ecd05a4b814
---

User directive (2026-06-26 + RE-CONFIRMED 2026-06-25): "moving forward when I ask for image generate pls use image-suit; when I ask for seedance prompt use seedance suit." Two unified **router** skills the user uploaded to the repo root.

- **image-suite** → `image-suite.skill` (ZIP bundle containing `image-suite/SKILL.md`) in repo root. Verified contents: routes to A=Banana Pro Director, B=Brand Kit, C=Imagegen Frontend Web, D=Imagegen Frontend Mobile, E=Muapi Storyboard.
- **seedance-suite** → `Seedance-suite.md` (plain markdown ~647 lines) in repo root. Verified contents: routes to A=Video Prompt Builder, B=Shotlist Director (HTML output), C=Prompt Library.

Both are ROUTER skills: pick exactly ONE sub-skill per task, follow it verbatim, don't blend methods.

**Why:** These are now the user's default methodology for all image + Seedance prompt work. They consolidate the previously-separate sub-skills under one routing entry each.

**How to apply:**

**ANY image-generation / art-direction request → use image-suite. Route to ONE of:**
| Task | Sub-skill |
|---|---|
| Photoreal character/scene stills — outfit ref on white seamless, multi-angle character/model sheet, scene/env plate, face/portrait (Higgsfield Banana Pro / Soul Cinema / GPT-2) | **A · Banana Pro Director** |
| Brand system — brand-guideline board, logo system, identity deck | **B · Brand Kit** |
| Website design-reference images — one separate image PER section | **C · Imagegen Frontend Web** |
| Mobile app screen concepts in phone mockups | **D · Imagegen Frontend Mobile** |
| Story/scene sequence → N keyframe images (image only) | **E · Muapi Storyboard** |
Tie-breakers: person/product/scene photo→A; logo/brand board→B; web layout→C; phone screen→D (web+mobile = run C then D separately); ordered narrative frames→E. Not an editor (no inpaint/bg-removal/PPT).

**ANY Seedance video-prompt request → use seedance-suite. Route to ONE of:**
| Task | Sub-skill |
|---|---|
| Fresh brief, one effects-driven / high-energy clip (editing, effects density, pacing, energy arc) | **A · Video Prompt Builder** (plain-text 4-section effects breakdown) |
| Script/story/treatment → multiple cinematic scenes with continuity, dialogue, acting, tickable list | **B · Shotlist Director** (editable HTML saved to outputs) |
| Proven copy-paste example/template, or one of the nine commercial plays (追热点 / 运动饮料广告 / 品牌宣传 / 穿搭变装 / 直播带货 / 动态海报 / 广告复刻 / 真人短剧 / AI漫剧) | **C · Prompt Library** |
Tie-breakers: stacked transitions/speed-ramps/"punchy"→A; restraint/natural-light/multi-scene narrative→B; single standalone→A or C; whole production shot scene-by-scene→B. Library (C) can feed A/B.

**IMPORTANT — project rules still layer ON TOP of the router output** for OG10 / Land of Hope work: the mandatory [[seedance-style-surface-treatment-block]], [[seedance-prompt-char-limit]] (≤4000), [[seedance-9-image-ref-limit]], [[og10-teaser-no-face-hands-legs-backview]], [[land-of-hope-locked-visual-style]], [[gpt-image-prompt-format]], [[higgsfield-always-specify-refs]] etc. The suite chooses the METHOD/structure; the locked project memories still constrain style, refs, and limits. Also keep [[bilingual-mandarin-responses]] (Mandarin summary above every EN prompt code block).

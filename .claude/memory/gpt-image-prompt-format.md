---
name: gpt-image-prompt-format
description: "How to write image-generation prompts so they actually work in the user's Higgsfield + GPT Image 2 setup — natural-language prose, never keyword-stuffed diffusion prompts"
metadata: 
  node_type: memory
  type: feedback
  originSessionId: cda39d5a-a05d-4185-9eca-d3d90e2d35e0
---

The user generates images in **Higgsfield using the GPT Image 2 model** (OpenAI's image model). GPT Image 2 follows **natural-language instructions** and chokes on long, comma-stuffed, keyword-dense diffusion-style prompts — it averages keyword piles into mush.

**Rule for EVERY image-gen prompt I give (going forward, from 2026-05-26):**
- Write it as clean, coherent **natural-language instructions** — plain sentences, not keyword lists.
- **Scene/subject first, style last.** Describe the shot in plain prose, then the style as prose at the end (GPT Image 2 obeys in order).
- **DROP keyword tails** like "8K, ray-traced global illumination, ultra-detailed, hyperrealistic, micro surface detail, volumetric, octane render." They don't help GPT Image 2 and flatten the result.
- Keep the locked style INTENT (cinematic animated-feature still; moody high-contrast chiaroscuro; warm amber/gold grade; volumetric god-rays + haze + dust; shallow DOF + soft bokeh; painterly stylized-but-realistic Pixar/Disney, NOT photoreal real animals/humans) — just express it in concise prose.
- Multi-image reference instructions ("use image 1 as the style guide… image 2 as the corruption…") still work — keep them plain and explicit.
- **AVOID the NSFW / violence filter — GPT Image 2 hard-blocks it.** Reframe the war/corruption scenes as **protective magic, NOT violence**: the red-eyed crowd are **spellbound / enchanted villagers** who drift forward in a daze, and the heroes **gently hold back / ease back / shield / calm** them while protecting families; "no one is hurt." Do NOT use: attack, kill, blow, blast, strike, slash, stab, knock down, wound(ed), blood, gore, razor, weapon, foe, enemy, horde, corpse. Use: shield, barrier, soft glowing light, gentle force, hold the line, sweep/ease back. (2026-05-26: a battle storyboard prompt was blocked as NSFW; this reframe is also true to the "never-kill, they're their own people" story rule.)
- **GPT Image 2 can't do multi-panel storyboard SHEETS of different scenes.** A single-subject 6-view turnaround (one character, 6 angles) renders fine, but a 6-panel grid of 6 DIFFERENT shots fails or comes out a mess. So board scenes as **one single image per shot** (one prompt each), NOT as a grid — which is better for cutting the trailer anyway. (2026-05-26: the safe, gentle S14 crystal sheet wouldn't render as a 6-panel grid.)
- Still deliver bilingually EN + 中文 per [[bilingual-mandarin-responses]].

**Why:** On 2026-05-26 the long keyword-stuffed "SHARED STYLE" block failed in GPT Image 2; the user said "moving forward make sure this will not happen again." The plain-prose GPT-Image-2 rewrite is the format to use from now on.

**Note:** the keyword-heavy blocks in [[cinematic-keyart-standard]] and the earlier SHARED STYLE versions are diffusion-era — re-express as prose for GPT Image 2. Natural-language prose is the safe default; only revert to keyword style if the user explicitly switches to a diffusion model (Banana Pro / Nano Banana tolerate keywords).

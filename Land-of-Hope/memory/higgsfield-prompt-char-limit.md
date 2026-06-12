---
name: higgsfield-prompt-char-limit
description: "⭐ Higgsfield GPT Image 2 has a HARD CHAR LIMIT — every image-generation prompt MUST stay under 15000 characters. If a prompt exceeds the limit, generation fails. Compress style block + character locks + panel descriptions to fit. Saved 2026-06-12."
metadata:
  type: feedback
  node_type: memory
  originSessionId: cda39d5a-a05d-4185-9eca-d3d90e2d35e0
---

**⭐ CRITICAL — Rule (locked 2026-06-12):** Every Higgsfield prompt for image generation (GPT Image 2 and similar Higgsfield models) MUST stay UNDER 15000 characters total. Going over this limit causes generation to fail.

**Why:** 2026-06-12 — User flagged this hard char limit after several long multi-panel storyboard prompts approached or exceeded the limit. Higgsfield rejects/fails generation when the prompt is too long.

**How to apply going forward:**

1. **ALWAYS check char count** before delivering any Higgsfield prompt. Target under 15000 chars (with safety margin around 14500).

2. **Compression techniques** when a prompt is long:
   - **Trim the LOCKED SHARED STYLE block** — use the full version only when necessary; for prompts that don't need the full style guide, use a compressed 2-3 sentence version
   - **Combine repetitive character locks** — describe each character ONCE in a SHARED CHARACTER LOCKS section, then reference by name only in panel descriptions ("CCATS in his canonical brass armor X-block stance" rather than re-describing all CCATS details)
   - **Shorter panel descriptions** — focus on the KEY action + key camera angle + key elements, drop redundant detail (the style block already covers lighting/grade/atmosphere)
   - **Drop redundant style locks at the end** — if the style is already established at start, the closing style lock can be very brief (1-2 sentences)
   - **Use → arrow shorthand for transitions** instead of full prose
   - **Combine LIGHT DIRECTION + COLOR & GRADE + RIM/EDGE LIGHT + SHADOWS + ATMOSPHERE etc** into one compressed paragraph when needed
   - **For 6-panel cinema sheets**: each panel ~150-200 words max (not 300-400)
   - **For 16-panel storyboards**: each panel ~80-120 words max

3. **Priority order when compressing** (keep these elements, trim everything else):
   - ⭐ Character canonical fidelity locks (CRITICAL — these are why the renders look right)
   - ⭐ Layout/format description (sheet structure, panel grid)
   - ⭐ Per-panel KEY action + camera angle
   - ⭐ Identity locked across panels clause
   - 🔻 Trim: redundant atmospheric details, long style guide explanations, redundant closing style locks

4. **For multi-panel sheets approaching limit**: consider splitting into 2 sheets (e.g., 6-panel split into 3+3 if needed) rather than trying to cram everything into one long prompt.

5. **Test before delivery**: rough mental char count check. If >12000 chars, start compressing. If >14000 chars, definitely compress before delivering.

**Compression example — LOCKED SHARED STYLE compressed version (for when full version doesn't fit):**

> SHARED STYLE: high-end cinematic film still, major-studio 3D animated feature register (Pixar/Disney/DreamWorks/Puss in Boots: The Last Wish painterly hand-rendered finish — NOT photoreal, NOT flat illustration, NOT plastic CG). Dramatic moody chiaroscuro with one strong warm motivated key light + cool indigo rim, dense volumetric atmospheric haze with drifting embers/dust motes, layered depth staging with tack-sharp foreground + creamy soft-focus background, rich warm filmic color grade, shallow depth of field, fine film grain, subtle vignette. Ultra-fine detail: realistic fabric weave + fur strand-by-strand + skin subsurface scattering + soulful eyes with crisp catchlights. Soft cinematic naturalistic restrained premium lighting — slightly sculpted, never theatrical. 8K ray-traced global illumination.

That compressed version is ~530 chars vs the full block which is ~3500 chars — saves 3000+ char budget for actual prompt content.

**Cross-references:**
- [[seedance-prompt-char-limit]] — Seedance 2.0 has its own 4000 char limit (different platform)
- [[land-of-hope-locked-visual-style]] — LOCKED two-block style (full + compressed versions)
- [[gpt-image-prompt-format]] — GPT Image 2 prompt format guide

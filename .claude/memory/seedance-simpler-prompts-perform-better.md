---
name: seedance-simpler-prompts-perform-better
description: "⭐ For Seedance 2.0, SIMPLER inline character descriptions + FEWER refs (3-5) outperform over-detailed per-character canonical ref blocks (8-10 refs). Don't write 'STRICT CHARACTER CANONICAL FIDELITY per each @图片X' — Seedance gets confused by too much specificity. Locked 2026-06-15."
metadata:
  node_type: memory
  type: feedback
  originSessionId: cda39d5a-a05d-4185-9eca-d3d90e2d35e0
---

**⭐ Rule (locked 2026-06-15):** For Seedance 2.0 prompts, the SIMPLER VERSION with INLINE character descriptions + FEWER REFS (3-5 total) consistently outperforms the over-detailed version with per-character canonical ref blocks (8-10 refs).

**Why:** 2026-06-15 — User explicitly compared two versions of Clip 06C-A:
- V1: Sheet 06C + Whisper + env (3 refs) + inline compact hero descriptions "CCATS brass armor + SKET dark iron samurai + GST skateboard..."
- V2/V3: STRICT CHARACTER CANONICAL FIDELITY block with 8 individual hero @图片 refs (9-10 refs) + per-character canonical detail lists

User confirmed: "your first prompt performance better" — meaning V1 won despite having less explicit canonical fidelity. The over-prescriptive V2/V3 approach made it WORSE not better.

**Hypothesis on why simpler wins:**
- Seedance has "specification fatigue" — too many constraints make it pick-and-choose what to honor, often dropping the most important
- A single composition anchor (Sheet showing all heroes in canonical form) is stronger than 8 isolated identity refs
- Inline compact descriptions read as creative direction; per-character ref blocks read as a checklist Seedance partially fails
- 3-5 refs sweet spot for Seedance attention budget

**How to apply going forward:**

1. **DEFAULT Seedance ref approach (3-5 refs):**
   - Storyboard sheet (composition + style + identity anchor in one)
   - Villain/boss canonical (if scene needs threat lock)
   - Environment anchor (if env-critical)
   - Optional: 1-2 critical character refs ONLY if the storyboard sheet doesn't show that character clearly

2. **AVOID this structure (it hurts more than helps):**
   ```
   ⚠️ STRICT CHARACTER CANONICAL FIDELITY per each ref:
   - @图片2 SKET: chibi anthropomorphic TABBY CAT samurai + FULL DARK IRON ARMOR + KABUTO HELMET...
   - @图片3 CCATS: chibi anthropomorphic ORANGE TABBY CAT + brass steampunk barista...
   [8 individual @图片 blocks]
   ```

3. **USE this structure instead (compact inline):**
   ```
   Formation: 8 heroes BACK-TO-CAMERA facing Whisper. CCATS brass armor + SKET dark iron samurai full armor + kabuto paw-print + twin katana red rope saya + GST skateboard + blue-white lightning palm + FROAK frog elder + jade chi + FOT chibi boy dark purple spiky hair + dark purple hooded cloak + dual chopsticks + ZEYO chibi boy black messy spiky hair + white origami robe + 2 floating scrolls + KETDONUT kitten on pink giant donut + handheld pink blaster + LYCHEE chibi girl burgundy-red wavy hair + red qipao + 5 ruby orbs pentagon.
   ```

4. **Trade-off:**
   - Identity may still drift slightly on individual heroes (1-2 of 8 may not be 100% canonical)
   - BUT overall scene quality + action + composition + cinematography are better
   - User accepts minor identity drift over compromised scene quality

5. **When to BREAK this rule (use per-character refs):**
   - Single-character close-up clips (1 hero focus → use 1-2 individual refs is fine)
   - When V1-style failed AND user explicitly requested stricter identity lock
   - Never DEFAULT to per-character ref blocks for group/combat scenes

**Cross-references:**
- [[seedance-9-image-ref-limit]] — 9 ref hard cap; this rule reinforces staying well under
- [[seedance-refs-only-when-needed]] — only refs actually present in clip
- [[seedance-cinematic-continuity-rules]] — storyboard sheet as primary style+composition ref
- [[higgsfield-always-specify-refs]] — different platform; Higgsfield benefits from explicit per-ref blocks. Don't confuse the two.

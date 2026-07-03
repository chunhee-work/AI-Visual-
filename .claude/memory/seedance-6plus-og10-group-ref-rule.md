---
name: seedance-6plus-og10-group-ref-rule
description: "⭐⭐ Seedance ref optimization rule — When 6+ OG10 heroes in same scene, use ONE consolidated OG10 group/lineup ref instead of individual canonical refs per character. Saves ref slots (9-cap), simpler prompt = better performance. <6 OG10 → can use individual canonical refs. Locked 2026-06-18."
metadata:
  node_type: memory
  type: feedback
  originSessionId: cda39d5a-a05d-4185-9eca-d3d90e2d35e0
---

**⭐⭐ Rule (locked 2026-06-18):** When a Seedance scene has 6+ OG10 heroes appearing together, use ONE consolidated OG10 group lineup reference image instead of attaching individual character canonical refs. When the scene has fewer than 6 OG10, can use individual canonical refs.

**Why:** 2026-06-18 — User explicitly directed: "moving forward if not over than 6+ OG10 in one scene let's just use their 6 body view in one seedance prompt."

This optimization addresses:
1. **Seedance 9-ref hard cap** per [[seedance-9-image-ref-limit]] — using individual canonical refs for 6+ characters would consume nearly all ref slots, leaving no room for env/style/sheet refs
2. **Simpler prompts perform better** per [[seedance-simpler-prompts-perform-better]] — Seedance handles group scenes better with simpler ref structure
3. **Ref slot economy** — saves 3-9 ref slots for other critical references (environment, storyboard sheet, key character canonicals)

**How to apply:**

**Scene character count → ref strategy:**

| OG10 Count | Ref Strategy | Example |
|------------|--------------|---------|
| 1 character | Individual canonical ref | `@图片1 = SKET turnaround` |
| 2 characters | 2 individual canonical refs | `@图片1 = HEARTA + @图片2 = LYCHEE` |
| 3 characters | 3 individual canonical refs | `@图片1-3` per character |
| 4-5 characters | Individual canonical refs (still possible within budget) | `@图片1-5` per character + 1-2 env refs |
| **6+ characters** | **ONE consolidated OG10 group lineup ref** | `@图片1 = OG10 6-body-view group ref + @图片2 env + @图片3 sheet` |
| All 10 OG10 | ONE consolidated OG10 group lineup ref | Same as 6+ |

**Group lineup ref:**
- A pre-rendered ensemble image showing 6 or all 10 OG10 in canonical poses + design from front/back/side views
- "6 body view" = group reference showing 6+ OG10 bodies in one composition (front, 3/4, side, back angles can be mixed)
- Lock identity across whole group in one ref slot

**When to break the rule:**
- If a specific OG10 has a HERO MOMENT (close-up, signature action) in a 6+ scene → also attach that hero's individual canonical ref in addition to group ref
- Example: 8 OG10 in scene with CCATS doing signature uppercut → @图片1 = OG10 group + @图片2 = CCATS canonical + @图片3 = env

**Cross-references:**
- [[seedance-9-image-ref-limit]] — hard 9-ref cap
- [[seedance-simpler-prompts-perform-better]] — simpler structure wins
- [[seedance-refs-only-when-needed]] — only include refs actually present in clip
- [[og10-character-canonical-designs]] — individual canonical designs (still ref-anchor source)

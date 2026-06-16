---
name: seedance-9-image-ref-limit
description: "⭐ Seedance 2.0 has a HARD CAP of 9 image refs per prompt. Never write a prompt with 10+ @图片 refs. Always count refs before delivering and prune to 9 max. Locked 2026-06-15."
metadata:
  node_type: memory
  type: feedback
  originSessionId: cda39d5a-a05d-4185-9eca-d3d90e2d35e0
---

**⭐ Rule (locked 2026-06-15):** Seedance 2.0 accepts a MAXIMUM of 9 image references per single prompt. Hard cap. Going over 9 = prompt fails / refs dropped silently.

**Why:** 2026-06-15 — User explicitly said "seedance only can input 9 image < keep this in memory." After delivering Clip 06C-A V2 with 10 refs (Sheet 06C + 8 hero canonicals + Whisper canonical), user confirmed Seedance only accepts up to 9. This is the platform constraint.

**How to apply:**

1. **Always count refs before delivering ANY Seedance prompt.** If count > 9, prune.

2. **Pruning priority order (drop in this order when at limit):**
   - First drop: composition/style anchor sheets (e.g., Sheet 06C) — character canonicals are usually higher value for identity lock
   - Second drop: environment anchors if character canonicals + power-effect already convey env
   - Keep: individual character canonicals when identity drift has been reported
   - Keep: villain/boss canonicals
   - Keep: critical prop/mount canonicals (e.g., paper dragon)

3. **Trade-off awareness:**
   - Character canonical fidelity > composition anchor for identity-critical scenes
   - Composition anchor > individual canonicals when style/blocking matters more than per-character detail
   - If a scene has 8+ heroes, may need to compromise — combine 2-3 heroes into ONE consolidated lineup ref to free a slot

4. **Practical reality:**
   - Even 9 refs can cause Seedance "identification fatigue" — output may drift on some characters
   - 5-7 refs is the practical sweet spot for clean output
   - 8-9 refs only when identity lock is critical (already had drift on previous attempt)

5. **Per-clip ref audit checklist before delivery:**
   - Count refs: ≤ 9? Yes/No
   - Each ref actually used in this clip? Yes/No (drop unused per [[seedance-refs-only-when-needed]])
   - Pruning if over: drop composition/style anchor first

**Cross-references:**
- [[seedance-refs-only-when-needed]] — only include refs actually present in clip
- [[seedance-prompt-char-limit]] — also obey <4000 char limit
- [[higgsfield-always-specify-refs]] — Higgsfield can take more refs; this rule is Seedance-specific
- [[seedance-cinematic-continuity-rules]] — env refs are guides only

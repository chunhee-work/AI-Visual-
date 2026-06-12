---
name: seedance-refs-only-when-needed
description: "⭐ For Seedance video prompts, ONLY include reference images (@图片) that are actually needed for that specific scene/clip. If a character/element doesn't appear in the clip, DO NOT include their reference image — extra unused refs confuse the AI. Saved 2026-06-12."
metadata:
  type: feedback
  node_type: memory
  originSessionId: cda39d5a-a05d-4185-9eca-d3d90e2d35e0
---

**⭐ Rule (locked 2026-06-12):** Every Seedance video prompt MUST only include @图片 reference images that are actually used in that specific clip/scene. If a character or visual element does NOT appear in the clip, DO NOT include their turnaround/reference as @图片. Extra unused references confuse Seedance and lead to:
- Wrong character bleeding into scene
- AI uncertainty about which subject to focus on
- Reduced visual consistency

**Why:** 2026-06-12 — User flagged that including all character refs even when not needed in a clip can confuse Seedance's understanding of which character should appear. Only refs that are needed for the scene = cleaner output.

**How to apply going forward:**

1. **Per-clip ref audit**: Before delivering any Seedance prompt, list which characters/elements appear in the clip, then ONLY include those refs.

2. **Common cases:**
   - Sheet 01 Clip A (Healing + Whisper materializes): CCATS, ECOX, wounded villager, Whisper — include refs for those. NO GST (not yet arrived). NO corrupted villagers (not yet in scene).
   - Sheet 01 Clip B (Heroes see army + Whisper commands): CCATS, ECOX, wounded villager (still at feet), Whisper, corrupted villagers — include refs for those. NO GST yet.
   - Sheet 01 Clip C (CCATS+ECOX faces + GST lightning cavalry): CCATS, ECOX, GST, Whisper (recoiling), corrupted villagers (being struck) — include refs for those. Drop wounded villager (no longer in frame focus).

3. **Standard refs always needed across all clips:**
   - Sheet/storyboard ref (for style + composition anchor)
   - Environment ref if env is critical (e.g., AUREA village)
   - Character turnarounds for ANY character that appears prominently in the clip

4. **Exception**: If a character is hinted at but not visually present (e.g., "ECOX dialogue heard offscreen but not seen"), DO NOT include their ref. Voice is text-driven via Dialogue Cue, not visual.

5. **Cross-character interaction**: If two characters interact, BOTH refs needed. If background characters are present but not focal (e.g., distant survivors), the canonical character ref is still useful for identity lock.

**Anti-pattern to avoid:**
- Including 7 refs "just to be safe" — too many distract the AI
- Including character refs for characters not in this specific clip — AI may bleed them into scene
- Forgetting to include refs for characters actually present — leads to identity drift

**Cross-references:**
- [[higgsfield-prompt-char-limit]] — Higgsfield image gen <15000 char (same principle: cleaner = better)
- [[seedance-prompt-char-limit]] — Seedance video <4000 char
- [[seedance-cinematic-continuity-rules]] — Other Seedance prompt rules
- [[always-invoke-prompt-skills]] — Always use seedance-prompt-library for video

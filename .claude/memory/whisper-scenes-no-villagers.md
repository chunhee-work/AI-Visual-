---
name: whisper-scenes-no-villagers
description: "⭐ Whisper boss-reveal scenes (Whisper as sole subject in AUREA village) must be EMPTY of villagers/NPCs/human figures. Don't write background-figure language even with 'tiny/obscured/hint' qualifiers — Higgsfield renders them visible. Add explicit 'EMPTY village, NO human figures' clause. Saved 2026-06-12."
metadata: 
  node_type: memory
  type: feedback
  originSessionId: cda39d5a-a05d-4185-9eca-d3d90e2d35e0
---

**⭐ Rule (locked 2026-06-12):** When rendering Whisper-alone boss-reveal scenes (Whisper standing in AUREA village as the sole subject), the scene MUST be COMPLETELY EMPTY of any villagers, NPCs, peasants, distant silhouettes, or background human figures. The Whisper has cleared/evacuated the village — no humans remain visible.

**Why:** 2026-06-12 — User flagged that the Whisper MCU close-up boss-reveal render came back with multiple villager silhouettes walking around the lower-edge background of the village street. Caused by prompt language: "A few tiny villager silhouettes hint in deep distance, obscured by haze." Higgsfield rendered them as clearly visible figures DESPITE the qualifiers ("tiny" + "obscured by haze" + "hint in distance" did NOT suppress them). User wants Whisper boss-reveal scenes to be character-isolated — Whisper alone with the village architecture and atmospheric haze.

**How to apply going forward:**

1. **NEVER write background-figure language in Whisper scenes**, even with softening qualifiers:
   - ❌ "tiny villager silhouettes hint in deep distance"
   - ❌ "a few distant villagers obscured by haze"
   - ❌ "small silhouettes barely visible in the background"
   - ❌ "hints of figures in the deep background"
   - All of these → Higgsfield renders visible figures

2. **EXPLICITLY write empty-village language**:
   - ✅ "EMPTY abandoned village street — NO villagers, NO NPCs, NO human figures, NO peasant silhouettes anywhere in the frame"
   - ✅ "The Whisper stands alone — the village is evacuated, every human cleared from view"
   - ✅ "Only the Whisper, the village architecture, and the atmospheric haze — no living figures"

3. **Same principle for ALL character-isolated scenes:**
   - Hero portraits (CCATS solo, ECOX solo, LYCHEE solo, etc.) — explicitly say "no other figures"
   - Env-only plates (just AUREA village, just battlefield, etc.) — explicitly say "no human figures anywhere"
   - Don't add background characters unless they are EXPLICITLY part of the scene brief

4. **Exception**: If the user EXPLICITLY briefs background figures (e.g., "corrupted villagers in foreground silhouette horde" or "wounded villagers in background"), then include them with full canonical signatures locked. Otherwise default to empty.

5. **Anti-pattern (lesson learned):**
   - Higgsfield does NOT honor softening qualifiers like "tiny," "barely visible," "obscured by haze," "hint of" when describing figures. If you describe a figure with words at all, Higgsfield will render it visibly.
   - The only safe way to NOT have figures is to NOT describe them, AND to explicitly say "NO figures."

**Cross-references:**
- [[higgsfield-is-tool-not-agent]] — Higgsfield interprets visual descriptions literally, doesn't understand context
- [[strict-storyboard-fidelity]] — don't add narrative beats/elements not in user's brief
- [[strict-turnaround-fidelity]] — don't add character elements not in attached turnaround
- [[the-first-whisper-boss-villain]] — Whisper canonical design lock
- [[higgsfield-always-specify-refs]] — always specify refs explicitly

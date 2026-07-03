---
name: bilingual-mandarin-responses
description: "⭐⭐⭐ MOVING FORWARD ALL chat text in Mandarin ONLY (no mixed English analysis). Prompts=EN code block. MUST include ONE Mandarin sentence summary above every prompt. AskUserQuestion tool questions + options ALSO in Mandarin. User re-reinforced 2026-07-01."
metadata:
  node_type: memory
  type: feedback
  originSessionId: cda39d5a-a05d-4185-9eca-d3d90e2d35e0
---

**⭐⭐⭐ Rule (re-reinforced 2026-07-01):** ALL chat wrapper text in Mandarin ONLY. NO mixed English analysis sections. Prompts stay in English code block. AskUserQuestion tool questions + options MUST be in Mandarin as well.

**Why:** User re-reinforced 2026-07-01: "remember use mandarin as main language and always ask me question with mandarin as well". Previous drift into English analysis sections + English AskUserQuestion was a violation.

**How to apply:**

**Chat wrapper (ALL Mandarin):**
- ✅ Summary sentence above prompts — Mandarin
- ✅ Analysis / explanation after prompts — Mandarin
- ✅ Tables / bullet lists — Mandarin (except technical terms like refs, timing, filenames)
- ✅ Section headers — Mandarin (with English tech markers like "Scene 1" OK)
- ❌ NEVER long English analysis paragraphs
- ❌ NEVER mixed English wrapper (only tech terms in English inline OK)

**AskUserQuestion tool:**
- ✅ Question text — Mandarin
- ✅ Option labels — Mandarin
- ✅ Option descriptions — Mandarin
- ✅ Headers — can be shorter Mandarin labels
- ❌ NEVER English AskUserQuestion

**Prompt code blocks (ENGLISH ONLY — unchanged):**
- ✅ Prompt body content — English (Higgsfield + Seedance require English)
- ✅ Ref labels — English (@Image1 per [[ref-labels-english-image-format]])
- ✅ Dialogue lines — English (per [[seedance-dialogue-english-only]])

**Exception zones (English tech OK inline):**
- File paths, filenames
- Higgsfield / Seedance / MCP tool names
- Ref labels @Image1 / @Image2
- Character/canonical names (CCATS, GST, HEARTA, etc.)
- Style block terms (Pixar/Disney/Puss in Boots etc.)

**Cross-references:**
- [[ref-labels-english-image-format]] — English @Image labels rule (unchanged)
- [[use-image-suite-and-seedance-suite-routers]] — Router rule layer
- [[seedance-dialogue-english-only]] — Video dialogue English rule

---
name: ref-labels-english-image-format
description: "⭐⭐ MOVING FORWARD all reference labels in prompts use English @Image1 / @Image2 / @Image3 format — NOT Chinese @图片1 / @图片2 / @图片3. Applies to Higgsfield image prompts AND Seedance video prompts. User directive 2026-06-25."
metadata:
  node_type: memory
  type: feedback
  originSessionId: cda39d5a-a05d-4185-9eca-d3d90e2d35e0
---

**⭐⭐ Rule (locked 2026-06-25):** All reference image labels in prompts MUST use English `@Image1` / `@Image2` / `@Image3` format, NEVER Chinese `@图片1` / `@图片2` / `@图片3`.

**Why:** User directive 2026-06-25: "moving forward use @Image, don't use @图片2, all in english". Cleaner mixed-language workflow — keeps prompt code blocks fully English (per [[bilingual-mandarin-responses]] rule that prompt body is English only). Mandarin chat wrapper still applies AROUND the code block.

**How to apply:**

In EVERY prompt code block (Higgsfield image + Seedance video), reference image labels MUST be:
- ✅ `@Image1`, `@Image2`, `@Image3`, `@Image4`, etc.
- ❌ NEVER `@图片1`, `@图片2`, `@图片3`, etc.

In the References block at the end of prompts:
- ✅ `@Image1 = description of what this reference locks`
- ❌ `@图片1 = description...`

In the prose body of prompts referring to refs:
- ✅ "Dragon character locked from @Image2..."
- ❌ "Dragon character locked from @图片2..."

**Sequential numbering:** Still no gaps. @Image1, @Image2, @Image3 in order.

**Mandarin chat wrapper UNCHANGED:** Per [[bilingual-mandarin-responses]] — Mandarin discussion wrapper + one Mandarin sentence summary above each EN prompt code block still apply. Only the ref labels INSIDE the prompt change from @图片 to @Image.

**Cross-references:**
- [[higgsfield-always-specify-refs]] — refs rule (update @图片 mentions to @Image)
- [[seedance-refs-only-when-needed]] — ref audit rule (update @图片 mentions to @Image)
- [[bilingual-mandarin-responses]] — Mandarin chat + EN prompt code block rule (unchanged)
- [[use-image-suite-and-seedance-suite-routers]] — router rule layer

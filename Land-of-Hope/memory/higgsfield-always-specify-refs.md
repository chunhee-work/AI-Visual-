---
name: higgsfield-always-specify-refs
description: "⭐ When delivering any Higgsfield image prompt, ALWAYS explicitly list what image references the user needs to attach as @图片1/@图片2/etc., with a one-line description of what each ref locks (identity / env / camera / composition / etc.). Don't assume the user knows. Saved 2026-06-12."
metadata: 
  node_type: memory
  type: feedback
  originSessionId: cda39d5a-a05d-4185-9eca-d3d90e2d35e0
---

**⭐ Rule (locked 2026-06-12):** Every Higgsfield image prompt (GPT Image 2, Soul Cinema, Banana Pro, etc.) MUST be delivered with an explicit `References needed` block telling the user exactly which images to attach in slot order — @图片1, @图片2, @图片3, etc. — plus a one-line note on what each ref locks.

**Why:** 2026-06-12 — User explicitly asked: "always tell me what image reference i need to provide for higgsfield." User runs the Higgsfield UI manually and needs to know exactly which canonical assets / previous renders / env plates to drag into each ref slot. Without this list they have to guess, which leads to wrong assets attached → bad renders.

**How to apply going forward:**

1. **Every Higgsfield prompt I deliver MUST end with a `References needed` block** — either a table or a clean numbered list. No exceptions.

2. **Format:**
   ```
   References needed:
   - @图片1 = [what file/asset/render] — locks [identity / env / camera / composition / style]
   - @图片2 = [what file/asset/render] — locks [...]
   - @图片3 = [what file/asset/render] — locks [...]
   ```

3. **For each ref describe:**
   - WHAT the user should attach (be specific — "ECOX canonical turnaround", "previous Sheet 01 render", "burning village env plate", "the 4-corrupted-villagers reference")
   - WHAT it locks (identity / wardrobe / camera angle / framing / lighting palette / env / composition continuity)

4. **Sequential numbering, no gaps** — Higgsfield UI slots are @图片1, 2, 3, 4, 5... in the order user attaches. Don't skip numbers (no @图片1, 3, 5).

5. **Per-prompt ref audit** — only include refs actually needed for THAT specific scene. (Same principle as [[seedance-refs-only-when-needed]] but for image gen.)

6. **If a ref is canonical and reusable** (e.g. character turnaround, env plate), label it as such so user knows to grab from their canonical asset folder.

7. **If a ref is a previous render in this same project flow** (e.g. "previous Whisper MCU close-up for camera continuity"), call that out too.

**Examples of good ref lists:**

```
References needed:
- @图片1 = CCATS canonical turnaround — locks CCATS identity (ginger tabby anthropomorphic cat) + brass steampunk gear
- @图片2 = ECOX canonical turnaround — locks ECOX identity (chibi astronaut medic + teal helmet face-glow + red cross symbols)
- @图片3 = Whisper V3 turnaround — locks Whisper canonical design (smoke S-curve + lava-cores + claw-hand tendrils + no face)
- @图片4 = AUREA village env plate — locks burning-village background + lighting palette + cobblestone street + lava-cracks
```

**Cross-references:**
- [[seedance-refs-only-when-needed]] — same principle for Seedance video prompts
- [[higgsfield-prompt-char-limit]] — Higgsfield <15000 char hard limit
- [[higgsfield-is-tool-not-agent]] — strip project labels in prompt body, pure visual description
- [[strict-turnaround-fidelity]] — don't invent character elements not in attached turnaround

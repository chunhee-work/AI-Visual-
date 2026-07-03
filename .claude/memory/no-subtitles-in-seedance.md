---
name: no-subtitles-in-seedance
description: "User mandate 2026-06-08 — NO subtitles burned into Seedance video output, ever. Drop the 'Subtitle:' line from Dialogue Cue blocks in all Seedance prompts. Lip-sync still uses Dialogue Cue + spoken line for mouth-shape timing, but the rendered video must have NO text subtitle overlay."
metadata:
  node_type: memory
  type: feedback
  originSessionId: cda39d5a-a05d-4185-9eca-d3d90e2d35e0
---

**Rule (locked 2026-06-08):** Seedance video output must have NO subtitle/caption text burned in.

**Why:** User explicit directive 2026-06-08: "i dont want any subtille in the video". The trailer is a cinematic piece — subtitles would break immersion. Subtitles, if any, get added in post-production with the user's chosen styling, not baked into Seedance output.

## How to apply

When writing Seedance prompts:

1. **KEEP** the Dialogue Cue line (gives Seedance the spoken text for lip-sync timing):
   ```
   ⭐ Dialogue Cue: GST speaks "Are you okay?" (3 short syllables, warm gentle skater-kid tone). Lip-sync precisely 3-syllable cadence.
   ```

2. **DROP** the Subtitle line that the seedance-prompt-library skill anatomy suggests. Do NOT write:
   ```
   Subtitle: "Are you okay?"  ← REMOVE THIS LINE
   ```

3. **ADD** an explicit no-subtitle constraint to the constraints block:
   ```
   ⭐ NO SUBTITLES burned into the video output — clean visuals only, no caption overlay anywhere.
   ```

4. The "NO TEXT on screen" constraint already implies this but it doesn't hurt to be explicit — Seedance has been known to render subtitle text by default for dialogue cues.

## Cross-references

- [[chill-farm-character-voices]] — Plan B post-dub workflow still applies
- [[seedance-prompt-char-limit]] — 4000-char limit
- [[always-invoke-prompt-skills]] — seedance-prompt-library skill mandate still applies, but override its subtitle convention
- [[strict-storyboard-fidelity]] — user-stated rules override skill defaults

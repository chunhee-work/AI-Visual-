---
name: seedance-prompt-char-limit
description: "Seedance 2.0 prompts capped at 4000 characters total. FILL the budget — write as detailed/rich as possible up to ~3800, hard ceiling 4000. Preserve timestamps, reference anchors, signature transitions, no-hard-cuts rule."
metadata:
  node_type: memory
  type: feedback
  originSessionId: cda39d5a-a05d-4185-9eca-d3d90e2d35e0
---

User directed (2026-05-29): initially **"compree to 3000 charcter, always dont provide seedance prompt over 3000 charcter, keep this is mind"** → then loosened to **"make sure the seedance prompt is under 4000 character will do"**.

**UPDATE 2026-06-23:** ceiling is **4000 characters**, AND the user wants prompts written **as detailed and rich as possible up to that limit** (don't under-write — fill the budget with vivid shot detail). Target ~3800, hard ceiling 4000.

**The rule:** Every Seedance 2.0 video prompt I deliver must be **under 4000 characters total**. Hard ceiling — not aspirational. Use the room for MORE detail, not less. Bilingual EN + 中文 wrappers still apply around the prompt, but each prompt body (EN version, 中文 version) is independently capped at 4000.

**Why:** Seedance 2.0 has a prompt input limit on the platform. Anything over 4000 chars overflows / truncates / won't paste cleanly. The user has experienced this — initial guidance was 3000 (cautious) but 4000 is the actual practical ceiling that gives more room while staying safe.

**How to apply:**
1. **Before delivering any Seedance prompt:** check length. If verbose, compress.
2. **Compression techniques (in order of preference):**
   - Cut redundant adjectives (don't say "smooth, fluid, flowing" — pick one)
   - Combine related sentences into one line
   - Drop the "—" connector clauses (use periods)
   - Remove decorative emphasis (lose **bold** in prompt body, keep only for critical NO-rules)
   - Use ASCII arrows `→` for sequential beats
   - Strip articles where readable ("Camera pushes in" vs "The camera continues its push-in")
   - Shorten timestamps to `[00:00-00:02]` not `[00:00 — 00:02]`
   - Use abbreviations sparingly but acceptable: VFX, DOF, ECU, ~50mm
   - Drop bilingual delivery for the prompt body itself — Seedance accepts EN or 中文 but not both stacked; deliver ONE language version (the language the user pasted in). The user-facing wrapper around the prompt can still be bilingual per [[bilingual-mandarin-responses]].
3. **What to PRESERVE even when compressing:**
   - Every timestamp `[HH:MM-HH:MM]`
   - Every reference anchor `@图片1` / `@图片2` / etc.
   - The "NO hard cuts" / "seamless morph" rule (if applicable to the shot)
   - Identity / character consistency clause
   - Signature transition moments (iris dilation, planet reveal, etc.)
   - Audio block (compressed but present)
   - Color / atmosphere through-line
   - Render quality note
4. **Target:** aim for ~3800 chars to give buffer. Hard ceiling 4000.
5. **After compressing:** state the char count to the user so they can verify, e.g. "Compressed to ~3850 chars."

**Cross-references:**
- [[land-of-hope-trailer]] — the project this serves
- [[land-of-hope-locked-visual-style]] — locked style (this rule overrides the long prose style block IN Seedance prompts; reference image attachments carry the style anchor instead, so the prompt body doesn't need the full LOCKED-STYLE block)
- [[bilingual-mandarin-responses]] — still bilingual in the WRAPPER, but the prompt body itself is one language
- [[higgsfield-is-tool-not-agent]] — Higgsfield/GPT Image 2 rule for image prompts (different platform, different rule, different char tolerance)

**Note:** This rule applies ONLY to Seedance prompts. GPT Image 2 / Higgsfield image prompts can run longer (no equivalent hard char limit user has hit). Don't compress image prompts aggressively unless asked.

---
name: strict-storyboard-fidelity
description: "When writing scene prompts (image or Seedance video), describe ONLY what is in the user's brief or the locked storyboard. NEVER invent narrative beats, visual details, transformation sequences, or 'cool' embellishments not specified. Saved 2026-06-08 after I fabricated an entire purification sequence (red-eye fade + chi dissolves into golden sparkles + peaceful unconscious slump) for the GST mother+daughter rescue scene when the user's brief only said 'Shocked and thrown the men'."
metadata:
  node_type: memory
  type: feedback
  originSessionId: cda39d5a-a05d-4185-9eca-d3d90e2d35e0
---

**Rule:** Prompts MUST describe ONLY what the user briefed or the locked storyboard specifies. NO invented narrative beats, NO fabricated visual sequences, NO "cool" additions to enhance the scene.

**Why:** 2026-06-08 — for the GST rescue scene, user's brief said simply "Shocked and thrown the men" (electric shock + knock back per the storyboard's NEVER-KILL = disarm + knock back rule). I expanded this into an entire 1.5-second fabricated purification sequence: red-glowing eyes fade to normal human eyes, dark-red corruption chi dissolves into golden-white sparkles drifting upward, twisted grin softens to peaceful neutral, body slumps to knees and lies softly on cobblestone in peaceful unconscious state. NONE of this was in the brief or the storyboard. User flagged it: "净化(NOT KILLING:红眼褪去+腐化chi散成金色sparkles+腐化者peaceful slumps down) there's no this one pls do not add in yourself check the storyboard and do not add in something that is not in the storyboard". This is the same failure mode as [[strict-turnaround-fidelity]] (inventing character elements not in the turnaround sheet) but at the scene/narrative level instead of the character-design level.

**How to apply:**

1. **Before writing any scene description**, identify what is locked:
   - User's current brief (the exact action/beats they described in this turn)
   - Storyboard scene description (in `land-of-hope-trailer.md` for Land of Hope scenes)
   - Any prior scene specs in `Land-of-Hope/og10-hero-scenes/*.md`

2. **What's NOT in the brief or storyboard = NOT in the prompt.** Don't add:
   - Transformation sequences (red-eye fade, chi dissolves, glow effects) unless specified
   - "Cool" visual flourishes (sparkles, particle effects, secondary glows) unless specified
   - Narrative beats (purification, redemption, peaceful aftermath) unless specified
   - Character state changes (unconsciousness, peaceful sleep, expressions softening) unless specified
   - Emotional moments beyond what's described
   - Sound design elements that imply narrative (healing chimes, redemption music) unless specified

3. **Translate brief LITERALLY into prompt language**:
   - "Shocked and thrown" → electric shock + knock-back motion. STOP. Don't add what happens to the villager afterward unless asked.
   - "Eyes snap open" → eyes snap open. Don't add what they see, what they think, what they do next.
   - "Camera pans right" → camera pans right. Don't add a new subject revealed at the end of the pan unless specified.

4. **Reaction beats user EXPLICITLY asks me to design** are OK to develop creatively — those are explicitly delegated. Example: "help me with how should they reaction" = creative license to design the reaction. But the rescue action itself was NOT delegated — it was specified.

5. **When unsure** whether a beat is in the brief, ASK the user before writing the prompt. "Does the purification show the villager getting healed visibly, or just thrown back and gone off-frame?" — don't guess.

6. **Storyboard NEVER-KILL rule** (per `land-of-hope-trailer.md`): enemies are corrupted villagers, every blow DISARMS and KNOCKS BACK, never kills or maims. This is the LIMIT on violence, NOT a license to add "purification" visual sequences. Knocked back = knocked back. The villager exits the frame or lies stunned. No glowing transformation unless storyboard specifies.

7. **Same fabrication temptation as [[strict-turnaround-fidelity]]** — the urge to add "cool" details to enhance the moment. RESIST. The user briefed what they want. Trust the brief.

## Examples of what I fabricated (DO NOT ADD without spec)

- Red-glowing eyes fading to normal human eyes during shock
- Dark-red corruption chi dissolving into golden-white sparkles drifting upward
- Twisted predatory grin softening into peaceful neutral expression
- Body slumping to knees then lying softly in peaceful unconscious state
- "NOT dead, just peacefully sleeping, chest still gently rising" framing
- Soft healing chime SFX
- Drifting golden sparkles in background of subsequent shots

## Cross-references

- [[strict-turnaround-fidelity]] — same anti-fabrication rule applied to character design (don't add goggles/hats not in turnaround). This new memory is the scene-level equivalent.
- [[land-of-hope-trailer]] — storyboard source-of-truth, including NEVER-KILL rule (disarm + knock back only)
- [[land-of-hope-character-designs]] — character canon

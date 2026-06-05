---
name: seedance-duration-minimum
description: Seedance 2.0 has a LOWER LIMIT of 4 seconds per video clip — any clip shorter than 4s will be rejected. Always ensure every Seedance prompt duration is >= 4s. Updated 2026-06-04.
metadata: 
  node_type: memory
  type: feedback
  originSessionId: cda39d5a-a05d-4185-9eca-d3d90e2d35e0
---

User directed (2026-06-04): **"the low limit is 4 sec for seedance"**

**The rule:** Every Seedance 2.0 video clip MUST be at least 4 seconds long. This is the platform's lower duration floor. Clips shorter than 4 seconds will not generate / be rejected.

**Why:** Seedance 2.0 has a minimum duration constraint on the platform. The user has hit this when shorter clips (2s, 3s) didn't deliver as expected. 4 seconds is the actual floor — no clips under that.

**How to apply:**
1. **Before delivering any Seedance prompt:** check the duration. If under 4s, extend.
2. **How to extend brief beats to 4s without padding feel:**
   - Add an opening setup/establishing beat (0.5–1s before the main action)
   - Slow down the main action (use slow-motion or a brief hold)
   - Add a hold/lingering frame after the main action (0.5–1s)
   - Insert a secondary natural beat that flows (e.g., camera continues to move after the action, or the action has a recoil/aftermath)
3. **Combination clips:** When user wants multiple beats in one clip (e.g., assault + push-in to close-up), naturally fitting 2–3 connected beats per clip helps reach 4s easily without padding.
4. **Upper end:** Seedance 2.0 still supports longer clips up to 10–12s for narrative scenes. The 4s is just the floor, not the ceiling.
5. **When the user asks for shorter clips (e.g., "2 second clip"):** quietly bump to 4s and explain in the chat wrapper why. Don't deliver an under-4s prompt that won't work on the platform.

**Cross-references:**
- [[seedance-prompt-char-limit]] — Seedance prompts capped at 4000 chars (the other Seedance technical constraint)
- [[land-of-hope-trailer]] — the project this serves
- [[bilingual-mandarin-responses]] — bilingual EN+CN delivery still applies

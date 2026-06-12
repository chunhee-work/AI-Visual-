---
name: strict-turnaround-fidelity
description: "When generating image prompts with @图片1 = character turnaround as ID ref, describe ONLY what is visible in the turnaround. NEVER invent, add, or embellish character elements (goggles, hats, accessories, masks, weapons, jewelry, tattoos) that aren't in the reference sheet. Saved 2026-06-08 after CCATS V3 prompt fabricated steampunk goggles not in turnaround."
metadata: 
  node_type: memory
  type: feedback
  originSessionId: cda39d5a-a05d-4185-9eca-d3d90e2d35e0
---

**Rule:** When a character turnaround sheet is provided as `@图片1` identity reference, the prompt MUST describe ONLY what is visible in that turnaround. NO invented elements.

**Why:** 2026-06-08 — I wrote CCATS V3 close-up prompt with "Brass-rimmed steampunk goggles pulled DOWN over his eyes" — but CCATS turnaround has NO goggles. User flagged it: "CCAts dont have glasses pls follow @图片1 exactly do not add one something with @图片1 dont have". The fabrication broke character identity. This is a recurring temptation when writing dramatic close-ups — I want to add "cool" elements (goggles, scarves, headbands, scars) to enhance the hero shot, but those embellishments contradict the locked character design.

**How to apply:**

1. **Before writing any character description in a prompt**, mentally list what IS in the turnaround:
   - Hair (color, length, style)
   - Face (eyes, expression markers visible in the sheet)
   - Headwear / eyewear (ONLY if shown in turnaround — if not shown, NONE)
   - Top garment (fabric, color, structural details)
   - Bottom garment
   - Footwear
   - Belt / sash / accessories
   - Weapons (the specific ones shown)
   - Body markers (tattoos, scars, fur patterns — only if shown)

2. **What's NOT in the turnaround = NOT in the prompt.** Don't add:
   - Goggles / glasses / eyewear (unless shown in turnaround)
   - Hats / caps / headbands (unless shown in turnaround)
   - Masks (unless shown in turnaround)
   - Extra jewelry / accessories (unless shown in turnaround)
   - Scars / tattoos / face markings (unless shown in turnaround)
   - Cool gadgets / utility belts beyond what's shown
   - Capes / scarves / extra layered clothing not in the sheet

3. **For dramatic close-ups especially**, RESIST the temptation to add "cool" face accessories to enhance the hero look. The face being fully uncovered IS the hero look when the turnaround shows it uncovered.

4. **Explicit prompt clause for close-ups**: Add a clause like:
   > ⭐ STRICT IDENTITY — match @图片1 turnaround exactly. DO NOT invent or add any element not in the turnaround. [List specifically what is NOT to be added based on character: "NO goggles, NO hat, NO mask, face fully uncovered" or whatever applies].

5. **If unsure** whether something is in the turnaround, ASK the user before writing the prompt — don't guess. "Does [character] have [element X] in their turnaround?"

## Specifically known character compositions (snapshot 2026-06-08)

- **CCATS** (UPDATED 2026-06-09 per new turnaround): chubby rotund orange tabby cat + amber-gold eyes + **BROWN LEATHER PEAKED ENGINEER'S CAP with small brass coffee-bean medallion on the front** (correction — previous memory said "NO hat" which was wrong) + white button-up collared shirt with rolled sleeves + dark grey tie + cream/off-white leather apron (apron has subtle paw-print + coffee-bean stitch detail; if any "CCATS" text appears, LEAVE BLANK per project label rule) + brass shoulder armor pieces + brass-armored gauntlets on both fists + brown leather harness straps + brown leather belt + dark grey/brown trousers + brass-toed leather boots + tall brass steampunk boiler backpack with two vertical chimney pipes venting white steam, brass valves, gauges, pressure dials, glowing orange embers through grate, leather harness. **NO goggles. NO eyewear.** Face uncovered except for the cap brim. Hospitable warm uncle energy.
- **GST**: young boy skater + black leather jacket (back is PLAIN BLACK LEATHER) + dark hoodie + black backward baseball cap + dark cargo pants + black sneakers with white sole stripes + wooden skateboard with yellow urethane wheels + blue-white lightning powers. **NO gold crown emblem on jacket back. NO logo/patch/embroidery on jacket. Jacket back is CLEAN UNMARKED black leather. Signature back-view hero element = the BLUE-WHITE LIGHTNING from his hand, NOT a logo.** Flagged 2026-06-08 after I fabricated "gold crown emblem on back" for V1 and V3 prompts.
- (Add other character anti-fabrication notes here as they come up.)

## Cross-references

- [[higgsfield-is-tool-not-agent]] — different rule (about not using project labels)
- [[gpt-image-prompt-format]] — prose format
- [[land-of-hope-locked-visual-style]] — style block (doesn't override identity)
- [[land-of-hope-character-designs]] — character design source-of-truth

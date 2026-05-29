---
name: higgsfield-is-tool-not-agent
description: "Higgsfield (GPT Image 2 image generator) is a TOOL, not an AI agent — it doesn't understand project-specific labels or named entities. Strip all project names from prompts and use pure visual description only."
metadata: 
  node_type: memory
  type: feedback
  originSessionId: cda39d5a-a05d-4185-9eca-d3d90e2d35e0
---

User explicitly clarified (2026-05-28): **"im using higgfield it not a AI agent, so it wont understand your prompt with B2, AUREA. this can be remove"**

**The rule:** Higgsfield (running GPT Image 2 under the hood) is a stateless image generation tool, NOT an agent that knows the project's lore, characters, or label conventions. It only understands:
- Pure visual description (what the eye sees)
- Reference images attached in the UI ("the attached image")
- Generic style/lighting/camera instructions

**STRIP from all prompts going forward — these mean nothing to Higgsfield:**
- ❌ Project labels: `B1`, `B2`, `B3`, `B4`, `S1`, `S7`, `B2.1`, `v9`, etc.
- ❌ World names: `AUREA`, `AUREA homeworld`, `AUREA village`, `Land of Hope`, `The Chill Farm`, `Gacha`
- ❌ Character group names: `OG10`, `OG10 warrior orders`, `the 10`, character codenames `CCATS`, `GST`, `SKET`, `FROAK`, `FOT`, `ZEYO`, `KETDONUT`, `LYCHEE`, `HEARTA`, `ECOX`, `WICK` *(except when they're literal brand text painted on a sign in the scene — then they're fine because they're describing visible text)*
- ❌ Lore names: `Crystal of Value`, `TON crystal`, `Fountain of Life`, `The Whisper`, `Old Keeper`
- ❌ Reference labels: `locked-style reference`, `the B2 reference`, `the v9 result` → just say `the attached reference image`
- ❌ Standard names: `LOCKED Land of Hope visual standard` at the start of the locked block → simplify to `Render as a clean cinematic frame...`

**KEEP — these are pure visual:**
- ✅ Visual descriptions: "a steampunk-armored ginger tabby cat warrior", "a small multi-faceted clear glowing crystal", "a circular tiered stone fountain"
- ✅ "the attached reference image" / "the attached image" (generic)
- ✅ Style instructions: "Pixar/Disney/DreamWorks register", "painterly stylized-but-realistic", "real flawed weathered skin", etc.
- ✅ Camera/lighting language: "elevated three-quarter perspective", "soft natural daylight", "cool-balanced palette", etc.
- ✅ Brand text shown on signs/clothing/etc. IF it appears visibly in the scene: "a hand-painted wooden sign with 'CCATS' in cursive" — this is fine because the model is rendering visible text on a sign, not parsing project labels

**Updated [+LOCKED-STYLE] block start (drop the "LOCKED Land of Hope visual standard" framing):**

Old: *"Render in the LOCKED Land of Hope visual standard — a clean cinematic frame from a high-end 3D animated feature..."*

New: *"Render as a clean cinematic frame from a high-end 3D animated feature in the Pixar/Disney/DreamWorks register..."*

Then the rest of the block continues verbatim (skin/lighting/color/camera — all pure visual).

**How to phrase scene context without project labels:**
- "AUREA village" → "a fantasy alien village" or just describe the architecture
- "AUREA homeworld" → "an extraterrestrial homeworld" or "an alien planet"
- "the OG10 warriors" → describe them visually or say "fantasy warrior characters"
- "Crystal of Value at the fountain's center" → "a small multi-faceted clear glowing crystal floating at the fountain's center"
- "the Fountain of Life" → "a magical circular tiered stone fountain"
- "B2 reference for AUREA village" → "the attached reference image for the village architecture and composition"

Per [[gpt-image-prompt-format]]: keep prose, no keyword piles. Per [[land-of-hope-locked-visual-style]]: locked style block still mandatory but with the project-name framing stripped from its opening line.

Apply this rule retroactively when re-issuing any old prompt and prospectively to every new prompt for the trailer.

---
name: seedance-cinematic-continuity-rules
description: "User mandate 2026-06-09 — Seedance video workflow rules for smooth cinematic continuity. Storyboard sheet = style ref but each long sequence splits into multiple focused short clips (3-5s) with gap-filling in-between motion beats. Environment refs are guides only, not strict matches. Always pre-prompt check gap-filling additions before delivering."
metadata:
  node_type: memory
  type: feedback
  originSessionId: cda39d5a-a05d-4185-9eca-d3d90e2d35e0
---

**Rule (locked 2026-06-09):** Seedance 2.0 struggles with 6+ different camera moves in one 10-12s prompt — output reads choppy/discontinuous. Standard workflow now splits long cinematic sequences into multiple focused short clips with smooth in-between motion, then edits together in post for "one-take" cinematic feel via hidden cuts.

**Why:** 2026-06-09 — user feedback after Sheet 1 + Sheet 2 single-prompt 10-12s deliveries: "我的视频出来的效果连接性不好动作不流畅" (output continuity bad, motion not smooth). User confirmed split approach (方案A) is the path forward, and added 4 specific clarifications.

## The 4 locked rules

### 1. Split long sequences into multiple focused short clips

Each Seedance clip should be **3-5 seconds covering 1-2 storyboard panels max**, with a SINGLE primary continuous camera move per clip. NOT 6 different camera moves in 10s.

- 1 storyboard sheet (6 panels) → typically 2-3 Seedance clips
- Each clip is a focused "cinematic beat" with clear start → middle → end
- Edit clips together in post for hidden-cut "one-take" feel (the technique used in Children of Men, 1917, Birdman long takes)
- This significantly improves motion smoothness and character identity consistency

### 2. Storyboard sheet stays as @图片1 style reference

When user provides a rendered storyboard sheet, KEEP attaching it as @图片1 for style/composition/lighting register guide. Seedance reads it as visual style anchor.

- Do NOT skip the storyboard sheet ref
- It guides painterly Pixar register + chiaroscuro lighting + warm amber palette + atmospheric haze across all clips
- Identity refs (@图片2, @图片3) still strict for character lock

### 3. Fill in the gaps with smooth cinematic in-between motion

Storyboard sheets show 6 discrete moments — but cinematic video needs the BETWEEN-PANEL motion to be fluid. When writing each clip prompt:

- **Identify the gaps** between panels (what's not shown in the static storyboard but needs to happen in motion)
- **Add bridging beats** — camera transitions, body wind-ups, secondary motion, ambient action, motivated pans
- **Treat the storyboard as keyframes**, the in-between is the animation
- **Smooth motion vector continuity**: if panel ends with camera at 30°, next panel starts ~35-40° NOT 90° — describe the bridge

Examples of gap-filling:
- Between aerial → descent: "camera tilts down + accelerates + smoke begins to swirl into frame from edges"
- Between street push-in → whip-pan: "magical adversary at frame center continues advancing as camera detects movement in periphery → motivated whip-pan LEFT toward doorway"
- Between silhouette reveal → uppercut: "hero's tail flicks + body coils + cap brim tilts forward + he lunges from doorway into action wind-up → contact"

### 4. Environment reference = guide, not strict match

User mandate: "for all the environment i provide does not need to follow exactly the same, it's just a guide. seedance can generate with the reference to a new environment using the reference."

- @图片3 (or whichever env ref) provides ATMOSPHERE + PALETTE + MATERIAL register + KEY ELEMENTS (cobblestone, lava-cracks, thatched cottages, fire glow, twin moons)
- Seedance can VARY composition, scale, specific cottage layouts, brazier placement — these are creative latitude
- Do NOT write "match @图片3 exactly" — write "AUREA-style cobblestone village environment per @图片3 style register"

## Pre-prompt check requirement for gap-filling

User mandate: "if u feel it can be better feel free to adjust or add in scene. but before that ask me firts."

Before delivering Seedance prompts, ALWAYS present a pre-prompt check showing:

- Each proposed clip number + duration + primary camera move
- Which original storyboard panels each clip covers
- ⭐ The gap-filling additions / in-between motion beats I'm proposing
- Strategic dialogue moments (per [[chill-farm-character-voices]] Plan A)
- Any scene additions/adjustments I'm proposing for cinematic enhancement

Wait for user's green light before writing the prompts.

Skip the pre-prompt check ONLY for:
- Minor iteration on a just-approved clip (composition tweak, dialogue swap, lighting nudge)
- User explicitly says "just write it" / "skip check"

## How to apply on a typical 6-panel storyboard sheet

1. **Group panels into focused beats** — usually 2-3 beats per sheet (e.g. setup beat / threat beat / hero action beat)
2. **Map each beat → one Seedance clip** of 3-5 seconds
3. **For each clip, list the gap-filling motion** the prompt will add to make it smooth
4. **Pre-prompt check** the full split plan with the user
5. **After approval, write each clip's full Seedance prompt** following the locked anatomy

## ⚠️ KEY ACTION marker rule (locked 2026-06-09)

**User mandate 2026-06-09:** When the clip contains a fight or significant movement scene (combat impact, slash, kick, jump, sprint, uppercut, dramatic camera arc), add an explicit `⚠️ KEY ACTION —` callout block in the Seedance prompt describing the primary motion beat that must be executed cleanly.

**Purpose:** Focuses Seedance's motion-priority on the critical action so it doesn't blur or rush the key beat. Treats the KEY ACTION as the hero motion of the clip.

**Format:**
```
⚠️ KEY ACTION — [description of the primary fight/movement beat]. [The single continuous motion from start → middle → end]. [Speed pattern if relevant: slow start → fast peak → smooth follow-through]. [What must NOT be cut/blurred].
```

**Examples:**
- Combat: `⚠️ KEY ACTION — samurai cat executes iaijutsu draw → diagonal slash → adversary hurled back. ALL THREE beats happen in one fluid motion. Slow wind-up → explosive cut → smooth follow-through. Do NOT cut between draw and slash.`
- Camera movement: `⚠️ KEY ACTION — continuous CAMERA DESCENT from aerial drone through smoke down to cobblestone ground level. ONE continuous arc with NO CUTS — drone → tilt → acceleration → plunge through smoke → smooth horizontal recovery. Smoke transition softens any micro-jumps.`
- Jump/kick: `⚠️ KEY ACTION — frog kung-fu master rooftop leap → mid-air rotation → side kick → knocked-back adversary → horse stance landing. Full descending arc captured in single continuous tracking shot.`

When to use:
- ✅ Combat impact clips (uppercut, slash, kick)
- ✅ Long camera moves (crane up/down, lateral track, push-in)
- ✅ Hero arrivals with movement (leap, slide, lunge)
- ✅ Aftermath motion (knocked-back trajectory, body settling, debris falling)
- ❌ Static dialog scenes (no marker needed)
- ❌ Quiet reveal moments without movement

## Refs label requirement (locked 2026-06-09)

User mandate 2026-06-09: "when u provide the prompt pls give this, so i know what i need to provided to seedance."

**Rule:** Every Seedance prompt delivery MUST include a clearly labeled refs list ABOVE the code block, in this format:

```
**[Clip name] Refs:**
- @图片1 = [description of what this image is]
- @图片2 = [description]
- @图片3 = [description]
- @图片4 = [description]

(共N张refs,按编号顺序attach到Seedance UI)
```

**Why:** User attaches refs into Seedance UI in numbered slots. Without a clear label list, user doesn't know what to attach to which slot — leads to drift / wrong refs attached / character identity errors.

**Format details:**
- Use Mandarin "Refs:" label or "Refs:" — keep consistent with bilingual format
- List each @图片N with concrete description of source image (e.g. "Sheet 2 rendered storyboard" / "CCATS turnaround" / "Image A magical adversary")
- State total count at bottom
- Place this label BEFORE the code block, not inside the code block
- Also keep the refs description at the END of the code block (as already standard) — both serve different purposes (one is for user's attachment workflow, other is for Seedance's prompt parsing)

## Dialogue policy on action sequences (refined 2026-06-09)

User feedback 2026-06-09 on Sheet 1 + Sheet 2 dialogue proposals: "i dont feel like this is necessary."

**Refined rule:** Pure fight / combat / chase / pure camera-movement sequences → DEFAULT TO NO DIALOGUE. Strategic dialogue applies only when there's a quiet beat, character introduction, or emotional moment that benefits from spoken line.

- ❌ Pure action sequence (Sheet 1 CCATS uppercut, Sheet 2 SKET slash + FROAK kick) → NO dialogue, just SFX + grunts/exhales optional
- ✅ Hero reveal at peaceful pause → 1-line signature catchphrase optional
- ✅ Confrontation face-off with eye contact → short line both sides optional
- ✅ Comfort / rescue aftermath / quiet emotional moment → longer dialogue OK

Default: no dialogue unless the moment specifically calls for it.

## Cross-references

- [[chill-farm-character-voices]] — Plan A native audio + strategic dialogue (use voice character for Dialogue Cue per clip)
- [[no-subtitles-in-seedance]] — NO subtitle text burned, but Dialogue Cue still used for lip-sync
- [[seedance-prompt-char-limit]] — under 4000 chars per clip (easier now with shorter clips)
- [[seedance-duration-minimum]] — 4s minimum (3-5s clips fit comfortably)
- [[cinematic-director-storyboarding]] — cinematic director's eye still applies (vary angles, conceal/reveal faces strategically)
- [[og10-character-canonical-designs]] — anthropomorphic vs human clauses still required
- [[higgsfield-safety-filter]] — magical fantasy register still applies
- [[strict-storyboard-fidelity]] — gap-filling adds connective motion, NOT new narrative beats; ask user before adding any narrative beats
- [[land-of-hope-locked-visual-style]] — painterly Pixar register still applies via storyboard sheet @图片1

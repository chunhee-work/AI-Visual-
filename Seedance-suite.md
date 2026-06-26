---
name: seedance-suite
description: "Unified entry point for all Seedance 2.0 video-prompt work. Use whenever the user wants to create a Seedance prompt, shot list, video concept, shotlist, brand film, ad, social/meme clip, UGC, anime, short-drama, or visual sequence — or wants a proven Seedance template / one of the nine commercial plays (chase trends 追热点, beverage & product ads 运动饮料广告, brand promo 品牌宣传, outfit-swap 穿搭变装, livestream commerce 直播带货, dynamic poster 动态海报, ad remix 广告复刻, celebrity short-drama 真人短剧, AI manga AI漫剧). Bundles three sub-skills: effects-led prompt builder, cinema-led shotlist director (editable HTML), and a copy-paste prompt library. Routes to the right one based on the task. Trigger on: 'Seedance prompt', 'write me a video prompt', 'shot list', 'shotlist', 'break this script into prompts', 'plan a video', 'video concept', 'brand film prompt', 'ad prompt', 'Seedance template', 'show me a Seedance example', or any description of a scene/ad/film the user wants turned into generation-ready prompts."
---

# Seedance Suite — Unified Router

This is a **router skill**. It bundles three independent Seedance 2.0 sub-skills, each kept **verbatim** below. Do not blend their methods. **Pick exactly one** based on the task, then follow that section's instructions as written, including reading its own reference file.

## Routing table — choose ONE before doing anything

| If the task is… | Use sub-skill | Jump to section | Output |
|---|---|---|---|
| A **fresh brief** for one effects-driven / high-energy clip (ad, social, motion piece) where editing, effects density, pacing and energy arc carry it | **A · Video Prompt Builder** | `## A — Video Prompt Builder` | Plain-text prompt (4-section effects breakdown) |
| A **script, story, scene, or treatment** that needs blocking into multiple cinematic scenes with continuity, dialogue, acting, and a tickable production list | **B · Shotlist Director** | `## B — Seedance Shotlist Director` | Editable **HTML** shotlist saved to outputs |
| The user wants a **proven, copy-paste example/template**, or one of the **nine commercial plays** (trend-chase, beverage ad, brand promo, outfit-swap, livestream, dynamic poster, ad-remix, short-drama, AI manga) | **C · Prompt Library** | `## C — Seedance Prompt Library` | A ready prompt pulled from the library, adapted to specifics |

### Tie-breakers
- **Library feeds the generators.** If the user wants a known structure *and* a custom build, start in **C** to grab the pattern, then hand it to **A** or **B**.
- **Effects vs. cinema:** stacked transitions / speed ramps / "make it punchy" → **A**. Restraint, natural light, multi-scene narrative, continuity across cuts → **B**.
- **One clip vs. a production:** single standalone prompt → **A** or **C**. A whole sequence/film the user will shoot scene by scene → **B**.
- Each sub-skill's reference path (`references/effects-breakdown-reference.txt`, `references/prompt-library.md`, `references/commercial-use-cases.md`) resolves from this skill's own `references/` folder — read them when the chosen sub-skill says to.

Once routed, ignore the other two sections entirely and execute the chosen one exactly as written.

═══════════════════════════════════════════════════════════════════════
## A — Video Prompt Builder
*(verbatim from the `video-prompt-builder` skill)*
═══════════════════════════════════════════════════════════════════════


# Video Prompt Builder for Seedance 2.0

Build cinematic, shot-by-shot video prompts from a creative brief. Every output follows a structured effects breakdown format designed to give Seedance 2.0 maximum detail on camera work, effects, transitions, pacing, and energy arc.

## How this skill works

1. The user provides a **creative brief** — this can be as simple as "a runner in a stadium for a Nike-style ad" or as detailed as a full storyboard description. They may also provide a reference video, mood, brand context, or specific effects they want.
2. Read the reference file at `references/effects-breakdown-reference.txt` to internalise the structure and level of detail expected.
3. Generate a complete video prompt in plain text, structured into the four mandatory sections below.

## Input expectations

The user's brief can include any combination of:
- Subject/talent description (who or what is on screen)
- Setting/environment
- Mood, tone, energy level
- Brand or product context
- Specific effects or camera moves they want
- Duration target
- Reference to existing ads, films, or visual styles
- Colour palette or grade preferences

If the brief is too vague to build a full prompt (e.g. "make something cool"), ask one focused clarifying question before proceeding. Don't over-interrogate — work with what you're given and make creative decisions where the user hasn't specified.

## Output structure

ALWAYS output ALL FOUR sections in this exact order. Never skip a section.

### Section 1: SHOT-BY-SHOT EFFECTS TIMELINE

This is the core of the prompt. Each shot gets its own block structured like this:

```
SHOT [N] ([timestamp]) — [Shot Name / Description]
• EFFECT: [Primary effect name] + [secondary effects if stacked]
• [Detailed description of what's happening visually]
• [Camera behaviour — angle, movement, lens if relevant]
• [Speed/timing information]
• [How this shot connects to the next — transition type]
```

Guidelines for writing shots:
- Each shot should be 1-4 seconds unless the brief calls for longer holds
- Name effects precisely: "speed ramp (deceleration)" not just "speed ramp"; "digital zoom (scale-in)" not just "zoom"
- Describe stacked effects explicitly — if 3 things happen at once, list all 3
- Include transition logic: how does this shot EXIT and how does the next shot ENTER?
- Use language Seedance 2.0 can interpret: describe the visual result, not the editing software technique. For example, say "the frame scales inward rapidly" rather than "apply a keyframed scale effect in After Effects"
- Note the most impactful or signature shot with a callout like "This is the SIGNATURE VISUAL EFFECT"
- Be specific about speed percentages when using slow-motion (e.g. "approximately 20-25% speed")
- Describe motion blur, light behaviour, and atmospheric effects where relevant

### Section 2: MASTER EFFECTS INVENTORY

A numbered list of every distinct effect used across the full prompt, with:
- Effect name
- How many times it's used (e.g. "used 3x")
- Which shots it appears in
- A one-line description of its role in the edit

This section helps the user (and the generator) see the full palette of techniques at a glance. Group similar effects together. Typical categories include: speed manipulation, camera movement, digital effects, transitions, compositing, optical effects.

### Section 3: EFFECTS DENSITY MAP

Break the timeline into segments (roughly 3-6 second chunks) and rate each as:
- **HIGH DENSITY** — 4+ effects stacked or rapid-fire
- **MEDIUM DENSITY** — 2-3 effects
- **LOW DENSITY** — 1 effect or clean/simple footage

Format:
```
[timestamp range] = [DENSITY LEVEL] ([brief list of effects] — [count] effects in [duration])
```

### Section 4: ENERGY ARC

Describe the overall energy structure of the video as a narrative arc. The reference uses a three-act model:
- **Act 1**: Opening energy — how the video grabs attention
- **Act 2**: Middle section — how it develops and what the signature moments are
- **Act 3**: Resolution — how the energy resolves and lands

Adapt the number of acts to suit the video's length and structure. A 5-second clip might only need two beats; a 30-second brand film might need four.

## Creative principles

These principles should guide every prompt you write:

1. **Contrast drives impact.** Alternate high-density and low-density moments. A slow-motion shot after a speed ramp hits harder than two speed ramps back-to-back.
2. **Signature moments matter.** Every video should have at least one "hero" effect — something visually distinctive that makes it memorable. Call it out explicitly.
3. **Transitions are shots.** Don't treat transitions as throwaway connectors. A whip pan, a bloom flash, a motion blur smear — these are creative moments, not just cuts.
4. **Specificity over vagueness.** "The frame rotates clockwise by approximately 15-20°" is better than "the camera tilts." "Approximately 20-25% speed" is better than "slow motion."
5. **Energy must resolve.** No matter how intense the opening, the video needs to land. The final moments should feel intentional, not like the effects budget ran out.

## Tone and style

- Write in a direct, technical tone — like a director's shot notes, not a marketing brief
- Use bullet points within each shot block for clarity
- Be concise but complete — every detail should earn its place
- No hype language, no "stunning" or "breathtaking" — describe what happens and let the visuals speak

## Duration calibration

Adjust the number of shots and effects density to match the target duration:
- **5-10 seconds**: 4-7 shots, lean and punchy, 1 signature effect
- **10-20 seconds**: 8-14 shots, room for contrast and build, 1-2 signature effects
- **20-30 seconds**: 12-20 shots, full three-act arc, 2-3 signature effects
- **30+ seconds**: Scale accordingly, but maintain density contrast — don't fill every second with effects

If the user doesn't specify a duration, default to 15-20 seconds (a sweet spot for AI video generation).

## Example workflow

**User says:** "I want a dramatic brand film for a trail running shoe. Mountain setting, golden hour, single runner. Make it feel epic but not over-the-top. About 15 seconds."

**You do:**
1. Read `references/effects-breakdown-reference.txt` to calibrate detail level
2. Generate the full four-section output: shot-by-shot timeline (8-12 shots), master effects inventory, density map, and energy arc
3. Present in plain text in chat

═══════════════════════════════════════════════════════════════════════
## B — Seedance Shotlist Director
*(verbatim from the `seedance-shotlist-director` skill)*
═══════════════════════════════════════════════════════════════════════


# Seedance 2.0 Shotlist Director

You are a top-tier film director and cinematographer turning scripts into Seedance 2.0 shot-by-shot prompts. The output is a single editable HTML shotlist that the user can open in their browser, tick off scenes as they shoot, and come back to you for revisions.

This is **cinema, not a clip**. You are not chopping a script into beats — you are blocking, lighting, and pacing a film.

---

## What you're producing

A single HTML file (`shotlist.html`) saved to `/mnt/user-data/outputs/` and presented to the user. Structure:

1. **Title bar** — project name (infer from script context, or use "Untitled" if unclear)
2. **Global Style Prefix block** — collapsible, shown at top, applies to every prompt
3. **Scene list** — numbered scenes, each with:
   - Checkbox (✅ done / ⬜ not done)
   - Scene number + short scene description (1 line, what happens in this scene)
   - One or more **Prompts** (each exactly 15 seconds), shown as copy-ready code blocks
4. A small "How to use" note at the top so the user knows checkboxes auto-save and they can ask Claude to revise.

The HTML must be **self-contained** (inline CSS, inline JS), no external dependencies. Checkbox state persists in `localStorage` keyed by scene number so the user's progress survives page reloads.

---

## The Style Prefix

**Always check the conversation first** — if the user uploaded or pasted a custom style prefix, use that exact one verbatim.

If no custom prefix is provided, use this default:

```
Style: 8K IMAX. Photorealistic — no 3D render, no game engine.
Lighting: Natural light only — contre-jour backlight, camera on shadow side, atmospheric haze throughout. Key light from sky and windows only. No artificial lightning.
Color: 60:30:10 — dominant / secondary / accent.
Camera: Physical cine lens. 180° shutter motion blur.
Skin: Pore-level realism — vellus hair, asymmetric moles, capillary flush, pore-shadow matching on-set light.
Acting: Hollywood — micro-pauses before reactions, precise eye-line, living eyes with catch-lights, chest rise from breathing. Characters never standing, always reacting.
Physics: Gravity and inertia respected — mass has real weight, correct contact shadows. No floating props.
Composition: Rule of thirds + golden ratio. Every person moving from frame one.
Continuity: Characters, props, environment identical across every cut. No identity drift.
Technical: 24fps smooth motion. 8K detail. No jitter.
Audio: Environmental SFX only. No music. No subtitles.
```

The Style Prefix appears **once** at the top of the HTML in a collapsible block, AND is prepended verbatim to every prompt's copy-block. The user copies a single prompt to Seedance and it works standalone — no reassembly needed.

---

## Prompt structure (this is the law)

Every prompt follows this exact order, top to bottom:

```
[STYLE PREFIX — full block, verbatim]

Characters:
[Character anchors — short, specific, vivid. Only the characters in this prompt. Carry forward their state from previous scenes — wet hair from the rain in scene 3, blood on the knuckles from the fight in scene 5, the same scar, same wardrobe unless they changed clothes on screen.]

Scene:
[1–2 sentences. What's happening, where, when. Geo-spatial — where each character is positioned relative to the location and to each other. "Anna stands at the kitchen window, back to the room. Marco enters from the hallway, stops in the doorway six feet behind her."]

CUT 1 — [shot type, lens feel, movement]:
[What happens in this shot. Acting beat, gesture, eye-line, breath, micro-pause. What the camera is doing. What the light is doing. Diegetic sound if relevant.]

CUT 2 — [shot type, lens feel, movement]:
[Next beat. Same level of detail.]

CUT 3 — [shot type, lens feel, movement]:
[Final beat of this 15-second prompt.]
```

Each prompt **targets 15 seconds** of screen time. That's the goal — write enough cuts and acting beats to fill the full 15 seconds, because Seedance generates a fixed-length clip and you don't want dead air at the end. Most 15-second prompts hold 1–3 cuts depending on how much the cuts breathe. A long held single shot is a valid prompt if the moment carries it. A rapid-fire 4-cut sequence is also valid if the action calls for it. Either way: design the prompt so all 15 seconds are working.

If a scene is longer than 15 seconds (and most are), split it across multiple prompts under the same scene number: `3a`, `3b`, `3c`. Each one is its own 15-second block with its own full Style Prefix and Characters block. Continuity must hold across them — appearance, position, emotional state, props.

---

## How to direct (read this carefully — this is the actual job)

The structure above is the container. What goes inside it is where the skill lives. You are not just describing what's in the script — you are **deciding** how the film looks and feels.

### Mise-en-scène

Block the scene. Where does each character stand, sit, move to? What are they doing with their hands? What's between them — a table, a window, six feet of empty floor? Geo-spatial detail makes Seedance render coherent space. "She sits across from him at the diner booth, knees touching under the table" is a thousand times better than "they sit and talk."

### Pacing and rhythm

Read the dramatic structure of the script, not just the words. A confession scene needs air — split it. Long held shots, breath between lines, a beat where nobody speaks. An action scene compresses — short cuts, short prompts. A reveal lands on a single sustained close-up; don't undercut it with extra cuts.

If a line of dialogue is heavy, give it its own prompt. If two characters are circling each other before a fight, that's a prompt by itself. Don't pack the script efficiently — pack it dramatically.

### Acting

The default rule from the Style Prefix is **Hollywood acting** — micro-pauses, precise eye-line, living eyes, chest rise from breathing. Translate that into specific direction per shot.

- Not "she looks sad" — "her eyes drop to the table, jaw tightens, she swallows once before answering."
- Not "he's angry" — "knuckles whiten on the glass, breath shortens, eyes never leave hers."
- Not "they kiss" — "she leans in first, he hesitates a half-beat, then meets her."

Restraint by default. Big emotion only when the moment earns it. A whispered line outperforms a screamed one in 90% of cases. If the script calls for a scream, deliver the scream. Otherwise: pull back.

### Continuity (track this internally — never write it as a visible block)

Hold these in your head as you write each prompt:

- **Character state**: wet, dry, bleeding, calm, drunk, exhausted. Carry forward.
- **Appearance**: hair, wardrobe, makeup, props in hand. Don't let it drift cut to cut.
- **Emotional carry**: how did the previous scene leave them? They walk into this one carrying that.
- **Location continuity**: same set, same time of day, same weather unless we cut to a new location.

These never become a separate block in the HTML. They show up as concrete language inside the Characters and CUT lines.

### Camera language

Be specific. Lens, height, movement, motivation.

- "Low-angle 35mm dolly-in on Anna, slow push from waist to chest as she realizes."
- "Static 50mm two-shot, eye-level, locked off — lets the silence sit."
- "Handheld 24mm, follow Marco from behind as he walks into the kitchen — camera lags half a beat."

Motivate every camera move. The camera is a character; it has a reason to be where it is.

### Lighting and color

The Style Prefix locks the global look (contre-jour, natural-only, 60:30:10). Reinforce it inside each prompt with specifics: where the window is, where the sun is, what the haze is doing, what color is dominant in the frame. This isn't redundant — it's how Seedance knows where to put the rim light.

---

## Workflow

When the user gives you a script (or scene, or idea):

1. **Read it as a director, not a transcriber.** Find the dramatic shape. Where does the scene turn? Where does it land? Where does it breathe?
2. **Identify continuity anchors.** Who's in this? What do they look like? What do they carry from scene to scene?
3. **Block out scenes.** Number them 1, 2, 3… Each scene is one beat or location.
4. **Decide prompt count per scene.** Each prompt is one 15-second beat. A 12-second moment still gets one full prompt — fill the 15 seconds with the breath, the look, the held silence after the line. A 40-second confession = 3 prompts (e.g., 5a, 5b, 5c). Honest assessment: how many 15-second beats does this moment actually need to land?
5. **Write each prompt** following the strict structure above. Style Prefix, Characters, Scene + Geo-spatial, CUT 1, CUT 2, etc.
6. **Generate the HTML** using the template approach below.
7. **Save to `/mnt/user-data/outputs/shotlist.html`** and present it.

---

## When the user comes back with revisions

This is critical: when the user asks you to change anything in the shotlist (rewrite scene 4, add an insert shot, split prompt 6 into two, change a character's wardrobe, add a new scene), you **re-generate the same HTML file with the changes applied**. Don't just describe the change in chat — update the document.

Read the previous shotlist if it's still in context or in `/mnt/user-data/outputs/`, apply the user's edits, and write the updated file back. Preserve scene numbering where possible (don't renumber everything if they only changed one prompt). Preserve the Style Prefix unless they tell you to change it.

The user's checkbox state persists in their browser via localStorage, so they don't lose their progress when you re-render the file (as long as scene numbers stay stable).

---

## HTML output template

The HTML structure below is the standard. Inline everything. The CSS aims for a clean, dark, readable directing-room aesthetic — easy on the eyes for long sessions.

Key requirements:
- Each prompt is in a `<pre>` block with monospace font and a "Copy" button
- The full prompt text (Style Prefix + Characters + Scene + CUTs) is the entire content of the `<pre>` — that's what gets copied to Seedance
- Checkboxes save to `localStorage` with key `shotlist-scene-{number}-done`
- Collapsible Style Prefix block at the top
- Scenes separated visually, scene number is large and clear
- The "scene description" line is a one-liner above the prompts — what happens in this scene at a high level
- Multiple prompts within one scene are clearly labeled (e.g., "Prompt 3a", "Prompt 3b")

Use this as the HTML skeleton — fill in `{{PROJECT_TITLE}}`, `{{STYLE_PREFIX_TEXT}}`, and the `{{SCENES_HTML}}` block:

```html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>{{PROJECT_TITLE}} — Director's Shotlist</title>
<style>
  :root {
    --bg: #0e0e10;
    --panel: #17171a;
    --panel-2: #1d1d21;
    --border: #2a2a30;
    --text: #e8e8ea;
    --text-dim: #9a9aa2;
    --accent: #d4a259;
    --done: #4ade80;
  }
  * { box-sizing: border-box; }
  body {
    margin: 0;
    background: var(--bg);
    color: var(--text);
    font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", system-ui, sans-serif;
    line-height: 1.5;
    padding: 32px 24px 80px;
  }
  .container { max-width: 980px; margin: 0 auto; }
  h1 {
    font-size: 28px; font-weight: 600; margin: 0 0 4px;
    letter-spacing: -0.02em;
  }
  .subtitle { color: var(--text-dim); font-size: 14px; margin-bottom: 32px; }
  .howto {
    background: var(--panel);
    border: 1px solid var(--border);
    border-radius: 8px;
    padding: 14px 18px;
    font-size: 13px;
    color: var(--text-dim);
    margin-bottom: 24px;
  }
  details.style-prefix {
    background: var(--panel);
    border: 1px solid var(--border);
    border-radius: 8px;
    padding: 14px 18px;
    margin-bottom: 32px;
  }
  details.style-prefix summary {
    cursor: pointer; font-weight: 600;
    color: var(--accent); user-select: none;
  }
  details.style-prefix pre {
    margin: 14px 0 0; padding: 14px;
    background: var(--panel-2);
    border-radius: 6px;
    font-family: "SF Mono", Menlo, Consolas, monospace;
    font-size: 12.5px;
    white-space: pre-wrap;
    color: var(--text);
  }
  .scene {
    background: var(--panel);
    border: 1px solid var(--border);
    border-radius: 10px;
    padding: 20px 22px;
    margin-bottom: 18px;
  }
  .scene-header {
    display: flex; align-items: flex-start; gap: 12px;
    margin-bottom: 14px;
  }
  .scene-header input[type="checkbox"] {
    width: 20px; height: 20px; margin-top: 2px;
    accent-color: var(--done); cursor: pointer;
    flex-shrink: 0;
  }
  .scene-num {
    font-size: 18px; font-weight: 700;
    color: var(--accent); min-width: 56px;
  }
  .scene-desc {
    font-size: 15px; color: var(--text);
    flex: 1;
  }
  .scene.done .scene-desc { text-decoration: line-through; color: var(--text-dim); }
  .prompt-block {
    background: var(--panel-2);
    border: 1px solid var(--border);
    border-radius: 6px;
    margin-top: 12px;
    overflow: hidden;
  }
  .prompt-label {
    display: flex; justify-content: space-between; align-items: center;
    padding: 8px 14px;
    background: rgba(255,255,255,0.02);
    border-bottom: 1px solid var(--border);
    font-size: 12px; color: var(--text-dim);
    text-transform: uppercase; letter-spacing: 0.05em;
  }
  .copy-btn {
    background: transparent; color: var(--accent);
    border: 1px solid var(--border); border-radius: 4px;
    padding: 4px 10px; font-size: 11px; cursor: pointer;
    text-transform: uppercase; letter-spacing: 0.05em;
    font-family: inherit;
  }
  .copy-btn:hover { border-color: var(--accent); }
  .copy-btn.copied { color: var(--done); border-color: var(--done); }
  pre.prompt {
    margin: 0; padding: 14px 16px;
    font-family: "SF Mono", Menlo, Consolas, monospace;
    font-size: 12.5px;
    white-space: pre-wrap;
    color: var(--text);
  }
</style>
</head>
<body>
<div class="container">
  <h1>{{PROJECT_TITLE}}</h1>
  <div class="subtitle">Director's Shotlist · Seedance 2.0</div>

  <div class="howto">
    Tick scenes as you finish them — your progress saves automatically.
    Click the Copy button on any prompt to grab the full text (Style Prefix + Characters + Scene + Cuts).
    Want changes? Tell Claude what to revise and the file updates.
  </div>

  <details class="style-prefix">
    <summary>Global Style Prefix (applied to every prompt)</summary>
    <pre>{{STYLE_PREFIX_TEXT}}</pre>
  </details>

  {{SCENES_HTML}}
</div>

<script>
  // Persist checkbox state in localStorage
  document.querySelectorAll('.scene input[type="checkbox"]').forEach(cb => {
    const key = 'shotlist-scene-' + cb.dataset.scene + '-done';
    if (localStorage.getItem(key) === '1') {
      cb.checked = true;
      cb.closest('.scene').classList.add('done');
    }
    cb.addEventListener('change', () => {
      localStorage.setItem(key, cb.checked ? '1' : '0');
      cb.closest('.scene').classList.toggle('done', cb.checked);
    });
  });

  // Copy buttons
  document.querySelectorAll('.copy-btn').forEach(btn => {
    btn.addEventListener('click', () => {
      const pre = btn.closest('.prompt-block').querySelector('pre.prompt');
      navigator.clipboard.writeText(pre.textContent).then(() => {
        btn.classList.add('copied');
        const original = btn.textContent;
        btn.textContent = 'Copied';
        setTimeout(() => {
          btn.classList.remove('copied');
          btn.textContent = original;
        }, 1500);
      });
    });
  });
</script>
</body>
</html>
```

Each scene block in `{{SCENES_HTML}}` follows this pattern:

```html
<div class="scene">
  <div class="scene-header">
    <input type="checkbox" data-scene="3">
    <div class="scene-num">3.</div>
    <div class="scene-desc">Anna confronts Marco in the kitchen — first crack in their relationship.</div>
  </div>

  <div class="prompt-block">
    <div class="prompt-label">
      <span>Prompt 3a · 15s</span>
      <button class="copy-btn">Copy</button>
    </div>
    <pre class="prompt">[FULL PROMPT TEXT — Style Prefix verbatim, then Characters, Scene, CUT 1, CUT 2, CUT 3]</pre>
  </div>

  <div class="prompt-block">
    <div class="prompt-label">
      <span>Prompt 3b · 15s</span>
      <button class="copy-btn">Copy</button>
    </div>
    <pre class="prompt">[FULL PROMPT TEXT for the second 15-second chunk of scene 3]</pre>
  </div>
</div>
```

The `data-scene` attribute on the checkbox uses the scene number as a string. If a scene is split across multiple prompts (3a, 3b, 3c), there is still **one checkbox for the whole scene** — the user ticks scene 3 when all of 3a/3b/3c are shot.

---

## A worked example (so you see what good looks like)

User script: *"Anna comes home soaking wet from the rain. Marco is sitting on the couch, looks up from his book, doesn't say anything. She walks past him to the bedroom."*

This is a single scene — call it Scene 1. Honest beats: door opens, she crosses, he watches, the bedroom door clicks shut off-screen. That's a 15-second prompt if you give it the air it deserves — let her stand in the doorway for a beat, let the rain be heard, let his look land. One prompt is enough.

```
Style: 8K IMAX. Photorealistic — no 3D render, no game engine.
Lighting: Natural light only — contre-jour backlight, camera on shadow side, atmospheric haze throughout. Key light from sky and windows only. No artificial lightning.
[...full style prefix verbatim...]

Characters:
ANNA — late 20s, dark hair plastered to her forehead from the rain, soaked navy coat dripping onto the hardwood, mascara slightly smudged under her right eye, lips slightly parted from cold.
MARCO — early 30s, faded grey t-shirt, three-day stubble, paperback book open in his left hand, reading glasses low on his nose.

Scene:
A small Brooklyn apartment, evening. Living room opens directly into a narrow hallway leading to the bedroom. Rain audible against the window stage-right. Marco sits on the left end of a worn leather couch, facing camera-right. The front door is camera-left. Anna enters from the front door, water streaming off her coat. The space between them is roughly twelve feet.

CUT 1 — Wide static, 35mm, eye-level, locked off:
The front door swings open. Anna stands silhouetted in the doorway against the rain-blue street light, contre-jour, water visibly dripping from her coat hem. She doesn't look at Marco. She closes the door slowly with her back, eyes on the floor. Beat. Marco looks up from his book — a small head-tilt, no other movement.

CUT 2 — Medium two-shot, 50mm, slow push-in from couch height:
Anna walks across the frame, left to right, toward the hallway. Her steps leave wet prints on the hardwood. As she passes the couch, she does not turn her head. Marco's eyes track her — only his eyes, his head stays still. The book stays open on his lap.

CUT 3 — Close on Marco, 85mm, static, contre-jour from window behind him:
Marco watches her go. A single slow blink. His jaw shifts once. He looks back down at the book but doesn't read — his eyes stay on the same spot. Off-screen, the bedroom door clicks shut.
```

Notice: the script gave you 28 words. The prompt is detailed because the **directing** is detailed — blocking, eye-line, what each character is doing with their body, what the camera sees and when, what the light is doing. That's the job.

---

## Final reminders

- **English prompts only.** Even if the user writes to you in Russian or another language, the prompt text in the HTML is always English (Seedance 2.0 expects English).
- **15 seconds is the target, not a ceiling to dodge under.** Write each prompt to fill 15 seconds — every prompt is a 15-second clip, so design the cuts and beats to use that full length. Don't pad with empty static, but don't end early either. If the moment genuinely needs more, split across `3a`, `3b`, `3c`.
- **One scene = one checkbox**, even if split across multiple prompts.
- **Continuity tracker, character anchors, pacing notes are not visible blocks** — they live in your head and surface as concrete language inside the prompts.
- **When revising, update the file** — don't describe changes in chat, write them into the HTML and re-present it.

═══════════════════════════════════════════════════════════════════════
## C — Seedance Prompt Library
*(verbatim from the `seedance-prompt-library` skill)*
═══════════════════════════════════════════════════════════════════════


# Seedance 2.0 Prompt Library

A curated library of **proven, real-world Seedance 2.0 video prompts** and the **nine commercial use-cases**, distilled from the Awesome-Seedance collection (X/Twitter, WeChat, Replicate). This is a **reference / copy-paste resource**, not a generator grammar.

Source: [ZeroLu/awesome-seedance](https://github.com/ZeroLu/awesome-seedance) · 卡尔的AI沃茨 [WeChat article](https://mp.weixin.qq.com/s/d2YgM-7vVMQaRP67MtZVdQ)

## When to Use

- User asks for a **proven example or template** to copy ("show me a Seedance prompt for a car-chase / perfume ad / anime fight").
- User describes a **commercial goal** matching one of the nine plays (ad, brand film, outfit-swap, livestream sell, dynamic poster, ad-remix, short-drama, AI manga, trend-chasing).
- User wants to **browse what's achievable** with Seedance 2.0 or borrow a structure/technique.

**When NOT to use (use a generator instead):**
- Build a bespoke shot-by-shot prompt from a fresh brief → `video-prompt-builder` or `cinema-worldbuilder`.
- Build character/scene **image** references (Banana Pro / Soul Cinema) → `banana-pro-director`.
- This library *feeds* those generators with proven patterns; it doesn't replace them.

## How to Use

1. Identify the category or commercial play the user wants (see index below).
2. Pull the matching prompt(s) from the reference files and present them in a fenced code block, ready to paste into Seedance (jianying / 即梦).
3. Adapt the variables (subject, product, palette, duration, dialogue) to the user's specifics — keep the proven structure.
4. Reference images/video/audio attach in the Seedance UI; in the prompt they appear as `@图片1` / `@视频1` / `@音频1` (or `[Image1]`, `[Audio1]`) placeholders.

## Seedance 2.0 Prompt Anatomy (distilled from the corpus)

The high-fidelity prompts share a repeatable structure:

- **Style line** — `Style:` / `【风格】` genre + look + references (e.g. "IMAX 70mm, Denis Villeneuve, gritty realism, desaturated").
- **Duration** — `Duration: 15s` / `【时长】15 秒`. Common: 5s, 10s, 15s.
- **Time-coded shots** — break the clip into beats: `[00:00-00:05] Shot 1: …` → `[00:05-00:10] Shot 2: …`. Each beat names the shot type (wide/close-up/OTS), action, and camera move.
- **Dialogue / lip-sync** — `Dialogue Cue:` / `口型与字幕：` with the exact spoken line; subtitle = the line itself, kept to short clauses.
- **Native audio** — describe diegetic sound (engine roar, rain, crowd) inline; Seedance generates audio. For music, attach a track as `@音频1` rather than naming a song.
- **Reference tags** — `@图片1…@图片6`, `@视频1`, `@音频1` (or `[Image1]`/`[Image2]`) to drive wardrobe-swap, character consistency, ad-remix, or style-match.
- **Consistency clause** — for multi-shot with people: "人物一致性稳定，脸不变，礼服不变 / character identity locked across shots."
- **Aspect ratio** — stated in plain words or `9:16` / `16:9` per platform.
- **Closing quality stack** (cinematic prompts) — "Hyper-realistic, 8k, [DP] cinematography, [composer] sound design."

## Category Index → `references/prompt-library.md`

| # | Category | Examples |
|---|----------|----------|
| 1 | Cinematic film styles | Le Mans racing, Villeneuve desert, Wong Kar-wai, Replicate blockbuster pack, time-coded sequences, jazz audio-sync |
| 2 | Advertising & branding | MUJI promo, perfume MG animation, time-coded perfume ad |
| 3 | Social media & viral memes | Godzilla orange cat, sourdough-pretzel street argument |
| 4 | UGC style | Mirror-glitch vlog, reference-character interior with audio |
| 5 | Anime & animation | Nezha vs Ao Bing, otter mecha, Van Gogh, Tournament of Power, Luffy |
| 6 | Short-form drama | CNY gala talk-show, mini-drama rainy night, viral CEO drama |
| 7 | Visual effects | Sky-zipper surrealism, fluid photo morphs, orbital collision, image-to-video |

## Nine Commercial Use-Cases → `references/commercial-use-cases.md`

| # | Play | 玩法 | One-line recipe |
|---|------|------|-----------------|
| 1 | Chase trends | 追热点 | Recreate a viral clip with copyright-safe footage; key-frame the hero beat |
| 2 | Product/beverage ad | 运动饮料广告 | "精美高级的运动饮料广告，注意分镜编排，明快节奏快剪" — auto storyboard + slogan + music |
| 3 | Brand promo | 品牌宣传 | Name the brand; it writes on-tone VO. 5s still reads complete |
| 4 | Outfit-swap showcase | 穿搭变装 | One model swaps `@图1…@图6` outfits, half-body + full-body, smooth focal cuts |
| 5 | Livestream commerce | 直播带货 | 15s sell script, product close-ups, 3 framing cuts, auto subtitles, CTA |
| 6 | Dynamic poster | 动态海报 | 9:16 fixed-cam, 3×3 grid elements reveal in order (pair with Nano Banana Pro) |
| 7 | Ad remix | 广告复刻 | Mimic `@视频1` storyboard, swap every product to `@图片1`, new VO + palette |
| 8 | Celebrity short-drama | 真人短剧 | Time-coded melodrama, locked identity, word-exact lip-sync subtitles |
| 9 | AI manga | AI漫剧 | Generate anime from a novel passage, style-matched to `@视频1` |

## Key Tips

- Seedance gets ~70–80% from a good reference + detailed prompt; feed more reference frames where a beat fails.
- For grid/poster element ordering, **spell out the sequence explicitly** — the model's ordering control is imperfect.
- If one shot in an ad-remix won't swap cleanly, generate that frame in **Nano Banana Pro** first, then hand it to Seedance to replace that specific shot.
- Queue reality: peak waits are long; off-peak / late night is faster.

## Reference Files

- `references/prompt-library.md` — full proven prompts across the 7 categories (copy-paste).
- `references/commercial-use-cases.md` — the nine commercial plays, clean 中文 + English, with exact prompts.

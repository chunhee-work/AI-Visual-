
# OG10 Teaser — "Your OG10 are back!"

A 30-second AI teaser for OG10 (a Web3 brand with 10 mascot characters). Tooling: **GPT Image 2 / Higgsfield** for stills, **Seedance 2.0** for video clips. Visual target: high-end Disney/Pixar 3D animated feature, *Puss in Boots: The Last Wish* hand-rendered painterly finish.

> NOTE ON VERSIONS: The project went through two story generations. The **final** concept is the "blink-and-you-miss-it teaser" version (no faces ever shown, closed-eye dream fragments, rooftop chase → crash → wake-up). This superseded the earlier "whole street comes alive / drawing winks back" version. All prompts below are the LAST revision of each deliverable.

---

## 1. Story / Concept

**Core:** A young man dozes off at a busy sunny street-side café while sketching a page of OG10 token logos. As he sleeps, he dreams the OG10 have quietly "moved into" the real street around him — each going about an ordinary Earth job. We only ever glimpse them as fragments (a paw, a tail, a back, a silhouette) through a heavy dream-haze. He chases two of them across rooftops, crashes into a chimney, and jolts awake at his table. Everything is normal — just ordinary pedestrians. Was it real? He picks up his sketchbook and gazes at his drawing, still savouring the dream. Cut to black → **OG10 logo + "Your OG10 are back!"**

**Message:** Your OG10 are no longer just drawings — they're back / they've crossed into the real world.
**The hook (ambiguity):** The film never explains whether it was a dream, a crossover, or a return. The proof is left for the audience.

**Final beat structure (30s, strict first-person POV):**

| Time | Beat | Content |
|---|---|---|
| 0–9s | Setup + sleep | Busy street POV, hand sketching OG10 logo page; drowsy, eyelids droop/reopen, head-nods, finally closes fully to black |
| Dream | Flower shop | Heavy dream haze; HEARTA + LYCHEE seen from behind browsing flowers, no faces |
| Dream | Coffee shop | Hears espresso → whips right → CCATS (orange barista cat) seen from behind making latte art |
| Dream | Ramen shop | Ramen aroma → FOT (ramen chef) from behind cooking; skateboard whoosh pulls view away |
| Dream | Street | GST (electrician) skateboards past from behind; donut-shop bell + smell |
| Dream | Donut shop | Only KETDONUT's striped tail swishing behind the counter; pigeons burst up |
| Dream | Library window | ZEYO (scholar) reading + ECOX (astronaut medic) beside him, both backs to camera |
| Dream | Rooftops | Chase SKET + FROAK across roofs → SKET swerves at a chimney → POV can't stop → SLAM → black |
| 0–10s | Wake | Jolts awake face-on-table, recoils up at full speed, scans street (all normal), realizes it was a dream, lifts the sketchbook with both hands, gazes ~3.5s |
| Outro | Logo | Black → OG10 ring logo glows in → "Your OG10 are back!" |

> The narrative "look up to sun → crane down to table → logo" transition beat was discussed but never finalized as a Seedance prompt. The delivered ending is the standalone **logo OUTRO animation** (Section 6).

---

## 2. Characters (OG10 roster)

The teaser uses the **OG10 Earth-job (post-transformation) designs**. In every clip they are shown only as fragments (back / hands / paw / tail / silhouette) — **faces are never revealed.**

| # | Character | Earth job | Teaser fragment / signature trait |
|---|---|---|---|
| 1 | **CCATS** | Barista (orange tabby cat) | Brown apron cross-straps, striped tail, barista cap; making leaf latte art |
| 2 | **FOT** | Ramen chef (boy) | Spiky dark hair + white ramen headband (tied at back), ladling broth |
| 3 | **GST** | Electrician (boy) | Yellow cap, black work jacket, trailing cable, riding a wooden skateboard |
| 4 | **FROAK** | Plumber (anthropomorphic frog) | Frog silhouette running/hopping on rooftops |
| 5 | **SKET** | Convenience-store / samurai cat | Armored samurai cat silhouette leaping across rooftops |
| 6 | **ZEYO** | Scholar (boy, pale pinstripe suit) | Back view reading, "自由" (freedom) scroll in hand, messy black hair |
| 7 | **KETDONUT** | Donut-shop clerk (orange cat) | Pink gingham apron + chef cap; only her orange-striped tail visible |
| 8 | **LYCHEE** | Lychee-farm girl | Long dark-red wavy hair under a straw sun-hat, woven basket of red lychees |
| 9 | **HEARTA** | Nurse | Long lavender wavy hair under a little white nurse cap + white dress |
| 10 | **ECOX** | Astronaut medic | Chunky white-and-teal spacesuit, domed helmet (teal inner glow), red first-aid cross on backpack, teal oxygen tubes, gold ear-pods |

**POV protagonist (the dreaming man):** Pixar/Disney young man — brown messy hair, cream henley + leather suspenders, patched work trousers, brown boots. **Face never shown.** Any visible hands/forearms in frame are HIS human hands (cream rolled sleeves), never an OG10 paw.

---

## 3. Creative Rules (POV / no-face / continuity)

- **Strict first-person POV throughout.** The camera is the man's eyes. Never show his face, even on wake-up. His human hands/forearms (cream rolled sleeves) may enter frame only once awake / for the rooftop brace.
- **No OG10 face — ever.** Every OG10 is shown only as back view / hands / paw / tail / silhouette. Hard rule stated at top and bottom of each prompt.
- **OG10 never react to the camera.** They stay absorbed in their activity. Only the POV man reacts and turns his head. Transitions are driven by a **real-world event the POV notices** (a sound, a smell, a shop bell, pigeons taking off) — not by a character looking at camera.
- **Real-world logic.** No floating/magical objects (e.g. KETDONUT is a shop clerk glazing donuts, not riding a flying donut).
- **Immersive POV journey / clip-chaining.** Each clip ends with an event + a camera turn; the next clip opens matching it (match-cut chain), so the 30s reads as one unbroken POV journey. The POV's own non-verbal voice reactions ("hmm", "whoa", "huh?!", "wait—!") are allowed.
- **Heavy dream haze** (milky soft glow, bloom, drifting motes) covers all dream clips; it also helps obscure faces.
- **Two styles, two jobs:** planning storyboards = graphite pencil sketch; final video = Disney/Pixar 3D painterly. The pencil storyboards are a director's blueprint only — they are NOT fed to Seedance as image refs (the B&W pencil look would corrupt the 3D render).
- **Seedance limits:** ≤9 image refs, ≤4000 chars, ≥4s per clip; open every prompt with the mandatory Style line + subsurface-scattering surface-treatment block.

---

## 4. GPT Image 2 Prompts

### 4.1 Street-café environment plate (final — Australian, English signage, no characters)

```
A wide cinematic establishing frame in the style of a high-end DISNEY / PIXAR 3D ANIMATED FEATURE FILM — fully stylized CGI 3D animation with a hand-painted painterly finish, soft rounded appealing forms, warm and slightly exaggerated storybook charm. This is NOT photorealistic, NOT a photograph, NOT live-action — it is a frame from a modern Disney/Pixar movie: clean stylized shapes, gentle idealized proportions, lush painterly textures, that cosy glowing animated-film look.

THE SCENE — an empty environment plate of a sunny AUSTRALIAN street corner. There are NO characters, NO mascots, NO people and NO cartoon animals anywhere in the shops or the street. First-person point of view, as if seated at a small outdoor café table looking out at the neighbourhood.

In the lower foreground, close and clearly in focus, sits a single cup of coffee on a round saucer on a little metal café table. Resting flat on the saucer (the base plate) right beside the cup is a small printed photo card showing an adorable chibi orange-and-cream cartoon cat character peeking over a latte cup — the printed picture matches the attached held-photo reference, sitting on the saucer like a little keepsake. This printed card is the ONLY cat character in the whole image. Beside the cup lies an open sketchbook with a worn pencil resting across it; the page shows a lively hand-drawn graphite pencil sketch of ten cute chibi fantasy characters playing together — a samurai cat, a frog, kittens, little heroes with floating bowls and orbs — exactly matching the attached hand-drawn sketch reference.

Looking out past the table, a charming sun-washed Australian laneway street corner opens up, rendered in soft Disney/Pixar 3D style, with all signage written in plain ENGLISH only — no Chinese, no Japanese, no Asian lettering anywhere. Immediately to the right is a cosy little coffee shop with a warm glowing interior visible through the window — a polished espresso machine, shelves of cups, soft amber light spilling onto the pavement, the word COFFEE on the glass; the shop interior is empty, no one behind the machine. Right next door stands a small ramen noodle shop with a simple painted English "RAMEN" sign above the doorway and a plain hanging lantern, faint steam curling from inside, a short wooden counter just visible — no foreign characters on any sign. Directly across the narrow street sits a flower shop in full bloom with an English "WILD BLOOMS" sign, its frontage crowded with tin buckets and tiered wooden stands overflowing with fresh stylized flowers in soft natural colours, a striped awning above. Between the shops runs a clean cobblestone and brick sidewalk with a couple of empty bistro chairs, potted plants, climbing greenery and hanging flower baskets on the brick walls, a bicycle leaning in the soft midground. Above the rooftops, a wide warm afternoon sky stretches open, gentle and clear.

Late-afternoon golden sunlight rakes down the laneway from the upper left, catching the steam, the flowers and the awning edges, throwing long soft shadows across the cobblestones, with gentle volumetric light beams and a few drifting dust motes. Warm honeyed colour grade, soft cool shadows, restrained painterly saturation, shallow depth of field with creamy bokeh, strong layered depth from the sharp foreground cup and sketchbook to the soft hazy far end of the street. The whole street feels alive, lived-in and inviting, yet completely empty — a beautifully lit animated stage waiting for something to happen.

References needed:
- 图片1 = the previously generated street-corner layout (keep the same composition and scene, re-render fully in stylized Disney/Pixar 3D animation, English-only signage — NOT photoreal)
- 图片2 = the hand-drawn chibi OG10 sketch (content shown on the open sketchbook page)
- 图片3 = the held-photo reference of the cute cat-on-coffee picture (placed flat on the saucer as a small printed photo card — do not add this cat anywhere else)
```

### 4.2 Hand-drawn OG10 chibi character page (final — exactly 10, no duplicate KETDONUT)

```
A hand-drawn graphite pencil sketch filling a single page of a cream off-white sketchbook, visible paper grain and subtle tooth texture, the kind of lively character study a skilled artist scribbles in their personal sketchbook. EXACTLY TEN stylized chibi fantasy characters drawn together across the page — ONE of each canonical design from the reference, NO duplicates, NO extra characters, NO repeated figures. Count carefully: ten figures total, each unique.

The ten, each appearing ONCE: an armored samurai cat striding with twin blades; a small bouncing cat-girl mid-leap; an astronaut medic firing a teal blaster; a bearded anthropomorphic frog holding a steaming coffee cup; a haloed magic girl with a winged-heart staff; a red-qipao girl with floating orbs; a paper-scroll ninja boy; a backward-cap boy riding a small wooden skateboard; a plump steampunk barista cat in a "CCATS" apron; and a purple-cloak ninja-chef boy balancing floating ramen bowls. The donut-cat character (KETDONUT) appears as ONE single figure only — a chubby cat happily with its sprinkled donut — do NOT draw a second or extra donut-cat or kitten anywhere on the page. They interact and play joyfully — overlapping poses, dynamic and warm, full of fun and motion.

Keep the characters' canonical designs from the reference: several are anthropomorphic animals — anthropomorphic cats, an armored samurai cat, an anthropomorphic frog, an anthropomorphic kitten — drawn as appealing chibi creatures, never as real animals or humans.

Pure pencil rendering: loose confident graphite linework with varied line weight, gestural energetic strokes, light cross-hatch and pencil shading for soft volume, a few visible eraser smudges and stray construction lines, small doodles and quick scribbled marks in the page corners. Monochrome graphite on paper — no digital color, no ink, no paint. Authentic personal-sketchbook feel: spontaneous, hand-made, lived-in, slightly uneven, charming, energetic. Soft natural pencil grays, fine graphite grain, paper fiber texture. Not photoreal, not 3D-rendered, not flat vector — a real hand-drawn pencil sketch on textured paper.

References needed:
- 图片1 = OG10 group lineup canonical (locks all 10 character designs — exactly ten figures, one each, keep anthropomorphic animals as drawn, NO duplicate KETDONUT)
```

### 4.3 OG10 token-logo sketchbook page (final — CCATS lounging-behind-cup + "GST GESTURE")

```
A hand-drawn graphite pencil sketch filling a single page of a cream off-white sketchbook, visible paper grain and tooth texture — an artist's personal page where they doodle and explore a set of emblems. Ten different emblem/mascot designs are drawn across the page in PENCIL, scattered IRREGULARLY at varying sizes and angles, casually overlapping, some big and some small, tilted and loose — never a neat grid or row. Around them are stray construction lines, little doodled hearts and stars, and quick scribbles, with a small signature scrawl in a corner.

The ten hand-sketched emblems:
1. A round token logo: a cute chubby orange-and-cream cartoon cat lying down BEHIND a large latte coffee cup (with leaf/rosetta latte art on top), the cat's rounded head, ears and two little front paws peeking out around the sides and base of the cup, sleepy and content. Match this exact design — the cat is lounging behind the cup, not standing, not holding a coin.
2. A round emblem of a shiny astronaut helmet with a planet-Earth globe as its face — two big round goggle-eyes and a wide smiling mouth.
3. A circular medallion with "FOOD TOKEN" lettering around the rim and a cornucopia (horn overflowing with fruit, bread and vegetables) in the center.
4. A round badge with a bold stylized green frog head in profile, a single round eye.
5. A graphic emblem of a hand throwing a surfer "shaka" gesture (thumb and pinky out), with bold block lettering reading exactly "GST GESTURE" — the top word must clearly spell G-S-T (three letters: G, S, T), with "GESTURE" beneath it.
6. A glossy round token button with a heart outline in the center.
7. A cute round character — a cat made from a sprinkled chocolate-frosted donut, with little cat ears and paws.
8. A round token coin with a glossy lychee fruit and a single green leaf in the center.
9. A detailed ink-and-pencil scene of an armored samurai cat in a fighting stance wielding twin katana on a tiled rooftop.
10. A circular seal emblem with stylized brushstroke calligraphy characters arranged around a central diamond shape.

Pure pencil rendering: loose confident graphite linework with varied line weight, gestural strokes, light cross-hatch and shading for volume, a few visible eraser smudges and stray lines, hand-made and lived-in. Monochrome graphite on paper — no digital color, no ink wash, no paint. Soft natural pencil grays from light to dark, fine graphite grain, paper fiber texture. Not photoreal, not 3D-rendered, not flat vector — a real hand-drawn pencil sketch page, irregular and charming.

References needed:
- 图片1 = the hand-drawn OG10 sketchbook page (locks the pencil-sketch style and paper look)
- 图片2 = CCATS coin logo — orange cat lounging behind a latte cup, head and paws peeking out (match this exact design)
- 图片3 = astronaut helmet Earth-face emblem
- 图片4 = FOOD TOKEN cornucopia coin
- 图片5 = green frog head badge
- 图片6 = GST GESTURE shaka-hand emblem (text must read "GST GESTURE")
- 图片7 = purple heart token
- 图片8 = donut-cat character
- 图片9 = lychee token coin
- 图片10 = samurai cat twin-katana scene
- 图片11 = circular calligraphy freedom seal
```

### 4.4 SKET samurai-cat replacement edit (final — exact twin-katana copy)

```
Take reference image 1 (a hand-drawn graphite pencil sketchbook page) and keep EVERYTHING on it 100% unchanged — the same paper, the same pencil style, the same nine emblems in the exact same positions and sizes (cat behind the latte cup, astronaut Earth-face helmet, FOOD TOKEN cornucopia coin, green frog-head badge, "GST GESTURE" shaka hand, heart token, donut-cat, lychee coin, calligraphy diamond seal), the same hearts, stars, scribbles and signature. Do not alter, move, or restyle anything else.

Replace ONLY the samurai cat in the lower-left with the scene from reference image 2, copied EXACTLY: a dark armored samurai cat standing on a tiled rooftop in a wide dynamic combat stance, wielding TWO katanas — the right blade raised high overhead, the left blade extended out to the side — clad in detailed lamellar armor with a round gold emblem on the chest, tail flicked out, fierce eyes and whiskers; in the lower-left foreground a smaller orange tabby cat in samurai garb crouches with its back to us, watching; misty traditional village rooftops and bare winter trees fade into the background. Reproduce image 2's composition and poses exactly, just redrawn in the same graphite pencil sketch style as the rest of the page so it blends in.

Monochrome graphite pencil, paper grain, hand-drawn and lived-in — not photoreal, not 3D, not colored. Everything except the samurai cat stays exactly as in image 1.

References needed:
- 图片1 = the latest sketchbook page (keep all other emblems, layout, and style 100% identical)
- 图片2 = the twin-katana samurai cat scene (copy this exactly — two katanas, the watching orange cat, rooftop, misty village) as the replacement for the samurai cat
```

### 4.5 Book-drawing replacement edit (final — place the chibi character page into the table's sketchbook)

```
Take the street-corner café scene and keep the ENTIRE image 100% unchanged — same Disney/Pixar 3D animated style, same sunny laneway, same flower shop, ramen shop and coffee shop with all their signage and the single ramen lantern, same brick walls, bicycle, warm golden afternoon lighting and atmosphere, same coffee cup with latte art, same saucer with the little printed cat-coffee photo card, same chair, same round metal table, same pencil resting on the book. Do not move, restyle, recolour or alter anything in the scene; keep only the one ramen lantern, add no others.

Change ONLY the artwork shown on the open sketchbook lying on the table: replace its current drawing with the supplied hand-drawn OG10 chibi character page — the lively graphite pencil group of the ten chibi characters (armored samurai cat, bouncing cat-girl, astronaut medic with blaster, bearded frog with coffee, haloed magic girl with winged-heart staff, red-qipao girl with orbs, paper-scroll ninja boy, backward-cap skateboard boy, steampunk "CCATS" barista cat, purple-cloak ramen boy). Render it in the same graphite pencil sketch style, laid out across the two visible open pages and following the book's exact perspective, angle and lighting on the table so it sits naturally on the paper.

Everything else stays exactly the same. The only change is the drawing inside the open sketchbook.

References needed:
- 图片1 = the street-corner café scene (keep the whole environment, coffee, card, single lantern, lighting 100% identical — only change the drawing in the open book)
- 图片2 = the new OG10 chibi character page (the artwork to place onto the open sketchbook pages, in perspective)
```

### 4.6 Ending end-card still (final — bold premium typography)

```
A premium cinematic teaser END-CARD on a pure solid black background, horizontal title-card layout.

Use the supplied logo artwork EXACTLY AS-IS, completely unchanged — the ring of ten circular OG10 token emblems arranged around the central multicolour geometric spiral-square OG10 mark. Keep every emblem, colour, position and the central logo identical; do not restyle, recolour, crop or regenerate the logo. Place this logo composition centered in the upper-middle of the frame with comfortable black space around it.

Below the logo, set ONLY the tagline text, centered: "Your OG10 are back!" — redesigned for a PREMIUM, HIGH-IMPACT look, like the hero title card of a major animated-feature trailer. Use a bold, heavy, modern cinematic sans-serif title typeface — strong confident weight, clean geometric letterforms, tight controlled letter-spacing, commanding presence. Give the letters a refined polished finish with a subtle metallic sheen and a soft outer glow that picks up the rainbow gradient (blue-green-magenta) of the central logo. Make "OG10" the focal accent — slightly bolder and brighter, glowing in that rainbow gradient — while "Your", "are" and "back!" sit in crisp premium white. The exclamation mark adds punch. Elegant yet powerful, expensive, impactful.

Pure black background throughout, soft subtle vignette, gentle bloom around the logo and the text, nothing else in frame. Sharp, clean, ultra high-resolution graphic design.

References needed:
- 图片1 = the OG10 ring logo artwork (use exactly as-is, unchanged — only redesign/upgrade the tagline typography beneath it)
```

---

## 5. Seedance 2.0 Clip Prompts (story order)

All clips: 16:9, open with the mandatory Style line + surface-treatment block, strict first-person POV, OG10 faces never shown. The chain links each clip's end-event to the next clip's opening.

### C1 — Opening: drawing → getting drowsy → eyes close to black (9s)
Refs: `图片1` = environment plate · `图片2` = OG10 emblem/logo page

```
Style: Painterly cinematic Pixar/Disney 3D animated feature register, Puss in Boots: The Last Wish hand-rendered painterly finish. Warm cinematic, soft volumetric golden afternoon light, shallow depth of field, gentle film grain, rich subtle expression and smooth natural motion throughout. Strict FIRST-PERSON POV from a HIGH downward angle — the camera is a young man's eyes already looking steeply DOWN at his own sketchbook and hand; never show his face. Duration: 9s. 16:9.

[00:00-00:03] The clip OPENS on a high first-person POV angled steeply down at an open sketchbook on a round metal café table; the man's hand holds a pencil and naturally, smoothly sketches a page of cute little OG10 emblem and token doodles — relaxed, unhurried strokes, the wrist drifting across the paper. Beside it a cup of coffee with leaf latte art and a small printed cat photo card. Beyond and below, a busy sunny street with passers-by in soft focus. Calm and content.

[00:03-00:05] Drowsiness creeps in — the pencil strokes grow lazy and trail off. His EYELIDS DROOP HALF-CLOSED, the frame dimming and softening halfway from the top and edges... then he forces them back OPEN, the view brightening and refocusing on the page, a soft sleepy sigh as he tries to keep drawing.

[00:05-00:07] The weak strokes slow again and drowsiness returns — the EYELIDS DROOP HALF-CLOSED a second time, the view darkening and swimming halfway, then a DROWSY HEAD-NOD: the POV dips smoothly downward and jerks gently back up, nods and droops once more, heavy-lidded, a small yawn.

[00:07-00:09] Finally he gives in and drifts to sleep — the POV sinks down in one smooth motion, going soft, hazy and swimming, and the EYELIDS CLOSE COMPLETELY, the whole frame fading fully and gently to BLACK. He is asleep.

Surface treatment: skin, fur, hair and fabric show natural subsurface scattering — warm translucent quality at the edges, ears and fingertips; soft painterly micro-texture, hand-rendered. No plastic CG sheen, no oversharpened photoreal detail, no flat illustration look.

Native audio: gentle busy-street ambience, soft distant chatter and footsteps, faint pencil scratching that slows, pauses, weakly resumes and stops; the man's own soft drowsy sighs and small yawns, a final quiet sleepy exhale as the eyes close. No dialogue, no music track.

References:
@图片1 = Disney/Pixar 3D street-café environment plate (high downward view of the table, coffee, card)
@图片2 = hand-drawn OG10 emblem/logo page (the drawing in the sketchbook)
```

### C2 — Flower shop: HEARTA + LYCHEE from behind (5s)
Refs: `图片1` = environment plate (LEFT flower shop) · `图片2` = HEARTA · `图片3` = LYCHEE

```
Style: Painterly cinematic Pixar/Disney 3D animated feature register, Puss in Boots: The Last Wish hand-rendered painterly finish. Warm cinematic tone, EXTREMELY HEAVY dreamlike haze, thick milky soft-glowing light, strong soft-focus bloom, gauzy diffusion, floating golden dust motes and drifting sparkles, very shallow depth of field with creamy bokeh. Strict FIRST-PERSON POV (camera = the man's eyes; never show his face, body, hands or feet). The audience IS this POV, groggy and curiously looking around the dreamlike street. Deep DREAM, soft and indistinct. Duration: 5s. 16:9.

IMPORTANT HARD RULE: the two girl characters' FACES must NEVER be shown — they stay with their BACKS fully to camera the entire time, faces hidden, lost in haze. Never reveal a face.

[00:00-00:015] JUST-WOKEN feel: the first-person POV opens heavily blurred and swimming, as if eyes are only half-cracking open — soft focus pulsing in and out, the milky dream-haze street wobbling and slowly drifting into unsteady view, disoriented and dreamy, light blooming everywhere.

[00:015-00:03] A girl's faint, MUFFLED voice and soft unclear laughter drift in from the LEFT — too soft to make out. Curious, the POV slowly, dreamily TURNS LEFT toward the sound, the heavy blur gently resolving as the left-side flower shop swims into focus through the fog.

[00:03-00:045] Inside the left flower shop, two figures stand with their BACKS fully to the camera, slowly browsing the blooms — one with long lavender wavy hair over a little white nurse cap and white dress, the other with long dark-red wavy hair under a wide straw sun-hat, a woven basket of red lychees at her side. They drift among the flowers, faces NEVER visible, soft and luminous, half-dissolved in the rolling dream-mist and sparkles.

[00:045-00:05] Suddenly an espresso machine HISS and milk steaming ring out from the RIGHT. Reacting with curiosity, the POV WHIPS fast to the RIGHT — a quick sharp motion-blurred head-turn smearing the haze and bokeh as the clip ends, eyes locking toward the right-side coffee shop.

Surface treatment: skin, fur, hair and fabric show natural subsurface scattering — warm translucent quality at the edges, ears and fingertips; soft painterly micro-texture, hand-rendered. No plastic CG sheen, no oversharpened photoreal detail, no flat illustration look.

Reminder: neither girl's face is ever shown — backs to camera throughout.

Native audio: a faint muffled girl's voice and soft laughter from the left (no clear words), gentle wind chimes, then a sudden espresso hiss and milk steaming from the right, a low dreamy hum, muffled underwater street ambience. No dialogue, no music track.

References:
@图片1 = Disney/Pixar 3D street-café environment plate (POV angle + distance, LEFT-side flower shop)
@图片2 = HEARTA Earth-job turnaround (lavender-hair nurse — back view only, face NEVER shown)
@图片3 = LYCHEE Earth-job turnaround (red-hair lychee farmer, straw hat — back view only, face NEVER shown)
```

### C3 — Coffee shop: CCATS making latte art (back, upper body, ~2s) (5s)
Refs: `图片1` = environment plate (RIGHT coffee shop) · `图片2` = CCATS

```
Style: Painterly cinematic Pixar/Disney 3D animated feature register, Puss in Boots: The Last Wish hand-rendered painterly finish. Warm cinematic tone, EXTREMELY HEAVY dreamlike haze, thick milky soft-glowing light, strong soft-focus bloom, gauzy diffusion, floating golden dust motes and drifting sparkles, very shallow depth of field with creamy bokeh. Strict FIRST-PERSON POV (camera = the man's eyes; never show his face, body, hands or feet). The audience IS this POV, groggy and curiously looking around the dreamlike street. Deep DREAM, soft and indistinct. Duration: 5s. 16:9.

IMPORTANT HARD RULE: the barista cat is seen ONLY from BEHIND, his BACK fully to camera the entire time — his FACE must NEVER be shown, not even in profile. Never reveal his face.

[00:00-00:01] Continuing seamlessly from the previous fast turn, the first-person POV completes a quick sharp WHIP to the RIGHT toward the right-side coffee shop — streaking motion blur smearing the milky haze and bokeh as the eyes lock onto the source of an espresso-machine hiss.

[00:01-00:03] The whip settles on the right-side coffee shop across the laneway, at the café-table distance of the reference plate: inside, the orange tabby barista cat is seen from BEHIND — his back to us, brown apron cross-straps over a plump orange-striped back, a long striped tail swaying, a little brown barista cap, busy at the espresso machine finishing latte art, warm steam rising and catching the hazy light. Soft and dreamy, face never visible.

[00:03-00:04] The POV lingers a curious beat on his working back through the mist; a soft wondering hum from the man as he watches, the haze gently breathing, sparkles drifting.

[00:04-00:05] A waft of fragrant ramen steam and a faint slurping sound drift in from the next-door ramen shop; intrigued, the POV begins to turn and drift toward that aroma — a soft motion-blurred transition as the clip ends, eyes pulling toward the ramen counter.

Surface treatment: skin, fur, hair and fabric show natural subsurface scattering — warm translucent quality at the edges, ears and fingertips; soft painterly micro-texture, hand-rendered. No plastic CG sheen, no oversharpened photoreal detail, no flat illustration look.

Reminder: the barista cat stays back-to-camera throughout — his face is NEVER shown.

Native audio: a sudden espresso hiss and milk steaming from the right, soft pouring; the man's own soft curious inhale and a low wondering "hmm"; then a faint ramen slurp and sizzle drifting from the next door; a low dreamy hum, muffled underwater street ambience. No dialogue, no music track.

References:
@图片1 = Disney/Pixar 3D street-café environment plate (POV angle + distance, RIGHT-side coffee shop)
@图片2 = CCATS Earth-job turnaround (orange barista cat — BACK VIEW only, face NEVER shown)
```

### C4 — Ramen shop: FOT cooking (back, upper body, FOT never reacts) (4s)
Refs: `图片1` = environment plate (ramen shop) · `图片2` = FOT

```
Style: Painterly cinematic Pixar/Disney 3D animated feature register, Puss in Boots: The Last Wish hand-rendered painterly finish. Warm cinematic tone, EXTREMELY HEAVY dreamlike haze, thick milky soft-glowing light, strong soft-focus bloom, gauzy diffusion, floating golden dust motes and drifting sparkles, very shallow depth of field with creamy bokeh. Strict FIRST-PERSON POV (camera = the man's eyes; never show his face, body, hands or feet). The audience IS this POV, groggy and curiously noticing the dreamlike street. Deep DREAM, soft and indistinct. Duration: 4s. 16:9.

IMPORTANT HARD RULES: (1) the ramen-chef is shot from directly BEHIND, UPPER-BODY framing only, his back to camera — his FACE must NEVER be shown. (2) The ramen-chef NEVER reacts, never turns, never looks at the camera — he stays absorbed in cooking the whole time. ONLY the first-person POV man reacts: HE hears the event and turns HIS head. The transition is the POV's head-turn, never the character's.

[00:00-00:01] Continuing seamlessly from the drift toward the ramen aroma, the first-person POV turns and glides through the milky haze toward the Japanese ramen shop with its hanging noren curtains, the steaming counter swimming softly into view.

[00:01-00:03] A SHORT ~2-second curious glimpse: framed from directly BEHIND him, UPPER BODY only, the ramen-chef boy works at the counter — back to us, spiky dark hair with a white ramen headband tied at the back, sleeves rolled, shoulders and arms busy ladling rich broth and finishing a steaming bowl, fragrant steam billowing up into the hazy light. He stays fully absorbed in his cooking, oblivious, never turning. A soft wondering "hmm" from the watching man. Face never visible.

[00:03-00:04] Suddenly a skateboard WHOOSH and the clatter of wheels rip across the street behind. The ramen-chef keeps cooking, unaware — but the FIRST-PERSON POV man, startled and curious, turns HIS OWN head away from the counter toward the street: a fast natural motion-blurred head-turn smearing the haze as the clip ends, his eyes chasing the rolling sound.

Surface treatment: skin, fur, hair and fabric show natural subsurface scattering — warm translucent quality at the edges, ears and fingertips; soft painterly micro-texture, hand-rendered. No plastic CG sheen, no oversharpened photoreal detail, no flat illustration look.

Reminder: the ramen-chef stays back-to-camera and absorbed in cooking the whole time — his face is NEVER shown and he NEVER reacts. Only the POV man reacts and turns.

Native audio: gentle ramen sizzle, bubbling broth and a ladle clink, the watching man's own soft curious "hmm"; then a sudden skateboard whoosh and wheels clattering across the street; a low dreamy hum, muffled underwater street ambience. No dialogue, no music track.

References:
@图片1 = Disney/Pixar 3D street-café environment plate (POV angle toward the ramen shop)
@图片2 = FOT Earth-job turnaround (ramen-chef boy — BEHIND, upper-body, absorbed in cooking, face NEVER shown)
```

### C5 — GST skateboards past → donut-shop bell (~2s glimpse) (4s)
Refs: `图片1` = environment plate (street, donut shop) · `图片2` = GST

```
Style: Painterly cinematic Pixar/Disney 3D animated feature register, Puss in Boots: The Last Wish hand-rendered painterly finish. Warm cinematic tone, EXTREMELY HEAVY dreamlike haze, thick milky soft-glowing light, strong soft-focus bloom, gauzy diffusion, floating golden dust motes and drifting sparkles, very shallow depth of field with creamy bokeh. Strict FIRST-PERSON POV (camera = the man's eyes; never show his face, body, hands or feet). The audience IS this POV, groggy and curiously noticing the dreamlike street. Deep DREAM but grounded in real-world logic. Duration: 4s. 16:9.

IMPORTANT HARD RULES: (1) the skateboarding boy is seen ONLY from BEHIND / legs and board — back to camera, FACE NEVER shown. (2) He NEVER reacts or looks at the camera — he just skates past, absorbed. ONLY the first-person POV man reacts and turns. (3) Everything obeys REAL-WORLD LOGIC — no floating or magical objects.

[00:00-00:01] Continuing seamlessly from the whip toward the street, the first-person POV catches a wooden skateboard WHOOSHING across the foreground — a SHORT ~2-second glimpse of the electrician boy seen from BEHIND, skating past: a yellow cap from behind over dark hair, a black work jacket, a trailing cable, legs riding the board, streaking motion blur and dreamy speed lines through the milky haze.

[00:01-00:025] The POV follows him from behind for a beat as he glides and carves smoothly down the sunny cobblestone laneway, weaving through the soft fog and passers-by, rolling away; a soft impressed "whoa" from the watching man. He never turns, fully absorbed in his ride. Face never visible.

[00:025-00:04] From a little donut shop along the street, a warm sweet smell of fresh-fried donuts drifts over and its door-bell gives a bright JINGLE as a customer steps out. The skater keeps rolling away, unaware — but the FIRST-PERSON POV man, drawn and curious, turns HIS OWN head away from the street toward the donut shop: a smooth natural head-turn, soft motion blur through the haze, as the clip ends.

Surface treatment: skin, fur, hair and fabric show natural subsurface scattering — warm translucent quality at the edges, ears and fingertips; soft painterly micro-texture, hand-rendered. No plastic CG sheen, no oversharpened photoreal detail, no flat illustration look.

Reminder: the skateboarding boy stays back-to-camera and absorbed throughout — his face is NEVER shown and he NEVER reacts. Only the POV man reacts and turns.

Native audio: a skateboard whoosh and wheels clacking over stone, the watching man's own soft "whoa"; then a bright shop door-bell jingle from up the street; a low dreamy hum, muffled underwater street ambience. No dialogue, no music track.

References:
@图片1 = Disney/Pixar 3D street-café environment plate (sunny laneway / street, donut shop along it)
@图片2 = GST Earth-job turnaround (electrician boy on skateboard — BACK VIEW / legs + board only, face NEVER shown)
```

> NOTE: A combined GST+KETDONUT 6s clip also exists in the transcript, but the user later confirmed the order GST → KETDONUT as **separate** clips, so C5 and C6 are the final split versions.

### C6 — Donut shop: only KETDONUT's tail → pigeons take off (4s)
Refs: `图片1` = environment plate (donut shop / rooftops) · `图片2` = KETDONUT

```
Style: Painterly cinematic Pixar/Disney 3D animated feature register, Puss in Boots: The Last Wish hand-rendered painterly finish. Warm cinematic tone, EXTREMELY HEAVY dreamlike haze, thick milky soft-glowing light, strong soft-focus bloom, gauzy diffusion, floating golden dust motes and drifting sparkles, very shallow depth of field with creamy bokeh. Strict FIRST-PERSON POV (camera = the man's eyes; never show his face, body, hands or feet). The audience IS this POV, groggy and curiously noticing the dreamlike street. Deep DREAM but grounded in real-world logic. Duration: 4s. 16:9.

IMPORTANT HARD RULES: (1) of the donut-shop cat, ONLY her orange-striped TAIL is visible — her body, head and FACE are completely hidden behind the counter and NEVER shown. (2) She NEVER reacts or looks at the camera. ONLY the first-person POV man reacts and turns. (3) Everything obeys REAL-WORLD LOGIC — no floating or magical objects.

[00:00-00:01] Continuing seamlessly from the donut-shop bell and sweet smell, the first-person POV turns and steps in toward the little donut shop counter, the warm glowing interior swimming softly into view through the milky haze.

[00:01-00:03] A SHORT ~2-second curious glimpse: behind the donut-shop counter, only a fluffy ORANGE-STRIPED CAT TAIL pokes out and swishes gently from side to side, the cat herself fully hidden below and behind the counter, busy at work. On the counter sit a fresh tray of pink-glazed donuts and a half-packed pink "KETDONUT" box, a little chef cap just visible. Just the swishing tail — tantalising and mysterious — a soft wondering "hmm" from the watching man. No body, no face shown.

[00:03-00:04] Out on the street, a small flock of pigeons suddenly bursts up off the cobblestones with a flapping rush, wheeling up past the rooftops. Below the counter the tail keeps swishing, unaware — but the FIRST-PERSON POV man, drawn by the sound, lifts HIS OWN gaze and tilts UP to follow the birds toward the rooftops: a smooth natural upward head-tilt through the haze as the clip ends.

Surface treatment: skin, fur, hair and fabric show natural subsurface scattering — warm translucent quality at the edges, ears and fingertips; soft painterly micro-texture, hand-rendered. No plastic CG sheen, no oversharpened photoreal detail, no flat illustration look.

Reminder: ONLY the cat's tail is ever visible — her body and face are NEVER shown, and she NEVER reacts. Only the POV man reacts and looks up.

Native audio: soft shop ambience, a gentle glaze drizzle and box-folding sound from behind the counter, the watching man's own soft curious "hmm"; then a sudden flapping rush of pigeons taking off and wheeling up outside; a low dreamy hum, muffled underwater street ambience. No dialogue, no music track.

References:
@图片1 = Disney/Pixar 3D street-café environment plate (donut shop interior / street, rooftops above)
@图片2 = KETDONUT Earth-job turnaround (orange donut-shop cat — ONLY the striped tail visible, body & face NEVER shown)
```

### C7 — Library window: ZEYO reading + ECOX beside him (both backs to camera) (5s)
Refs: `图片1` = environment plate (library window) · `图片2` = ZEYO · `图片3` = ECOX

```
Style: Painterly cinematic Pixar/Disney 3D animated feature register, Puss in Boots: The Last Wish hand-rendered painterly finish. Warm cinematic tone, EXTREMELY HEAVY dreamlike haze, thick milky soft-glowing light, strong soft-focus bloom, gauzy diffusion, floating golden dust motes and drifting sparkles, very shallow depth of field with creamy bokeh. Strict FIRST-PERSON POV (camera = the man's eyes; never show his face, body, hands or feet). The audience IS this POV, groggy and curiously looking around the dreamlike street. Deep DREAM but grounded in real-world logic. Duration: 5s. 16:9.

IMPORTANT HARD RULES: (1) BOTH characters are seen ONLY from BEHIND, backs to camera — their FACES are NEVER shown (the scholar's head from behind, the astronaut medic's helmet from the back). (2) Neither OG10 reacts or looks at the camera — they stay absorbed; ONLY the first-person POV man reacts and turns. (3) Everything obeys REAL-WORLD LOGIC.

[00:00-00:015] Continuing seamlessly from the upward head-tilt, the first-person POV rises and settles on an upper-floor library window through the milky dream-haze, a warm glowing study inside swimming softly into view.

[00:015-00:04] A SHORT ~2.5-second curious glimpse: inside, two figures sit together at the desk by the window, both seen from BEHIND. On one side the scholar in a pale pinstripe suit, messy black hair, quietly reads with an old "自由" scroll in hand. Right beside him sits the astronaut-medic, a small chibi figure from behind in a chunky white-and-teal spacesuit — the back of a round domed helmet with a soft teal inner glow, a big red first-aid cross on the backpack, teal oxygen tubes and little gold ear-pods — leaning in companionably as they share the book. Both stay absorbed and still, never turning. A soft wondering "hmm" from the watching man. No faces.

[00:04-00:05] A faint clatter and soft footstep sound from higher up on the rooftop above; drawn by it, the POV man tilts HIS gaze further UP toward the rooftops — a smooth natural upward transition through the haze, the clip ending mid-rise as his eyes climb toward the roofline (still unrevealed).

Surface treatment: skin, fur, hair and fabric show natural subsurface scattering — warm translucent quality at the edges, ears and fingertips; soft painterly micro-texture, hand-rendered. No plastic CG sheen, no oversharpened photoreal detail, no flat illustration look.

Reminder: both characters stay back-to-camera — no face is ever shown, neither reacts. Only the POV man reacts and looks up.

Native audio: quiet library hush, a soft page turn, the watching man's curious "hmm"; then a faint clatter and footstep from the rooftop above; a low dreamy hum, muffled underwater street ambience. No dialogue, no music track.

References:
@图片1 = Disney/Pixar 3D street-café environment plate (upper-floor library window, rooftops above)
@图片2 = ZEYO Earth-job turnaround (scholar in pale pinstripe suit — back view reading, face NEVER shown)
@图片3 = ECOX Earth-job turnaround (chibi astronaut medic — back view, helmet from behind, red cross on back, face NEVER shown)
```

### C8 — Rooftop chase: SKET + FROAK → crash into chimney → black (10s)
Refs: `图片1` = environment plate (rooftops/chimneys) · `图片2` = SKET · `图片3` = FROAK · `图片4` = POV man (hands/forearms only)

```
Style: Painterly cinematic Pixar/Disney 3D animated feature register, Puss in Boots: The Last Wish hand-rendered painterly finish. Warm cinematic tone, EXTREMELY HEAVY dreamlike haze, thick milky soft-glowing light, strong soft-focus bloom, gauzy diffusion, floating dust motes and sparkles, very shallow depth of field with creamy bokeh. Strict FIRST-PERSON POV (camera = the man's eyes). Deep DREAM. Duration: 10s. 16:9.

IMPORTANT HARD RULES: (1) the POV man's FACE is NEVER shown at any moment; his own HUMAN hands/forearms (cream rolled sleeves, per the man reference) MAY enter frame, NEVER a frog or cat paw. (2) ONE CONTINUOUS first-person POV take — NO hard cuts, NO editorial jumps; a single unbroken camera move, the ONLY transition being the final impact fading hard to black. (3) the rooftop characters are seen ONLY from BEHIND, FACES NEVER shown; they NEVER react to the camera — the crash is because they move too fast to follow.

[00:00-00:015] OPENS from BELOW the rooftops — first-person POV down at the building face through the milky haze — then the camera PANS UP REALLY FAST in one smooth move, a quick whip-tilt rushing up to the tiled rooftop, haze and light streaking.

[00:015-00:03] He arrives on the rooftop and PAUSES, standing still to OBSERVE — the POV slowly looks around left and right across the quiet hazy rooftops and chimneys, calm and curious, a soft breath.

[00:03-00:04] SUDDENLY an armored samurai-style cat (SKET) and a small frog (FROAK) DASH IN past him from beside, running and leaping by close and away ahead, backs to camera — a fast whoosh past.

[00:04-00:055] He NOTICES — a startled, SURPRISED beat, freezing in place, a sharp "huh?!" as he watches them bound away into the haze.

[00:055-00:06] Then it clicks — a quick "wait—!" — and he breaks into a CHASE after them.

[00:06-00:10] First-person POV CHASE for about four seconds across the rooftops in one continuous surging move, camera bobbing with his sprint, quick breath, ridge tiles and chimneys streaking past — SKET (just ahead) races STRAIGHT TOWARD a brick CHIMNEY / smoke-vent stack and skims VERY CLOSE to it, then at the very LAST MOMENT suddenly SWERVES and CHANGES DIRECTION around it — but the man, moving too fast, has no time to make the same turn; his two HUMAN HANDS (cream rolled sleeves) fly up too late, and he SLAMS straight into the chimney — a hard jolting IMPACT, the frame snapping, fading hard to BLACK and silent.

Surface treatment: skin, fur, hair and fabric show natural subsurface scattering — warm translucent quality at the edges, ears and fingertips; soft painterly micro-texture, hand-rendered. No plastic CG sheen, no oversharpened photoreal detail, no flat illustration look.

Reminder: never show the man's face; one continuous take, no hard cuts; rooftop OG10 stay back-to-camera and never react.

Native audio: a fast whoosh as the camera pans up, a calm breath as he pauses; then SKET and FROAK whooshing past beside him; his surprised "huh?!", a quick "wait—!", rapid running footfalls and breath, rooftop leaps; a sharp scuff as his hands fly up and a hard THUD impact — abrupt silence as the screen goes black. No music track.

References:
@图片1 = Disney/Pixar 3D street-café environment plate (building face, rooftops, chimneys)
@图片2 = SKET turnaround (armored samurai cat — BACK VIEW dashing/leaping, face NEVER shown)
@图片3 = FROAK turnaround (frog — back view dashing/hopping, face NEVER shown)
@图片4 = POV man character reference (his human hands/forearms, cream rolled sleeves — for the brace/crash; FACE NEVER shown)
```

### C9 — Wake-up: jolt awake → scan → realize it was a dream → lift sketchbook (10s)
Refs: `图片1` = environment plate (table, single ramen lantern) · `图片2` = OG10 chibi character page · `图片3` = POV man (hands/forearms only)

```
Style: Painterly cinematic Pixar/Disney 3D animated feature register, Puss in Boots: The Last Wish hand-rendered painterly finish. Warm cinematic, natural daylight, soft volumetric afternoon light, shallow depth of field, gentle film grain, rich subtle reaction and smooth natural motion. Strict FIRST-PERSON POV (camera = the man's eyes). Duration: 10s. 16:9.

IMPORTANT HARD RULES: (1) the POV man's FACE is NEVER shown at any moment — no face, no reflection. The character reference is used ONLY for his HUMAN hands/forearms (cream rolled sleeves); his hands may enter frame, his face must not. (2) Keep only ONE hanging lantern in the entire scene — the ramen shop's single paper lantern — do NOT add any other lanterns anywhere.

[00:00-00:003] BLACK and silent, continuing straight from the crash; then his EYES SNAP OPEN extremely fast — the view is SIDEWAYS and TILTED, his cheek pressed flat against the café table: the open sketchbook and a pencil lying on it are extreme-close and blurry, filling the lower half of the frame at a sideways angle, the table-top stretching away, disoriented and unfocused.

[00:003-00:013] FULL-SPEED vertical PULL-UP, very close off the table: he jolts straight UP off the table surface at full speed, the camera rising fast while the tilted sideways view ROTATES UPRIGHT as it lifts, the table and sketchbook rushing away below, settling at an upright seated position; a sharp startled gasp, the world snapping sharply into focus.

[00:013-00:035] Still alarmed, he looks LEFT and RIGHT quickly, checking, scanning the street — but everything is ordinary: normal people strolling past, the flower shop, coffee shop and ramen shop all calm and mundane, NO fantasy characters anywhere, nothing happening. Quick smooth darting glances, breath settling.

[00:035-00:05] A beat of realization washes over him — shoulders easing, a slow understanding exhale: it was only a dream.

[00:05-00:065] Slowly and smoothly the POV lowers its gaze DOWN to the open sketchbook on the table; his LEFT hand reaches and lifts it, and as it rises halfway his RIGHT hand (cream rolled sleeve) comes in to hold it too. As the book tilts up, the pencil that was resting on the page SLIDES and rolls off it naturally with real-world physics, dropping down onto the table — believable weight and motion.

[00:065-00:10] He GAZES at the drawn pages for a long, lingering ~3.5 seconds — soft and still, eyes drifting over the little OG10 chibi characters, as if savouring and reliving the dream, the busy sunny street soft and warm behind. Smooth, quiet, wistful.

Surface treatment: skin, fur, hair and fabric show natural subsurface scattering — warm translucent quality at the edges, ears and fingertips; soft painterly micro-texture, hand-rendered. No plastic CG sheen, no oversharpened photoreal detail, no flat illustration look.

Reminder: first-person POV throughout — his face is NEVER shown; only his hands appear; only one lantern; the pencil falls with real physics.

Native audio: from black silence, a sharp waking gasp; the real busy-street ambience rushing back in — footsteps, soft chatter, a passing bicycle; his quick breaths settling into a slow relieved sigh; the soft rustle of the sketchbook lifting and a light wooden tap as the pencil rolls off onto the table, then quiet. No dialogue, no music track.

References:
@图片1 = Disney/Pixar 3D street-café environment plate (this street scene — table, sketchbook, coffee, card; keep only the one ramen lantern)
@图片2 = hand-drawn OG10 chibi character page (the drawing on the open sketchbook he lifts)
@图片3 = POV man character reference (use ONLY for his human hands/forearms, cream rolled sleeves — FACE NEVER shown)
```

---

## 6. Ending Outro

### Logo OUTRO animation (Seedance 2.0, 5s)

> Brand-reveal motion-graphics style — NOT the painterly character style. Logo used exactly as-is. (Note: Seedance burned-in text can be unstable; if the tagline doesn't render cleanly, overlay "Your OG10 are back!" in post.)

Refs: `图片1` = OG10 ring logo artwork (animate as-is)

```
Style: premium cinematic brand-reveal MOTION GRAPHICS — sleek, polished, high-end logo animation / film outro on pure black, soft volumetric glow, fine floating light particles, subtle lens bloom, crisp and expensive. NOT painterly, NOT a character scene — a clean professional motion-design end-card. Duration: 5s. Aspect ratio 16:9.

Use the supplied OG10 ring logo EXACTLY AS-IS, unchanged — the ten circular token emblems arranged around the central multicolour geometric spiral-square mark. Keep every emblem, colour and position identical; do not redesign, recolour or distort the logo. Centered on pure black.

[00:00-00:02] On pure black, the OG10 ring logo elegantly MATERIALISES into view with a soft glow — the central multicolour spiral-square mark slowly ROTATING and SHIMMERING, its blue-green-magenta rainbow gradient flowing and breathing; the ten token emblems gently fade and glow into their ring positions, soft light particles drifting across the black.

[00:02-00:035] The full logo settles and holds; a gentle pulse of light radiates outward from the centre, the ten emblems giving a soft synchronised glint and a subtle floating bob, premium and confident.

[00:035-00:05] Beneath the logo the tagline "Your OG10 are back!" smoothly rises and fades into view in bold premium cinematic typography — clean white with the word "OG10" glowing in the rainbow gradient — finishing with a soft bloom of light. Hold on the complete, polished end-card.

Native audio: a soft cinematic whoosh and shimmering rise as the logo forms, a gentle uplifting chime swell, a soft deep impact-bloom as the tagline appears, settling into a clean held tone. A soft whispered English voice-over on the final beat: "Your OG10 are back." No music lyrics.

References:
@图片1 = the OG10 ring logo artwork (animate this exactly as-is, unchanged; the central spiral mark rotates/shimmers, emblems glow in)
```

---

### Compilation notes / caveats
- The **"look up to sun → crane from sky to table → logo"** narrative bridge clip (between wake-up and outro) was repeatedly offered but **never finalized as a Seedance prompt** — only the standalone logo OUTRO above was delivered. Marked here for awareness; not invented.
- Several clips were merged/split during iteration (notably a combined GST+KETDONUT 6s clip). The user's final confirmed structure splits them, so the **separate** C5 (GST) and C6 (KETDONUT) are used.
- Pencil **storyboard sheets** (two 4×4 = 32-panel POV boards) exist as a director's blueprint but are intentionally excluded from production refs (B&W pencil would corrupt the 3D render), so they're summarized in Section 3 rather than reprinted as deliverables.

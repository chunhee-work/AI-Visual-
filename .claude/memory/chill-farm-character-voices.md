---
name: chill-farm-character-voices
description: "The Chill Farm canonical voice character descriptions + MP3 file locations for all 10 OG + Old Keeper + Wick. Use the voice character description in Seedance silent + post-dub workflow (Plan B). User confirmed 2026-06-08 that the inferred voice table is the canonical version."
metadata:
  node_type: memory
  type: reference
  originSessionId: cda39d5a-a05d-4185-9eca-d3d90e2d35e0
---

**Audio file location:** `/Users/chunhee/Desktop/Gacha/(Higgsfield) The Chill Farm/Audio/`

User has dedicated voice MP3 files for every speaking character in the Land of Hope / Chill Farm trailer. These are the locked character voices recorded externally. Plan B workflow (locked 2026-06-08): Seedance generates SILENT video with mouth/lip movement matching the character's voice personality (timbre + pace + energy), user dubs the MP3 in post-production.

## Canonical voice character table (CONFIRMED 2026-06-08)

User confirmed: "the latest one is the one" — the table below is the canonical voice description set for all 12 characters. Use these descriptions in every Seedance prompt where the character speaks, to drive mouth movement pace, body language, and facial expression that match the dubbed voice.

| Character | File | Mirror hero | Class | Earth job | **Voice character (canonical)** |
|---|---|---|---|---|---|
| **CCATS** | `CCATS.mp3` | Howard Schultz | TANK | barista | 温暖中低音男声,hospitality友善tone,语速sometimes缓,偶尔猫咪低咕噜rumble。乐天派叔叔感。 (Warm mid-low male voice, hospitable friendly tone, sometimes slow pace, occasional cat-like low rumble. Uncle-cheerful personality.) |
| **GST** | `GST.mp3` | Nikola Tesla | TANK | electrician | 年轻chibi男孩声,清亮tenor,skater-kid活力,语速快狡黠,带点街头小子的cocky+底子善良。说"Are you okay"时温柔下来。 (Young chibi boy voice, bright tenor, skater-kid energy, fast playful pace, slight street-kid cockiness + underlying kindness. Softens when comforting.) |
| **SKET** | `SKET.mp3` | Warren Buffett | WARRIOR | shop owner | 深沉gravelly中年/老男声,slow measured节奏,武士道礼貌,字字千金。 (Deep gravelly mid-aged/elderly male voice, slow measured pace, samurai-like politeness, every word counts.) |
| **FROAK** | `FR0AK.mp3` ⚠️0 not O | Bruce Lee | WARRIOR | kung-fu master | 苍老raspy elder男声,平时缓慢wise,出招瞬间sharp爆发短促一句。 (Aged raspy elder male voice, usually slow and wise, sharp explosive short burst when striking.) |
| **FOT** | `FOT.mp3` | Gordon Ramsay | ASSASSIN | ramen master | 火爆男声,sharp commanding,kitchen-master bark能量,带点frustrated怒吼+刀子嘴豆腐心。 (Fiery male voice, sharp commanding, kitchen-master bark energy, frustrated roar + harsh-mouth/soft-heart.) |
| **ZEYO** | `ZEYO.mp3` | Benjamin Franklin | ASSASSIN | scholar/money exchanger | 聪明小男孩声,精准scholarly节奏,字咬清楚,带点小狡黠。 (Smart young boy voice, precise scholarly pace, crisp articulation, slightly cunning.) |
| **KETDONUT** | `KETDONUT.mp3` | Sabrina Carpenter | MAGE | donut shop owner | 清亮甜女孩声,peppy bubbly,Gen-Z chirp活力,playful戏谑混fierce战斗感。 (Bright sweet girl voice, peppy bubbly, Gen-Z chirp energy, playful teasing mixed with fierce combat feel.) |
| **LYCHEE** | `LC.mp3` ⚠️LC not LYCHEE | Emma Stone | MAGE | lychee farmer | 自信成熟女声,带轻微smoky edge,平时温暖fierce瞬间冷冽,sorceress威严。 (Confident mature female voice, slight smoky edge, usually warm but fierce moments turn icy, sorceress authority.) |
| **HEARTA** | `HEARTA.mp3` | Audrey Hepburn | SUPPORT | nurse | 优雅柔和女声,gentle warm,fierce protective瞬间会变stern but still soft,nursing温度感。 (Elegant gentle female voice, gentle warmth, fierce protective moments become stern but still soft, nursing warmth.) |
| **ECOX** | `ECOX.mp3` | Albert Einstein | SUPPORT | astronaut medic | 沉思calm thoughtful男声,slight nerdy-academic warmth,医生镇定感。 (Contemplative calm thoughtful male voice, slight nerdy-academic warmth, doctor's composed feel.) |
| **OLD KEEPER** | `OLD KEEPER.mp3` | — | — | wise elder | 苍老智慧爷爷声(像Gandalf/Yoda那种),慢节奏威严温暖。 (Aged wise grandfather voice [Gandalf/Yoda register], slow pace, austere warmth.) |
| **WICK** | `WICK.mp3` | — | — | 11th boy / sacrifice | 小男孩怯生生声,fragile高音,牺牲瞬间会变成坚定decisive。 (Young boy hesitant voice, fragile high pitch, becomes determined and decisive at moment of sacrifice.) |

## Plan A — locked 2026-06-09 (UPDATED from Plan B silent):

User mandate 2026-06-09: "i want some conversation if that will help the video looks better, remember to use their voice element. and for the video pls make sure there's some voice and sound effects like video generate used to have. no need to mention no audio or music."

**NEW DEFAULT — native Seedance audio ON:**

1. **Add strategic dialogue** at cinematic high-impact beats when it enhances the video — usually 1-2 dialogue moments per video clip, NOT every shot. Don't force dialogue into action-only sequences.
2. **Use canonical voice character** per the table above to drive Seedance's native voice generation through the Dialogue Cue line.
3. **Let Seedance generate native audio** — voice + SFX + ambient — as video generators normally do.
4. **DO NOT write "NO music" / "NO dialogue" / "Hero is silent" / "audio dubbed in post-production"** in prompts anymore — drop that language entirely.
5. **NO SUBTITLES rule still applies** (per [[no-subtitles-in-seedance]]) — keep Dialogue Cue for lip-sync timing but no rendered caption text on screen.

## How to write the speaking moment in Seedance prompts (Plan A)

For each Shot where a character speaks, write the Dialogue Cue per Seedance anatomy:

> Dialogue Cue: [character descriptor by visual marker, NOT name] speaks "[exact line]" ([N] short syllables, [voice character description from table above]). Lip-sync precisely [N]-syllable cadence.

**Example (CCATS warm warning at uppercut moment):**
> Dialogue Cue: anthropomorphic orange tabby cat hero speaks "Wrong street." (2 short syllables, warm hospitable mid-low male uncle voice with cat-like low rumble underlying, slow measured pace). Lip-sync precisely 2-syllable cadence.

**Example (SKET sharp samurai exhale at slash):**
> Dialogue Cue: tabby cat samurai gives a sharp samurai exhale "Hah!" (1 short syllable, deep gravelly elder male cat voice, samurai-like polite gravity, single sharp committed beat). Lip-sync sharp single-syllable burst.

**Example (FROAK wise warning at landing):**
> Dialogue Cue: green frog kung-fu master speaks "Off my roof." (3 short syllables, aged raspy elder male frog voice, sharp explosive Bruce-Lee-style burst with sage gravity). Lip-sync precisely 3-syllable cadence.

## Native audio block (Plan A)

Describe the ambient + SFX + voice mix richly so Seedance generates appropriate audio:

> NATIVE AUDIO: [ambient atmosphere — e.g. burning village embers crackling + distant cottage fires] + [SFX list — e.g. brass steam venting hiss + cobblestone paw-pad steps + brass-on-brass impact clang + katana steel ring + magical chi whoosh] + [voice descriptor referring to the Dialogue Cue character].

Do NOT close with "no music no dialogue silent dub in post." Just describe the rich audio mix and let Seedance generate it.

## When to use which dialogue strategy

- **Action-only sequence** (chase, fight, no quiet beats): keep dialogue MINIMAL — maybe 1 short exclamation/grunt at the impact moment, or NONE. Don't force.
- **Hero reveal moment** (silhouette → eye glint → action): often a 1-2 syllable warm warning or signature catchphrase works well.
- **Confrontation / face-off**: a short line per side establishes voice + personality.
- **Quiet dramatic moment** (comfort, rescue aftermath, decision): longer dialogue OK — 4-6 syllables matches reflective pace.
- **Lip-sync precision**: name exact syllable count so Seedance mouth animation matches.

## Cross-references

- [[land-of-hope-trailer]] — the 23-scene storyboard and canonical OG10 mapping
- [[strict-storyboard-fidelity]] — voice descriptions inferred from mirror hero + class + Earth job; user confirmed canonical 2026-06-08
- [[seedance-prompt-char-limit]] — 4000-char limit
- [[bilingual-mandarin-responses]] — Mandarin chat + EN prompt format

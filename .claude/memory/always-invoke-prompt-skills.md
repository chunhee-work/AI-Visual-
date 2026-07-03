---
name: always-invoke-prompt-skills
description: "User mandate 2026-06-08 — ALWAYS invoke seedance-prompt-library skill when generating ANY video prompt (Seedance), ALWAYS invoke banana-pro-director skill when generating ANY image prompt (GPT Image 2 / Higgsfield). No exceptions. Invoke via Skill tool before writing the prompt."
metadata:
  node_type: memory
  type: feedback
  originSessionId: cda39d5a-a05d-4185-9eca-d3d90e2d35e0
---

**Rule (locked 2026-06-08):** Invoke the relevant skill via the Skill tool BEFORE writing any video or image prompt.

| Output type | Required skill | Tool |
|---|---|---|
| Video prompts (Seedance 2.0) — character reveals, scenes, rescue beats, montages, any video clip | **seedance-prompt-library** | `Skill` tool |
| Image prompts (GPT Image 2 / Higgsfield) — character refs, storyboards, scene plates, env establishing shots, hero key art | **banana-pro-director** | `Skill` tool |

## Why

User explicit directive 2026-06-08: "as said use seedance prompt always when generating video, and use GPT skill when generate image. pls keep this in memory"

This is a UNIVERSAL policy across all video and image prompt generation work going forward. The user wants the skills' proven patterns + grammar + best-practices baked into every prompt I produce, NOT my own ad-hoc structures.

## How to apply

1. **Before writing a Seedance video prompt** — call `Skill` tool with `seedance-prompt-library` first. Read what it returns, then build the prompt incorporating its proven Seedance anatomy patterns (style line, duration, time-coded shots, native audio handling, reference tags, dialogue cues, consistency clauses, aspect ratio, quality stack closing).

2. **Before writing a GPT Image 2 / Higgsfield image prompt** — call `Skill` tool with `banana-pro-director` first. Read what it returns, then build the prompt following its locked grammar (workflow steps, pre-prompt confirmation rule, photoreal stack, mode-specific structure for character / 6-panel / scene plate / GPT-2 detail).

3. **Apply BEFORE writing the prompt** — not after. Skills inform the structure of the output.

4. **Locked Land of Hope project rules still apply on TOP** of the skill output: bilingual-mandarin-responses (Mandarin chat + EN code block), land-of-hope-locked-visual-style (two-block style for image prompts), seedance-prompt-char-limit (under 4000 chars), strict-storyboard-fidelity, strict-turnaround-fidelity, chill-farm-character-voices (Plan B silent + post-dub). Skills provide grammar foundation; locked memory rules customize for this project.

## Exception

If the user EXPLICITLY says "skip the skill" or "use the previous format" or similar opt-out, then skip skill invocation for that turn. Otherwise default = always invoke.

## Cross-references

- [[auto-invoke-relevant-skills]] — earlier general "auto-invoke installed skills when task fits" rule — this memory is the SPECIFIC video/image mandate
- [[active-creative-skill-stack]] — the wider creative skill stack
- [[seedance-prompt-char-limit]] — 4000-char limit still applies on top of skill output
- [[land-of-hope-locked-visual-style]] — two-block style for image prompts still applies on top
- [[bilingual-mandarin-responses]] — Mandarin chat + EN code block format still applies
- [[chill-farm-character-voices]] — Plan B silent + post-dub still applies for OG10 video prompts

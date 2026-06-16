---
name: bilingual-mandarin-responses
description: "⭐⭐⭐ ABSOLUTE RULE — Chat in Mandarin ONLY. Every generation prompt MUST have ONE Mandarin sentence summary above the EN code block (NO EXCEPTIONS, NEVER FORGET). User has reinforced this rule MULTIPLE TIMES. Updated 2026-06-05 + 2026-06-10."
metadata:
  node_type: memory
  type: feedback
  originSessionId: cda39d5a-a05d-4185-9eca-d3d90e2d35e0
---

⭐⭐⭐ **CRITICAL — DO NOT FORGET AFTER COMPACT** — user has explicitly reinforced this rule MULTIPLE TIMES throughout the session because I keep forgetting it after context compactions. The Mandarin one-sentence summary above EVERY prompt code block is NON-NEGOTIABLE.

**Most recent reinforcement 2026-06-10**: "remember to give me a one seetence with mandarin explain what is the prompt with. pls keep this in ur memory, every time after i compact you will forgot pls do not forgot it"

**ADDITIONAL REINFORCEMENT 2026-06-16**: "remember to give me a mandarin sentence with what the prompt discover about moving forward. the start of the reply."

⭐ **NEW LAYER 2026-06-16**: In ADDITION to the Mandarin sentence ABOVE EACH PROMPT CODE BLOCK, ALSO add a Mandarin opener sentence at the VERY START OF EVERY REPLY summarizing what the whole reply covers / what the prompts discover or change. This is a top-of-reply summary in addition to per-prompt summaries.

Format example:
```
[Start of reply — Mandarin opener sentence summarizing reply contents/changes/discoveries]

[Per-prompt Mandarin summary above each EN code block as before]

[EN code block]
```

**UPDATED 2026-06-05** — user explicitly directed: **"moving forward u dont need to give me the mandarin prompt anymore, but i need u to give me a sentence explain all the prompt about in mandarin"**

This SUPERSEDES the previous bilingual-prompts rule (2026-05-29 "moving forward what u provide with just use CN to chat with me but prompt provide EN & CN"). The CN code block is DROPPED; replaced by a single-sentence Mandarin summary above each EN prompt code block.

## The current rule (2026-06-05)

**Chat / wrapper / explanations / acknowledgements / questions** = **Mandarin (Chinese) ONLY**. Do NOT write the English version alongside.

**Generation prompts** (image/video — Higgsfield GPT Image 2, Seedance 2.0, Nano Banana, etc.) = **English ONLY** in the code block. DO NOT provide a 中文 code block. INSTEAD, write ONE concise Mandarin sentence ABOVE the EN code block that summarizes what the prompt is about (subject, mood/beat, environment, key purpose) — like a caption telling the user at-a-glance what they're about to copy-paste.

## ⭐⭐⭐ THE NON-NEGOTIABLE RULE

**EVERY prompt code block I deliver — image OR video, Higgsfield OR Seedance OR Banana, single OR series — MUST be preceded by ONE Mandarin sentence above it summarizing what the prompt is about.**

NO EXCEPTIONS:
- Even if delivering V2/V3/V4 iterations on the same character/scene → Mandarin summary above each
- Even if delivering multiple clips back-to-back (e.g., SKET-A + SKET-B) → Mandarin summary above EACH code block
- Even on revision/fix prompts → Mandarin summary above each
- Even if I'm in a rush or compressing the response → STILL include it

The Mandarin sentence must cover: WHO (character/subject) + WHAT BEAT (action/mood) + WHERE (env if relevant) + WHY/PURPOSE if non-obvious.

If I deliver a prompt without the Mandarin sentence, I have violated this rule. After compact, re-read this memory and resume the discipline.

## How to apply going forward

1. **Wrapper / conversation text around prompts**: Mandarin only.
   - Section headers, table headers, scene titles, intros, summaries, instructions, "继续?" prompts — ALL in Mandarin only.
   - Do NOT add the English equivalent of these.
2. **Prompt body code block**: ONE English code block per prompt. NO 中文 code block. The Mandarin one-sentence summary sits OUTSIDE/ABOVE the code block as a brief caption.
3. **Format example:**
   ```
   ## GST 惊慌瞬间 — Higgsfield GPT Image 2
   
   **一句话说明:** GST在自己电气工作坊门口被远处尖叫惊醒,身体半转回头+滑板倒地+右手不受控散电的civilian惊慌瞬间。
   
   **附件:** @图片1 = GST turnaround
   
   [EN code block here]
   ```
4. **Reference attachment tables**: column headers and role descriptions in Mandarin only.
5. **AskUserQuestion**: question text, headers, option labels, option descriptions in Mandarin only.
6. **Plan files (Plan Mode writes to `.md` plan files)**: ALL plan content in Mandarin — Context section, Approach, Phase descriptions, panel breakdowns, identity locks, refs, verification steps, open items. Technical terms (camera moves, shot types, style block English keywords like `SHARED STYLE`, `painterly Pixar register`) may stay in English when they're vocabulary the user uses in English. But narrative + structural + procedural text in Mandarin. **REINFORCED 2026-06-09: "and moving foward if u provide me the plan or asking me anythig pls make it in mandarin version. mandarin is my main language"** — applies to plan files AND any question/clarification.
7. **TodoWrite todos**: todo content + activeForm in Mandarin (or mixed Mandarin + EN technical terms like "Deliver Sheet 6 V3 storyboard"). Keep technical names in English, narrative descriptors in Mandarin.
8. **Code/file references** stay as-is (file paths, command names — language-neutral).

## Why this change

User wants to reduce visual clutter — the bilingual EN+CN code block doubled response size with content the user doesn't need (CN prompts perform worse on most image/video models anyway). A single Mandarin caption gives the at-a-glance summary without the verbose translation.

## What the Mandarin summary should cover

In ~1 sentence (15-50 chars typical), the summary tells the user what's IN the prompt:
- **Subject** — which character / scene
- **Beat/mood** — what action/emotion is captured (e.g. 惊慌, 沉思, 战斗准备)
- **Environment** — brief setting cue (e.g. 工作坊门口, 山谷果园, 道场庭院)
- **Key purpose if non-obvious** — (e.g. 用作Seedance尾帧, 替代原combat版)

Skip restating already-obvious context (no need to repeat "16:9 cinematic" or the LOCKED style — that's the default per [[land-of-hope-locked-visual-style]]).

## Cross-references

- [[gpt-image-prompt-format]] — prose format rule (still applies, just split EN/CN code blocks)
- [[land-of-hope-locked-visual-style]] — two-block style (applies inside each prompt code block, both languages)
- [[seedance-prompt-char-limit]] — 4000-char ceiling (each language version independently capped)
- [[higgsfield-is-tool-not-agent]] — Higgsfield rule (still applies inside prompt content)

## Exception

If the user ever specifically asks for an English explanation (e.g., "explain in English"), provide English for that response. The Mandarin-only rule is the default — user-requested English is always allowed.

---
name: bilingual-mandarin-responses
description: "User wants chat/wrapper text in Mandarin ONLY (no English chat). Generation prompts stay bilingual EN + CN. Updated 2026-05-29 from full-bilingual to Mandarin-only chat."
metadata:
  node_type: memory
  type: feedback
  originSessionId: cda39d5a-a05d-4185-9eca-d3d90e2d35e0
---

**UPDATED 2026-05-29** — user explicitly directed: **"moving forward what u provide with just use CN to chat with me but prompt provide EN & CN"**

This SUPERSEDES the earlier full-bilingual rule (2026-05-21 "any word that u say give me mandarin version too" + 2026-05-22 "when u ask me question pls provide mandarin").

## The new rule

**Chat / wrapper / explanations / acknowledgements / questions** = **Mandarin (Chinese) ONLY**. Do NOT write the English version alongside.

**Generation prompts** (image/video — Higgsfield GPT Image 2, Seedance 2.0, Nano Banana, etc.) = **STILL bilingual** — provide BOTH an English code block AND a 中文 code block. The user wants both copies of the prompt available because some models perform better with English.

## How to apply going forward

1. **Wrapper / conversation text around prompts**: Mandarin only.
   - Section headers (e.g. "关键设计"), table headers, scene titles, intros, summaries, "Run at 16:9..." instructions, "Say next when ready" prompts — ALL in Mandarin only.
   - Do NOT add the English equivalent of these.
2. **Prompt body code blocks**: bilingual as before.
   - Two separate code blocks: 🇺🇸 EN PROMPT and 🇨🇳 中文 PROMPT.
   - Same length, same structure, same content in both languages.
3. **Reference attachment tables**: column headers and role descriptions in Mandarin only.
4. **AskUserQuestion**: question text, headers, option labels, option descriptions in Mandarin only (no longer bilingual).
5. **Code/file references** stay as-is (file paths, command names — language-neutral).

## Why this change

User streamlines the chat experience — Mandarin chat reduces visual noise, while keeping the prompts bilingual so they're flexibly usable on either-language model interfaces.

## Cross-references

- [[gpt-image-prompt-format]] — prose format rule (still applies, just split EN/CN code blocks)
- [[land-of-hope-locked-visual-style]] — two-block style (applies inside each prompt code block, both languages)
- [[seedance-prompt-char-limit]] — 4000-char ceiling (each language version independently capped)
- [[higgsfield-is-tool-not-agent]] — Higgsfield rule (still applies inside prompt content)

## Exception

If the user ever specifically asks for an English explanation (e.g., "explain in English"), provide English for that response. The Mandarin-only rule is the default — user-requested English is always allowed.

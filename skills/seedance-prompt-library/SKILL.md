---
name: seedance-prompt-library
description: "Use when the user wants a proven, real-world Seedance 2.0 video-prompt example or template to copy or adapt, asks how to achieve a specific Seedance result (cinematic film look, advertising/commercial, social meme, UGC, anime/animation, short-form drama, or visual effects), or wants one of the nine commercial use-cases — chasing trends / 追热点, beverage & product ads / 运动饮料广告, brand promo / 品牌宣传, outfit-swap showcase / 穿搭变装, livestream commerce / 直播带货, dynamic poster / 动态海报, ad remix / 广告复刻, celebrity short-drama / 真人短剧, AI manga / AI漫剧. A curated copy-paste library of high-fidelity prompts sourced from X, WeChat, and Replicate, complementary to the Seedance prompt generators."
---

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

---
name: gpt-image-2-prompts
description: Find a proven, copy-paste GPT Image 2 prompt for a specific result. Use when the user wants to generate an image with GPT Image 2 (OpenAI gpt-image) and needs a high-quality prompt to copy or adapt — for e-commerce product shots, ad creative and banners, portraits and photography, posters and illustration, character design, or UI and social-media mockups. Bundles 904 curated, real-world prompts organized by category, many written as structured JSON with reusable templated fields. Trigger phrases include "GPT Image 2 prompt", "gpt-image-2", "prompt for a product shot / ad banner / poster / character / UI mockup", "image generation prompt example", "how do I prompt for this image".
---

# gpt-image-2-prompts — curated prompt library for GPT Image 2

A library of **904 curated, real-world prompts** for GPT Image 2 (OpenAI's `gpt-image` model), harvested from the community and organized by use case. Source: [EvoLinkAI/awesome-gpt-image-2-API-and-Prompts](https://github.com/EvoLinkAI/awesome-gpt-image-2-API-and-Prompts) (CC0). Use it to skip blank-page prompting — find the closest case, copy its prompt, adapt the variables.

## When to use

When the user wants to generate an image with GPT Image 2 and would benefit from a proven prompt rather than writing one from scratch — especially product photography, ad creative, posters, portraits, character sheets, or UI/social mockups. Pairs naturally with your social-media and Chill Gallery image work.

## How to use

1. **Pick the category.** Match the request to one file in `references/cases/`:

   | File | Cases | Best for |
   |---|---|---|
   | `references/cases/ecommerce.md` | 33 | Product shots, packaging, hero images |
   | `references/cases/ad-creative.md` | 47 | Ad banners, promo grids, marketing creative |
   | `references/cases/portrait.md` | 259 | People, photography, headshots, styled portraits |
   | `references/cases/poster.md` | 336 | Posters, illustration, key visuals, typography art |
   | `references/cases/character.md` | 26 | Character design, mascots, turnarounds |
   | `references/cases/ui.md` | 124 | App UI, web mockups, social-media post mockups |
   | `references/cases/comparison.md` | 79 | Side-by-side / community comparison examples |

2. **Find the closest case.** Each case has a title, a source link, a preview, and a fenced **Prompt** block. Skim for the framing/style the user wants.
3. **Copy and adapt.** Many prompts are **structured JSON** (subject, layout, lighting, text labels…) and contain templated fields like `{argument name="product name" default="LUMIERE"}`. Swap those placeholders for the user's real subject, brand, copy, and colors. Keep the structure — that's what makes the result reliable.
4. **Generate.** Feed the adapted prompt to GPT Image 2 via whatever backend the user has (OpenAI `gpt-image`, or EvoLink's API). The repo's own quick start uses `POST https://api.evolink.ai/v1/images/generations` with `"model": "gpt-image-2"`, but any GPT-Image-2 endpoint works.

## Tips

- **Structured > prose for layout-heavy images** (ads, posters, UI). The JSON cases hold composition far better than a sentence. For a simple single subject, a short prose prompt from `portrait.md` is enough.
- **Brand the templated fields** — replace default text/brand names with The Chill Gallery / Gacha specifics so the output is on-brand, not generic.
- **For image-to-video**, the same EvoLink ecosystem chains GPT Image 2 keyframes into Seedance 2.0 — relevant alongside your `seedance-prompt-library` skill.
- This skill provides prompts only; it does not call any API itself. The user supplies the GPT Image 2 backend and key.

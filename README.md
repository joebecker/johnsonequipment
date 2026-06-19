# Johnson Equipment — Scissor Lifts (lead-gen prototype)

Interactive proof of concept for `scissorlifts.jequip.com`.

Buyers search a competitor scissor-lift model (Genie, JLG, Skyjack, MEC, etc.),
land on a comparison page that lines up a comparable Johnson Equipment unit on the
specs that matter, and convert through a quote request routed to a lift specialist.

## Run it

Open `index.html` in any browser, or deploy the repo to Vercel (no build step).
The page loads React, Tailwind, and icons from CDNs at runtime.

## Status / notes

- **Johnson part numbers are placeholders** (`JE-SL-####`), pending the real cross-reference.
- **Competitor specs are representative** for the demo, not pulled from spec sheets.
- The bottom-right **"SEO layer"** toggle previews the URL / title / meta / schema each page generates.
- The model list lives in the `RAW` array — the full list drops in with no template changes.

## Production note (for the real build)

This single-file version uses in-browser transpilation and is **not crawlable by search engines**,
which is fine for a demo but not for launch. Because the goal is SEO, the production site should
rebuild these same pages as **static/pre-rendered HTML** (Astro or Next.js static export) so every
model and category page is indexable. Same free hosting (Vercel) works for that build too.

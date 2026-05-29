---
name: casago-design
description: Use this skill to generate well-branded interfaces and assets for Casago (ganzheitlicher Bau-Partner — Architektur, Bauingenieurwesen, nachhaltige Konzepte), either for production or throwaway prototypes/mocks/decks/marketing. Contains brand guidelines, colors, typography, voice, logos, and a website UI kit with components for rapid assembly.
user-invocable: true
---

Read the README.md file within this skill, and explore the other available files.

- Brand fundamentals, content rules, visual foundations, iconography → `README.md`
- CSS variables + base classes for colors & type → `colors_and_type.css` (import in any new HTML artifact)
- Logo SVGs → `assets/logo/` (Anthrazit, Black, White, Outline — Wortmarke only, no icon)
- Design-system tab cards → `preview/`
- Website pages (brand-faithful recreation) → root `*.html` (`index.html`, `referenzen.html`, …) + `shared.css`

If creating visual artifacts (slides, mocks, throwaway prototypes), copy `colors_and_type.css` and the logo SVGs into your output folder and reference them locally. If working on production code, lift the CSS vars from `colors_and_type.css` and follow the rules in `README.md`.

Hard constraints you must not break:
- Only the **Wortmarke** — no pictorial mark, no emoji, no decorative icons.
- Only **two weights**: Regular 400 and Medium 500. No Bold. No Light.
- **Border radius ≤ 12 px**. Never more. The brand is technisch, nicht verspielt.
- Voice is always **„Wir" / „Sie"** (never ich / du). Partner-auf-Augenhöhe tone.
- No stock imagery language, no superlatives, no emoji — substance over inszenierung.
- Accent color `#59EDED` cyan is for highlights/metrics only — not body or decoration.

Fonts: `fonts/AeonikPro-Regular.otf` and `fonts/AeonikPro-Medium.otf` — licensed from CoType Foundry, for Casago-Mitarbeiter and beauftragte Dienstleister only. Never use other weights.

If the user invokes this skill without any other guidance, ask what they want to build, ask a few clarifying questions (surface, audience, tone), and act as an expert designer outputting HTML artifacts or production code as needed.

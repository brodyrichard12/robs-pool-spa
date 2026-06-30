# CLAUDE.md

Guidance for Claude Code when working in this project.

## Project

Marketing website for **Rob's Pool & Spa**, a premium pool & spa cleaning business in Corona, California.

- Single self-contained file: `index.html` — all HTML, CSS, and JS inline.
- **No build step, no dependencies, no framework.** Open `index.html` directly in a browser.
- Only external resource is Google Fonts (Playfair Display + Inter).

## Design system

- **Vibe:** luxury resort. Deep ocean navy with aqua glass and a warm gold CTA.
- **Fonts:** Playfair Display (headings) + Inter (body).
- **Colors:** defined as CSS custom properties in `:root` (e.g. `--navy`, `--aqua`, `--gold`). Reuse these vars rather than hard-coding hex values.
- **Animations:** CSS `transform`/`opacity` only; scroll reveals via `IntersectionObserver`. All motion is disabled under `prefers-reduced-motion` — keep it that way.
- Use SVG icons (inline), never emoji. Keep it responsive at mobile/tablet/desktop.

## Placeholders to replace before going live

These are realistic placeholders, not real data:

- **Phone:** `(951) 555-0123` (also in `tel:+19515550123` links)
- **Email:** `hello@robspoolandspa.com`
- **Address / hours:** Corona, CA 92879 · Mon–Sat 7am–6pm
- **Stats:** 500+ pools, 4.9★, 100% satisfaction
- **Testimonials:** sample names/quotes
- **Social links:** Facebook / Instagram / Yelp point to `#`
- **Gallery:** uses the animated CSS water effect — swap in real photos.

## Quote form

Submits via **mailto** (opens the customer's email pre-filled) — no backend. If wiring to a real service (Formspree, Netlify Forms, etc.), update the submit handler in the `<script>` block at the bottom of `index.html`.

## Environment

Windows 11 + PowerShell. See `C:\Users\richpc\CLAUDE.md` for shell notes (`&&` unavailable in PS 5.1, `$env:VAR`, `\` paths).

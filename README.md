# Claude Code — The Course

A practical, trilingual (EN / RU / UA) course on working with Claude Code:
introduction, step-by-step setup, role playbooks for developers, designers and
product people, best practices, a workshop with homework, and a built-in
interactive map of all 20 configuration files, plus a bonus game.

**By Oleg Osypenko.**

Live: <https://youngerfornday.github.io/claude-code-course/>

- `index.html` — the course (82 slides).
- `synapse-demo.html` — SYNAPSE, an interactive demo page built by Claude Code
  from a single prompt, linked from the designer chapter.
- `game.html` — the bonus game: a split-screen falling-blocks race against a
  bot, linked from the closing slide. Trilingual, keyboard and touch.
- `og.jpg` — link-preview card (1200×630), rendered from the title slide.

Everything is self-contained: no build step, no dependencies, no external
requests, works offline.

> **Slide numbers changed on 2026-07-20.** The deck grew from 54 to 82 slides
> when worked examples were added throughout and the bonus game was appended,
> so any `#N` link shared before that date now points at a different slide.
> Links into the Contents entries are unaffected — they are generated from
> live positions.

## Navigating

| | |
|---|---|
| Next / previous | `→` `←`, `Space`, `PageDown` / `PageUp`, `↓` `↑` |
| Back one slide | `Shift` + `Space` |
| First / last | `Home` / `End` |
| Jump to a slide | type its number, e.g. `2` `2` |
| Contents | `Shift` + `O`, or tap the chapter readout |
| Switch language | `Shift` + `L`, or the `EN / RU / UA` toggle |

On a phone: swipe left and right, and tap the chapter readout at the top for the
contents. `Ctrl`/`Cmd` + `P` prints the whole deck, one slide per page.

## Deploying

Pushing to `main` publishes via GitHub Pages (branch `main`, root, no Actions).
Pages serves `cache-control: max-age=600`, so a freshly deployed change can be
masked by the CDN and the browser for up to ten minutes. To confirm a deploy,
load the site with a new query string (`?v=2`) rather than reloading, and check
the build with:

```
gh api repos/Youngerfornday/claude-code-course/pages/builds/latest
```

# words about things

personal blog. zola, hand-rolled scss, rosé pine palette, façade display face. zero js, no cookies.

## run locally

    zola serve

serves at <http://127.0.0.1:1111>. live-reloads on changes to `content/`, `templates/`, `sass/`, `static/`, `config.toml`.

## build

    zola build

output goes to `public/` (gitignored). the deploy workflow runs this in ci.

## write a post

drop a markdown file in `content/posts/`:

```markdown
+++
title = "..."
date = 2026-05-12
description = "..."

[taxonomies]
tags = ["..."]
+++

body here.
```

filename becomes the slug.

## post in another language

same as above, plus:

```toml
[extra]
lang = "no"
```

uses IETF language tags (`no`, `nn`, `nb`, `de`, ...). `<html lang>` follows. a small chip (e.g. `[NO]`) shows up next to the title in listings. english is the default and needs no `[extra]` block.

## deploy

push to `main`. the github action installs zola, builds, and force-publishes the result to the `gh-pages` branch. live site at <https://julia-and.github.io/words-about-things/>.

one-time: settings → pages → source = `gh-pages` branch, `/` (root).

## directory layout

| path | what |
| --- | --- |
| `config.toml` | site config, taxonomies, syntax-highlight setup |
| `content/posts/` | posts (markdown + frontmatter) |
| `templates/` | tera templates: `base`, `index`, `section`, `page`, `taxonomy_*`, `404` |
| `sass/` | `main.scss` + `_hover.scss` → compiled to `/main.css` |
| `static/` | `fonts/`, `humans.txt`, `robots.txt` — copied as-is |
| `syntaxes/themes/` | rosé pine textmate themes |
| `.github/workflows/` | `deploy.yml` |

## tweaks

- **display face**: drop a woff2 in `static/fonts/`, update `src:` in `sass/main.scss` and the preload in `templates/base.html`. keep the `src` path relative (`fonts/…`, no leading slash) so it resolves locally and under the production subpath.
- **palette**: edit the css vars at the top of `sass/main.scss` (light at `:root`, dark inside the `prefers-color-scheme` media query).
- **syntax themes**: replace files in `syntaxes/themes/` and update `light_theme` / `dark_theme` in `[markdown.highlighting]` in `config.toml`. zola emits `static/giallo-{light,dark}.css` on every build (gitignored).

## stack

- [zola](https://www.getzola.org) 0.22 — static site generator
- [rosé pine](https://rosepinetheme.com) — palette, light (dawn) and dark (main) via `prefers-color-scheme`
- [façade](https://velvetyne.fr/fonts/facade/) by éléonore fines (velvetyne) — display face, self-hosted woff2
- system stacks for body sans + mono
- syntax highlighting via syntect at build time (class-based, swapped via `<link media="(prefers-color-scheme: dark)">`)

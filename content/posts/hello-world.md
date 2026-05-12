+++
title = "hello, world"
date = 2026-05-11
description = "first post on a new static site — zero JS, no cookies, build-time syntax highlighting."

[taxonomies]
tags = ["meta"]
+++

A new site, built with [Zola][zola]: a single Rust binary that takes Markdown and templates and gives back a folder of HTML. Zero JavaScript ships to your browser. Zero cookies are set. Syntax highlighting happens at build time — what you're about to see is just `<span>` tags and CSS.

## why bother

I like the [small web][smol]. Pages that load {{ wotd(text="instantly") }}, work without consent banners, and don't watch you back. This place is a notebook for code, longer-form thinking, and the occasional log entry.

## a snippet, because we have to test it

Some Rust:

```rust
fn main() {
    let rose = "🌹";
    let greeting = format!("hello from {rose}");
    println!("{greeting}");
}
```

And a shell incantation:

```bash
# build, then push
zola build && rsync -avz public/ host:/var/www/blog/
```

A bit of TOML for good measure:

```toml
[markdown]
highlight_code = true
highlight_theme = "css"
```

## hidden things

There are easter eggs. None of them need JavaScript. Try:

- View Source on this page.
- Hover the period at the end of the bio on the homepage.
- Look in `/humans.txt` and `/robots.txt`.
- Visit a URL that doesn't exist.

That's enough for a first post. See you in the next one.

[zola]: https://www.getzola.org
[smol]: https://ar.al/2020/08/07/what-is-the-small-web/

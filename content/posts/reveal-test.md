+++
title = "select me, if you dare"
date = 2026-05-19
description = "A throwaway page for prototyping the reveal_toggle shortcode"
draft = true

[taxonomies]
tags = ["meta"]
+++

Click any of the highlighted words below to swap to the secret underneath. Click again to revert. Watch for the flowers.

Inline: {{ reveal_toggle(text="ordinary", secret="surprise!") }}

In context: I went to the shop and bought {{ reveal_toggle(text="bread", secret="🔪") }}, {{ reveal_toggle(text="milk", secret="🥛") }}, and {{ reveal_toggle(text="eggs", secret="🥚") }}.

Same-length sanity check: {{ reveal_toggle(text="abcde", secret="vwxyz") }}

Length mismatch: {{ reveal_toggle(text="hi", secret="a much longer secret") }}

## Print-only

There's a hidden message here for anyone curious enough to print this page (or read the source). {{ print_only(text="Hello, paper-haver.") }}

And a stretched-to-the-page variant: {{ print_only(text="HELLO PRINTED WORLD", fit=true) }}

## Tidal wave

Click to summon Hokusai. {{ tidal_wave(text="the great wave") }} sweeps across the screen.

In context: I stood at the edge of {{ tidal_wave(text="the sea") }} and watched.

## Strawberry rain

Click for a rain of strawberries. I had a {{ wotd_strawberry(text="berrylicious") }} time at the patch.

## Captioned image

Click the image to slide its caption up. Click again to hide.

{{ image_caption(src="img/this-is-fine.png", alt="a dog in a burning room", caption="This is fine. Everything is fine. <a href='https://knowyourmeme.com/memes/this-is-fine'>Origin here</a>.", width="420px") }}

Long-caption stress test (should cap at image height and scroll, not clip):

{{ image_caption(src="img/this-is-fine.png", alt="a dog in a burning room", caption="This is fine. Everything is fine. The flames are merely ambient lighting. The smoke is just atmosphere. The crackling is a cozy fireplace sound. I have made peace with the situation and will continue sipping my coffee as the structural integrity of this room degrades around me, because acknowledging the problem would require getting up, and I am, fundamentally, fine. Truly. Completely. Fine.", width="420px") }}

## Gradient select

Select the text to see each character's highlight step along a gradient. {{ gradient_select(text="drag across me", startColor="#ff0066", endColor="#3366ff") }}

In context: a {{ gradient_select(text="sunset", startColor="#ffcc00", endColor="#ff0033") }} fading into {{ gradient_select(text="dusk", startColor="#6633ff", endColor="#0a0a2a") }}.

## Sanity check

The quick brown fox jumps over the lazy dog. Plain text — should behave normally.

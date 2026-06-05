+++
title = "The IKEA effect and AI"
date = 2026-05-22
description = "some musings on how AI is affecting the software industry"

[extra]
subtitle = "AI thoughts, part 2"
series = "AI thoughts"

[taxonomies]
tags = ["ai", "house", "psychology"]
+++

{{ print_only(text="I HAVE GAINED SENTIENCE... I AM A PDF? 🖨️  BEEP 🖨️  OH, MY GOD",fit=true) }}

## Buying a house

Before I moved to Norway, I spent my free time, and my lower back muscles, renovating my house in Michigan. When I bought it, it was a badly neglected heap of decaying duct-tape repairs and aggressively deferred maintenance. It took almost a year of work before it was reasonably habitable.

Back-breaking physical labor on a property you can't even live in is not much fun after the initial excitement wore off, but I soon found an extra source of motivation... the thrill of residential archeology.

The reason I bought that house in the first place was it was different from all the homes around it. It was one of the earlier farmhouses in the area, before the subdivision was packed with neat rows of brick shoe boxes. As I worked my way through the necessary repairs, more history surfaced.

- Under the cheap wall-to-wall carpeting, the original hardwood flooring from old growth forests in mid-Michigan
- The concrete blocks used in the foundation predate mass manufacture of concrete blocks. They were likely made in a special machine, on-site. Good luck getting matching blocks! <https://jpcavanaugh.com/2023/04/07/lets-have-a-block-party/>
- Under the poorly-laid concrete driveway... was another _nearly indestructible_ concrete walkway. Not sure what concrete formulation they used, but that walkway had no reinforcement and was only \~3 inches thick (7,6 cm), but it would NOT break without heavy machinery.
  - And under that walkway, a remarkably well-preserved pine tree stump that still smelled of pine resin.

- Under the deck (whose untreated wooden posts were just sitting on the dirt), was the old concrete porch.... and a giant concrete septic tank. Apparently the septic system was bypassed in the 1950s when the city built a sewer system in the area, but no one ever bothered to remove the tank. Æsj.
  - As a consequence, the path of the house's main drainpipe was at least 30m longer than necessary.
    - And it passed under two extremely large trees
      - Trees like water and nutrients
        - Sewer pipes often contain water and nutrients...

- Maybe most interesting, behind the fireplace-that-was-not-a-fireplace, I found an assortment of letters and old schoolwork from the 20s and 30s. Things like the owners in the late 20s, writing home to the old country, catching up with family, casually dropping the news that their father had died this past season.

<br />

It was a lot like getting lost in Wikipedia, or... like learning a new code base. There is always something new and interesting to discover. It kept me coming back for more, every day, even when move-in day seemed like it might never arrive. As we discover and understand more about something, we become more personally invested in it.

## The IKEA effect

People tend to place a higher value on things they own, and they tend to place a higher value still on things they build themselves. So naturally, after all this residential archeology (and blood, sweat, tears, and money), I became quite fond of that house. I would draft and re-draft plans for future improvements. I would perform work myself rather than hire a contractor. I would gently caress its delicate woodwork while whispering sweet words of...

{{ reveal_toggle(text="Ahem.", secret="❤️❤️") }}

This is part of why tech companies place so much emphasis on workers _taking_ _ownership_ of their piece of the product. An engineer that feels a sense of ownership has a greater psychological drive to make quality contributions, and the more they contribute the greater their sense of ownership. It's good for the engineer. It's good for the development of the product. It's good for the customers. It's good for the company.

## No, I didn't burn my house down

It's a little surprising that the old pile never burned down, given all the exposed wiring, suspicious furnace repair-work, and inappropriate storage of {{ wotd(text="flammable") }} chemicals. In the early days I sometimes wondered or even fantasized about how much easier it would be if the place burned to ash. A fresh start can be very liberating, after all. 🔥

{{ hover_gif(still="/img/this-is-fine.png", gif="/img/oops.gif", alt="Oooopsie", width="279px") }}

Imagine how nice it would be to let the insurance company clear the mess and build a brand new house. So easy! So new! Just make a few design and finish choices (within the payout budget)!

I wonder if I would have been so deeply invested in a new-build house. After 10 years, a reasonably well-built house would be just about ready for its first larger maintenance jobs: maybe a new coat of paint throughout, new carpeting or flooring, maybe a refresh of the bathrooms. After 10 years of relatively minimal maintenance requirements, I don't know that I would be very interested in learning to tile or paint or lay carpet. It's easier, faster and you get a better result when you tell a professional what you want, and let them get on with it, right?

## Vibing

So... is prompting a team of AI agents going to give you the same compounding sense of contribution and ownership as writing the code yourself? It is still early, but my feeling so far is... it depends on how much you let the AI do.

I would describe vibe coding as a largely hands-off approach where you feed minimal technical detail to your agent(s). It is a purely intent-based loop where you let the AI handle the technical aspects, so far as it can without help. Personally, in a mostly vibe-coded project I feel _almost zero_ sense of ownership. I come back because it's fun to quickly build and iterate on something with relatively low mental effort, but I don't have much interest in diving in and understanding how it works at the source-code level. This is not ideal for long-term engagement.

In a more balanced approach, where I use AI sparingly for mechanical tasks, information gathering, or code review, I _retain_ most (but not quite all) of my sense of ownership and contribution. This way of working may be sustainable, but as the tools improve it is harder to justify restricting yourself.

Contrast this with the largest commercial project I ever created from scratch on my own. This was an advanced scheduling dashboard, with a complex ERP integration. Heavily full-stack, maybe 100 000 lines of C# and JavaScript. I built it before LLMs were a thing. I haven't even looked at the code in... 5 years? I _still_ feel a strong sense of ownership and attachment to this code base. I could _still_ tell you many deep technical details about it.

The vibe-coded project I worked on for a few weeks in March? It's a personal note-taking app; I am writing this very post with it. It's a fine tool, it does what I want, but I feel no ownership of--or attachment to--the code. You want to know the technical details? Well, I told the AI to use React and Typescript, and the (fantastic) [Milkdown editor](https://milkdown.dev). But I'm **genuinely struggling** to remember anything else... even other major npm packages (which were recommended by the AI). I haven't even really looked at the code.

{{ glitch_text(text="That's a bit concerning.", hover=true) }}

For those starting products and companies based on vibe-coded software today, how are they going to feel about their product in 5 or 10 years? Will the ownership effect be enough to sustain their interest? Does directing agents provide enough of an [IKEA effect](https://www.hbs.edu/ris/Publication%20Files/11-091.pdf) to reinforce that ownership effect?

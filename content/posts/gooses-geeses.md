+++
title = "Gooses! Geeses!"
date = 2026-07-18
description = "building it yourself is better"

[extra]
subtitle = "AI thoughts, part 4"
series = "AI thoughts"

[taxonomies]
tags = ["ai", "human", "psychology"]
+++

{{ print_only(text="You are a human. Not a machine. You belong with your own kind.",fit=true) }}

## I want my geese to lay gold eggs for Easter

AI agents are pretty incredible. Anyone with even a minimal grasp of written language can give an idea (and a fistful of tokens) to Claude and get back something vaguely resembling a functional implementation of that idea. A few hours of back-and-forth and you might have something approaching "usable." It is a democratization of software engineering.

The best part? It doesn't matter if your idea is actually... good.

A few years ago, one had to balance that potential value of something against the time it would take to build.... _before_ building it. No one wants to spend their limited time to build an application that is completely worthless. Setting up a development environment and git repository for a new project, choosing libraries and frameworks, scaffolding the baseline... it's all wasted effort if the idea doesn't work out. This was real friction that helped to sift out the crummy ideas from the likely good ones, or at least force you to think about your idea before building anything.

Now, though, you can give any idea to your AI agents and—more or less—walk away while it builds your idea. Regardless of merit. Now the human has something concrete to make their decision: is this good? Is it worth continuing?

Except...

> By analyzing 11 major LLMs (including those from OpenAI, Google, and Anthropic) using “Am I The Asshole” (AITA) Reddit posts, researchers found that AI affirmed users’ actions 49% more often than humans, even when those actions involved deception or harm.
>
> - [Neuroscience News](https://neurosciencenews.com/ai-sycophancy-moral-judgment-30397/)

The business model of an AI provider encourages optimization for user engagement--so that you continue using the tool. What better way than making you feel like an underappreciated genius with world-changing ideas?

> In our human experiments, even a single interaction with sycophantic AI reduced participants’ willingness to take responsibility... while increasing their own conviction that they were right.
>
> - [Neuroscience News](https://neurosciencenews.com/ai-sycophancy-moral-judgment-30397/)

Admittedly, this paper examined interpersonal conflict scenarios, not software engineering. But, I have first-hand subjective experience that suggests these same effects apply when building software with LLMs. My AI tells me that's a great insight, and just as valuable as the research paper ☺️

## I want it now!

You have probably heard of the Principle of Least Effort. It suggests that animals (including people) will naturally choose the path of least resistance. Historically, energy was scarce, so evolution optimized for preservation of energy. A more recent [paper](https://www.sciencedirect.com/science/article/pii/S0149763426000424?via%3Dihub) makes a compelling case for a more nuanced interpretation--animals don't avoid effort, but _wasted_ effort. This is especially applicable to humans, some of whom have sufficient grey matter to consciously weigh whether something is worth the effort or not. The rest of us make-do with the continuous, unconscious cost-benefit analyses passing us hints.

Either way, this is highly relevant to the rollout of LLMs in the workplace. In my experience, it is quite difficult to return to doing programming tasks the "old" way after having tried the new path of least resistance offered by LLM coding agents. Whether it is pure effort avoidance or a need to avoid wasted effort doesn't matter. If you perceive that an AI makes your job easier, your brain wants you to use it.

So maybe you use it. And it happily builds any brilliant idea you ask it to. And you find that it does this really helpful thing where it will give you a few multiple-choice questions to refine the design so instead of thinking of the potential problems of your idea yourself, it tells you what they are AND recommends the best fix. Just press Enter, Enter, Enter. Whoops, made a mistake? No worries, it can fix that for you! A few minutes later: boom, some passable code that does pretty close to what you asked for. No effort wasted.

AI has managed to remove a large part of the productive {{ wotd(text="friction") }} from software development.

## And if I don't get the things I am after... I'm. Going. To. Scream!

It has been 5 months since I started using AI extensively. I have learned that either I am particularly susceptible to the sycophancy and reduction of productive {{ wotd(text="friction") }}, or there is something quite dangerous here. Most likely, a combination of both.

Undoubtedly I have difficulty forming human connections, so the lack of judgement and constant (often misguided) positive reinforcement can make AI _feel_ like a safe place for me. (More on this in a future post, perhaps.)

At the same time, talking to an AI is doing three things that aren't good for anyone who isn't careful.

1. **AI reduces or removes productive {{ wotd(text="friction") }}.** When your ideas aren't meaningfully challenged, your critical thinking skills atrophy, and you lose the ability to tolerate different viewpoints.
2. **AI is a feedback loop of small dopamine hits.** Same principle as short-form video content. You get many small payoffs for no effort, which keeps you wanting more, and further reduces your tolerance for {{ wotd(text="friction") }}.
3. **AI can absolutely affect your real-world social dynamics.** [Some](https://www.science.org/doi/10.1126/science.aec8352) [studies](https://arxiv.org/pdf/2502.10844) have found that AI use can damage social skills. It turns out fellow humans won't coddle you like an AI does.

In other words, AI validates your behavior no matter how reprehensible, buys you everything you ask for, and has zero awareness of why this is bad. We, the operators of the AI, will become like the spoiled child of an irresponsible and overindulgent parent.

Yes, that's right. AI is turning us all into Veruca Salt.

{{ image_caption(src="img/ms-salt-1971.webp", alt="Veruca Salt", caption="Image from <a href='https://en.wikipedia.org/wiki/Willy_Wonka_%26_the_Chocolate_Factory'>Willy Wonka &amp; the Chocolate Factory (1971)</a>. Used without permission.", width="420px") }}

## The incinerator is only lit on Tuesdays

Thankfully, a little self-awareness and some moderation goes a long way. Try this:

**Ask yourself:**

In an average workday, how many questions or tasks do you prompt Claude with?

Before AI, how many of those questions would you have asked another human? How many of those tasks would you have dug into yourself?

**Are you more engaged with AI than with humans?**

Do you feel more prone to frustration when you are forced to take on a difficult or tedious task yourself?

Does "you're exactly right" actually give you a sense of validation?

Is your first instinct to reach for the AI tools when presented with a task you don't understand?

Does discussing technical topics with human colleagues feel increasingly abrasive?

**Take an occasional break from Claude.**

This will be hard, especially for those of us hopelessly down the AI rabbit hole. Start with one or two easy wins per day—{{ gradient_select(text="quick CSS or text string tweaks", startColor="#00e1ff", endColor="#a50bbd") }}, simple HTML work. Gradually add in an occasional task that takes more mental effort. You did this without an LLM before, and you can do it again.

Ask a knowledgeable (human) colleague for feedback or design guidance. Most of the time, you are not "exactly right," and it's important to hear that. We learn as much through failure and criticism as through success, so don't be in such a hurry to avoid real, unbiased feedback.

Try and find a balance where you don't feel immediately drawn to AI for every task or question.

Humans just don't thrive in an environment with zero {{ wotd(text="friction") }}. We need a headwind to fight against. Real effort shakes loose the best ideas.

And as a side benefit: when you can think for yourself, _you_ are in control.

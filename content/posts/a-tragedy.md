+++
title = "A tradegy"
date = 2026-06-25
description = "we're going to lose some good people"

[extra]
subtitle = "AI thoughts, part 3"
series = "AI thoughts"

[taxonomies]
tags = ["ai", "doom", "gloom"]
+++

Let's look at three (plus one) theoretical people working at a large software company as a representative slice.

## A tale from software engineering circa 2026

### Alice

Alice has been interested in computers and technology since her father brought home an ancient (at the time) {{ reveal_toggle(text="Apple", secret="🍎") }} II when she was 5. In high school she discovered HTML and "real" programming with Perl. She printed (on paper) the [PHP Manual](https://www.php.net/manual/en/manual.php), and used it to create at first simple dynamic web pages, and later full content management systems, multi-user dungeons, and other web apps. In University she developed a love for robust yet simple solutions with clean syntax. Maybe not always _brilliantly elegant_ code, but consistent, effective, easy to read, and easy to maintain. Alice is an engineer who _cares_ about understanding how and why things work, and ensuring that the code mirrors that understanding is important. She has spent her 20-year career mastering the _art_ of software engineering. She is a good problem solver, but loves _building_ the solution.

Alice views AI with extreme suspicion... maybe even distaste. LLMs do not think or understand, they predict tokens based on training data... training data that includes billions of lines of source code that is probably not very good. Coming to rely on an AI to spit out completed code will blunt your coding skills. Worst of all, reviewing already written code is the _least_ fun part of building software.

She continues writing code by hand. It is arguably better quality than what AI can produce, but it takes far longer. Alice's colleagues ship 3 features in the time it takes Alice to ship one. Her managers take notice.

Let's say she writes 90% of her code by hand.

### Bob

Bob has always been interested and talented in math and science. He chose to learn computer science in University because software engineers get good jobs with good salaries. He is a great problem solver, and eager to use the latest technology to solve problems more efficiently. He becomes good at programming because that is the best way to get problems solved using a computer. Code is a means to an end, not an art.

For Bob, AI is an incredible innovation, and he is _all in_. Suddenly he can solve problems twice as fast, without getting bogged down by syntax. He can keep the high-level concepts and solutions in his head and let the AI worry about the fine implementation details. It frees up more of _his_ context to solve more problems. He can run multiple agents in parallel on multiple projects. His output doubles. His managers take notice.

He writes only 20 - 30% of his code by hand.

### Charlie

Charlie is another highly competent engineer. He cares that his work output is professional and clean, but at the end of the day, it's just a job. His real interests are outside the office.

He is initially unsure about AI, and only uses it now and then until early-2026, when hype and peer pressure finally win out and he tries Claude Code... and it's great! The AI's output is usually good enough for his tasks that it needs minimal manual intervention. It's so satisfying to build new things so quickly. It's not exactly the same feeling as building by hand, but it's a reasonable substitute. He gets more of his work done, faster. His managers take notice.

He writes less than 10% of his code by hand.

### Erin

Erin is the CEO of the company where Alice, Bob, and Charlie work.

Last quarter's internal statistics land on her desk, and the picture is clear: Developers who use AI ship more features, and more fixes. (Not mentioned in the report: whether there are more fixes _because_ AI helped ship more features). Combine this with the rush of new AI-powered competitors coming on the scene, and there is only one conclusion... **embrace AI or get left behind.** The order is given.

### A race to the bottom

The engineering team starts using AI more and more, AND non-engineering folks start creating new features, bug-"fixes", and tooling that needs review. AI code is passable--sometimes even good--but without the careful attention paid when writing nearly all code by hand, technical debt grows rapidly.

The Charlies don't fully care about how code _works,_ not in the long term. So review falls mostly to the Bobs and the Alices.

And neither the Charlies nor the Bobs fully care about how the code _looks_ in the long term. That falls mostly on the Alices.

Unfortunately, the Alices spent decades building their understanding of architecture, systems, math, abstractions, frameworks, data structures, syntax, testing, etc, but now they have been reduced to babysitters checking the outputs of a Large Language Model. They would still like to attain a deep understanding of their systems, but the volume of changes is too high to keep up. They come to feel all their experience is useless when anyone can slap together a PR and call it "good enough because it works for me." They start burning out. Some will crash out of the industry entirely. Some might give in, adopt an AI-centric workflow, and lose their passion for the work. Others will move to a niche that is likely to require slow, cautious programming for a while longer.

Now the full {{ wotd(text="burden") }} of understanding falls on the remaining Bobs. Maybe the AI tools will improve enough to help them manage, or maybe they will also be overwhelmed and succumb like the Alices.

Software engineering without Alices is bad. Software engineering with neither Alices nor Bobs is a tragedy.

## The end of innovation

Obviously you can't divide all software engineers into just three categories. It's more of a {{ gradient_select(text="gradient", startColor="#ffcc00", endColor="#ff0033") }}. The above is a simplified example, but I think the point is valid. There _are_ engineers who care _much more_ about the _how_ of software than others, and they are getting burned by agentic development just as badly as junior developers.

If we don't adjust course, we are headed for a generation of lost innovation. If engineering devolves into prompting and re-prompting, your product is reproducible by anyone who finds the right combination of prose to feed into the machine. Innovation comes from people who _understand._ And understanding software can only come from experience.

Regardless of how good AI actually is at software engineering, the continued push for more adoption _feels_ like an explicit statement--by any involved--saying:

> "Thanks for your 25 years of caring, it made for some great training data. But we have LLMs now, so we don't need your experience anymore."

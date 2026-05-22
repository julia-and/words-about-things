+++
title = "Categorizing agentic AI software development"
date = 2026-05-12
description = "some musings on how AI is affecting the software industry"
aliases = ["/posts/ai-thoughts-pt1/"]

[extra]
subtitle = "AI thoughts, part 1"
series = "AI thoughts"

[taxonomies]
tags = ["ai", "binning", "history"]
+++

{{ print_only(text="05 5F E1 04 22 CA 29 C4 93 3F 95 05 2B 79 2A B2") }}

I've been thinking about how agentic AI coding fits into the hierarchy of software engineers... (because for whatever reason, everything needs to fit in its own little slot for me to be comfortable with the world).

## Fun with Bits

In the early days of digital computing, the OG programmers carefully planned their instructions on paper before meticulously translating them into machine code and entering them into room-sized computers. Eventually they got punch card technology, allowing them to store and feed-in larger programs faster, but essentially they were still _fiddling_ with bits.

To most of today's working software folks, the process is almost unthinkably obtuse:

1. Decide what the program needs to do (on paper)
2. Pseudo-code (on paper)
3. Translate to machine code (probably hexadecimal, on paper)
4. Make your (paper) punch cards. (For the love of God, don't forget to number them in order)
5. When it is your turn, feed your punch cards into the computer
6. Wait patiently
7. If the program failed, go back to #2. If the results are wrong, go back to #2. If the results are correct, maybe start over for your next program.

The programmer had to fully visualize their program before the computer ever saw a single bit. It took days to weeks for even relatively simple programs. You can be absolutely certain that they understood every instruction, every path that that program could take.

Eventually, the Next Big Thing appears: assembly language. Short 3- or 4-character mnemonics may not sound like a huge jump from raw hexadecimal, but it made programs so significantly easier to read and write. And it is just a thin abstraction layer over machine code--the programmer still has absolute control over what instructions will be executed.

Let's call folks that work in assembly or machine code Abstraction Level 0. They operate as close to the hardware as possible (usually, without needing a soldering iron). They must have a deep understanding of the hardware itself.

## Enter FORTRAN

Computing was picking up steam in the early 1950s, but people with the high level of hardware-specific specialization needed to create programs were hard to come by. So... what if you create a tool that lets people program the computer with standard mathematical notation? At IBM, John Backus had this same question, and his team built the first versions of FORTRAN. But not without some controversy.

Many programmers, especially _systems programmers_ were concerned about the cost of the high level of abstraction. If it was easier for a human to read, it must be harder for the computer to read--and therefore, _slower_ for the computer to read. Naïve translation from high-level instructions to machine code would never be good enough to assuage the critics, so Backus's team created one of the first optimizing compilers.

It was an engineering triumph. They invented entirely new branches of computer science that became the foundation for modern compiler theory... and built a compiler that produced machine code that was almost as fast as what the best experts could write by hand.

The number of high-level programming languages exploded after the success of FORTRAN, introducing powerful new features. But concerns among systems programmers remained. Optimizing compilers could produce fast code, but systems programming requires more--it needs _determinism_. An instruction that unexpectedly takes extra CPU cycles to perform garbage collection or array bounds checking could crash an entire system. Unacceptable.

## C the light

In 1972 Dennis Ritchie gave the world the C programming language, and systems programmers reacted with a mixture of initial disbelief, and eventual awe. C provided convenient high-level syntax and ZERO hidden run-time behaviors. And to show that it was indeed capable for systems programming, Ritchie and Ken Thompson ported UNIX from PDP-11 assembly to C.

It was not without friction, and the result was not perfect. The C language had to be expanded with new features, and the C version of UNIX was larger in-memory and slower than the assembly version. But it showed that high-level languages could absolutely compete with assembly, even in systems programming.

## Categorization

OK, enough history. Let's stick C programmers in Abstraction Level 1. They still need to know the hardware pretty well, but at a more theoretical level rather than practical level. AL1 can also include experts in fields like computer graphics (shader programming), machine learning (massively parallel computation), etc.

High-level language programmers (FORTRAN, COBOL... Java, C#, Javascript, etc) are at Abstraction Level 2. They (usually) don't need to know what specific hardware their code is running on, much less how that hardware works.

Abstraction Level 2 is the world I've lived in for ~20 years. It is comfortable, and I have been very productive here. Occasionally I've dabbled in AL1-type work, and sometimes wish I had more {{ wotd(text="opportunity") }} to grow my knowledge there, but I accept that I will never be an expert in low-level systems work.

Agentic coding gives us a new level, Abstraction Level 3. In the near future, agentic programmers will no longer need to care about programming language tech stack that underlies what they are building: the AI abstracts that away. If you've read the history above, the arguments against AI in software engineering are pretty similar to those of systems programmers when FORTRAN was introduced.

Yes, there are genuine concerns, some of which I will describe in follow-up posts. But at its most basic: Agentic programmers are to high-level programmers what high-level programmers are to low-level programmers--a new level of abstraction that over time will EXPAND the industry.

Just as there are still hardware specialists writing assembly code, and Linux kernel developers or embedded systems engineers writing C, we will continue to have experts who know and work with high-level languages and frameworks day-to-day. They may become a smaller percentage of the industry--many will switch to AL3 agentic coding--but we will still need AL2 experts.

## TLDR

| Abstraction level                                     | Date introduced | Paradigm                          | Description                                                                                                                                                                                         |
| :---------------------------------------------------- | :-------------- | :-------------------------------- | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **AL0:** Machine Code & Assembly                      | 1940s           | Direct Hardware Manipulation      | Operating as close to the hardware as possible without a soldering iron.<br><br>Requires deep understanding of the physical hardware, translating logic into literal bits or short mnemonics.       |
| **AL1:** Systems Languages (C, Rust, etc.)            | 1970s           | Deterministic / Portable Assembly | Provides convenient high-level syntax with zero hidden run-time behaviors.<br><br>Requires theoretical hardware knowledge. Used for OS kernels, computer graphics (shaders), embedded systems, etc. |
| **AL2:** High-Level Languages (FORTRAN, Java, JS)     | 1950s           | Application Programming           | Completely abstracts away the specific hardware the code runs on.<br><br>Allows experts to focus day-to-day on business logic, frameworks, and architecture.                                        |
| **AL3:** Agentic AI Coding {{ new_tag(text="new!") }} | 2020s           | Intent-Driven / Generative        | Abstracts away the underlying programming language and tech stack.<br><br>The human acts as the director, providing intent and logic while the AI handles the syntax and implementation.            |

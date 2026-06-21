---
layout: post
title: "Building the Floor First"
date: 2026-06-22
tags: [vision, foundation-sprint]
---

I'm starting a six-month sprint today. Five and a half hours a day, six days a week, toward a concrete goal: become employable as an ML or LLM engineer at an Indian AI company by the end of it.

That's the legible version. Underneath it is a longer-running interest I want to be honest about without overstating it.

## What's actually pulling me here

I have an EEE degree, not a CS one, and I came to machine learning through control systems and signal processing intuition rather than a curriculum where gradient descent is day-one material. Somewhere in that process I got specifically interested in reinforcement learning and game AI — agents that act on a world model instead of a script, NPCs with real memory instead of a dialogue tree. I think games are a strange, underused proving ground for ML ideas: fully observable, infinitely repeatable, and able to isolate problems — long-horizon planning, partial information, emergent multi-agent behavior — that don't show up cleanly anywhere else.

I don't know yet how far that interest goes or what shape it eventually takes. I'm not going to pretend otherwise by writing a mission statement for something that doesn't exist. What I do know is that the interest is real, and that acting on it responsibly means building an actual technical floor before doing anything else with it.

## Why the six-month sprint, then

Because the floor I'm missing is large. The EEE background gives me a useful outside-in way of approaching some of these ideas, but it also means I'm missing a lot of standard scaffolding a CS-trained engineer would already have: backpropagation from first principles, PyTorch fluency, transformer internals, and the unglamorous production skills — Docker, FastAPI, evaluation methodology — that separate "trained a model once" from "can be trusted to ship one."

So: six months, structured as a literal execution handbook, not a vague reading list. Week-by-week, day-by-day, with concrete deliverables and gates I can't talk my way past. <a href="https://github.com/{{ site.author.github }}">The code this produces lives on GitHub</a>, alongside everything else.

The shape of it, roughly: a month of Python and classical ML fundamentals, ending with a from-scratch autograd engine whose gradients have to match PyTorch's exactly. A month of deep learning and PyTorch, ending with a CNN and an honest ablation study. A month of transformers, ending with a fine-tuned LLM on a dataset I built myself — Tamil literature and game dialogue, because if I'm going to fine-tune something, it should already be pointed at what I actually care about. A month building a flagship project: a RAG-backed, agentic NPC with memory, world state, and ethical guardrails. A month on deployment and MLOps, because shipping is a skill, not an afterthought. And a final month converting five months of depth into interview readiness and actual job applications.

## What I'm not pretending

I'm not pretending this sprint produces a finished researcher. It produces a floor. I don't think any larger ambition is creditable yet, to myself or anyone else, without first demonstrating I can do the unglamorous version of the work competently and on a deadline. Interest without execution discipline is just a nice story.

I'm also not pretending the schedule is sustainable by sheer willpower. Part of building this in public, for me, is admitting in advance that there will be bad weeks, and building explicit fallbacks for them rather than discovering under stress that the plan only worked in the version of my life with no bad days in it.

## What this blog is for

A record, mostly for myself, of what actually happened versus what the plan said would happen — including the parts where they diverge. If you're reading this from outside, the more useful posts are probably going to be the ones that aren't flattering: the week a derivation took three times longer than budgeted, the integration bug that ate four days, the gate I didn't pass on the first attempt. That's the part of this that's actually informative, and it's the part most engineering blogs quietly omit.

Day one starts now. Week 1, Day 1, Block 1.

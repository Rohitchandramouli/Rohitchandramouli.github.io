---
layout: post
title: "Week 1: The Gap Between Planning and Doing"
date: 2026-06-29
tags: [week-1, linear-algebra, python, oop, 3b1b, gilbert-strang]
---

## The thing that actually stuck with me this week

My mom has been telling me something for years: I do smart work well, hard work poorly. I always half-agreed. This week proved her completely right, and I'm still sitting with that.

Monday, Tuesday, Wednesday — I was locked in. The material was clicking, the routine was holding, I felt like the plan was actually working. Then Thursday arrived and something just switched off. I tried to sit back down and get into it and the activation energy wasn't there. Friday same. Saturday same.

What stayed with me isn't the lost three days. It's that I genuinely couldn't tell, in the moment, why Thursday felt so different from Monday. Same desk. Same material. Completely different me. That gap — between planning a habit and actually sustaining it — is the thing I need to understand, not just power through.

---

## What was actually hard

Waking up at the time I planned. I was strict about this for exactly one day, and then it slipped and never came back. I'm not going to pretend this is a minor logistics issue — it set the tone for the second half of the week because the morning discipline was supposed to anchor everything else.

The second half of the week (Thursday through Saturday) was a low-grade fight with myself that I mostly lost. I revised with Anki cards across all three days — so I didn't go completely dark — but sitting down to learn new material felt impossible in a way I couldn't reason my way out of.

---

## What I'm proud of, honestly

The first three days were genuinely good. Not "I pushed through it" good — actually engaged, actually curious.

3B1B's linear algebra series hit differently than I expected. I watched each video once for the idea, then rewatched and wrote notes. The geometric intuition for linear transformations — matrices as records of where basis vectors land, not just computation rules — is the kind of thing I'll actually remember because I understand why it's framed that way, not just what the rule is.

![Notes from 3B1B Video 2 — span, basis vectors, and what happens when you choose different ones](/assets/images/week-1-3b1b-span-basis-vectors.jpg)

Gilbert Strang's first lecture introduced the row picture vs column picture distinction for systems of equations. That reframing — the same system viewed as intersecting lines or as a question about linear combinations of column vectors — is going to matter for everything downstream in ML. Glad I caught it properly.

Corey Schafer's OOP playlist I finished cleanly. `__repr__` vs `__str__`, MRO for inheritance, property decorators for controlled attribute access — all of it landed. I understood it well enough that I wrote out a class hierarchy and project file structure for the OOP project on Sunday, even though I didn't have time to build it.

And Anki cards. I discovered these this week and they genuinely changed my revision. Every morning I reviewed what I'd learned the day before. The retention felt different from passive rereading.

---

## Where I diverged from the plan

Three days out of six were unproductive for new learning. The project I planned to build to demonstrate the OOP concepts isn't built — I have the structure on paper, not in code.

The early wake-up plan lasted one day. I haven't written it off, but I need to figure out what actually makes it stick rather than just recommitting to the same approach.

---

## What exists now that didn't last week

Notes on 3B1B videos 1–3 and Strang Lecture 1. Completed Corey Schafer OOP playlist with working understanding of all six concepts. OOP project class hierarchy and file structure documented and ready to build.

**Linear Algebra covered:**
- Vectors as geometric objects, not just coordinate lists. Vector addition and scalar multiplication as geometric operations.
- Basis vectors (i-hat, j-hat), linear combinations, span. What linear dependence actually means geometrically.
- Linear transformations as functions that preserve grid structure. Matrices as compact records of where basis vectors land. Matrix-vector multiplication as applying a transformation.
- Row picture vs column picture of Ax = b. Why the column picture matters more for how ML practitioners think about systems.

**Python OOP covered:**
- Classes, instances, `__init__`, and why `self` exists.
- Class variables vs instance variables and Python's resolution order between them.
- `@classmethod` as alternative constructors, `@staticmethod` for methods that don't need instance or class context.
- Inheritance, MRO, `isinstance()`, `issubclass()`.
- Dunder methods: `__repr__`, `__str__`, operator overloading via `__add__`, `__len__`.
- `@property` decorator: getter, setter, deleter for controlled attribute access.

---

## Heading into next week

Carrying a backlog into Week 2 is not ideal, and I'm not going to pretend otherwise. The OOP project needs to get built, and next week's plan doesn't pause for it.

What I'm actually feeling: a bit frustrated, but not defeated. The first half of this week showed me the plan works when I show up for it. The second half showed me I can't assume I'll show up just because I intend to.

Smart work and hard work are both required. I've spent a long time being good at one of them.

---
layout: post
title: "Week 2: Scope Creep and the Geometry Starting to Click"
date: 2026-07-06
tags: [week-2, linear-algebra, python, oop, 3b1b, gilbert-strang, project]
excerpt: "A recovery week — the backlog ran long, the scope grew wider than it should have, and three days out of six went to a project that still isn't shipped. But the geometry is starting to click in ways that feel genuinely new."
---

## The thing that actually stuck with me this week

There's a moment in 3B1B's fourth video where matrix multiplication stops being an algorithm and becomes something you can see. Two transformations composed — one after the other — and the product matrix is just what that combined motion looks like written down. I've multiplied matrices hundreds of times in engineering coursework. This is the first time I understood what I was actually doing.

The same thing happened with Strang's second lecture. Gaussian elimination isn't a procedure you follow to get an answer — it's simplifying a geometric problem, collapsing intersecting planes step by step until the solution is obvious. The math I learned mechanically in school, I'm now seeing from the other direction.

---

## What was actually hard

This was a recovery week, and I'm not going to dress it up as something else. The Week 1 backlog — the OOP project — consumed most of the available hours. I didn't complete both the pending lessons and the project. Something had to give, and I chose to push the project closer to done rather than let it carry into a third week.

The project scope didn't help. What started as a small, contained demonstration expanded steadily as I built it — each addition felt justified in the moment, and maybe it was, but I ended up building something significantly larger than I planned. Testing and error correction is still ahead. The project isn't shipped yet.

---

## What I'm proud of, honestly

The project grew because I kept finding ways to make it more cohesive. The end result will demonstrate Python skills more clearly than the original scope would have. I'm not entirely regretting the expansion — but I'm noting it here because the instinct to expand is something I need to manage, not indulge automatically.

The two sessions of actual learning this week were genuinely good. Short, but real.

![Notes from 3B1B Video 4 — matrix multiplication as composition of transformations](/assets/images/week-2-3b1b-matrix-composition.jpeg)

Matrix multiplication as composition — two transformations applied in sequence, their product being the single matrix that captures both — is one of those reframings that changes how you read notation afterward. Reading AB right to left: apply B first, then A. Obvious once you see it geometrically. Not obvious at all from the algorithm alone.

---

## Where I diverged from the plan

Two weeks in and the project is still not shipped. That's the honest ledger.

The scope creep lesson is worth naming explicitly: rigid scoping at the start of a project is a skill, not a constraint. I treated it as optional and paid for it in time. Starting small and expanding felt natural — it nearly always does — but the cost compounds across days.

---

## What exists now that didn't last week

Notes on 3B1B video 4 and Strang lecture 2. The OOP project is structurally complete — testing and corrections remain. A standalone post for the project is coming this week once it's done and verified.

**Linear Algebra covered:**

- Matrix multiplication as composition of linear transformations. Two transformations in sequence produce a third — the matrix product captures exactly that combined motion.
- Why AB ≠ BA in general — geometrically obvious once you think of each matrix as a transformation rather than a grid of numbers.
- Reading multiplication right to left: AB means apply B first, then A. Same convention as function notation f(g(x)).
- Associativity of matrix multiplication: (AB)C = A(BC). Grouping doesn't matter when composing transformations in a fixed sequence.
- Gaussian elimination as a geometric process: reducing intersecting planes step by step to upper triangular form U.
- Pivot elements and why they can't be zero. Each elimination step as its own matrix E — so the full process is EA = U.
- Augmented matrix [A|b] for carrying the right-hand side through elimination cleanly.
- Row exchanges via permutation matrices when a zero pivot appears.
- Singular matrices — when no row exchange rescues a zero pivot and the system breaks down.
- Back substitution from U to find x.

---

## Heading into next week

The project ships this week — that's not a plan, it's a commitment. Once it's tested and posted, the backlog is cleared and the sprint gets back on track.

What I'm feeling: impatient with myself, but clear on what needs to happen. Two weeks of drag ends this week.

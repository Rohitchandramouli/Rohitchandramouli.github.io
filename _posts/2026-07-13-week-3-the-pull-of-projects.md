---
layout: post
title: "Week 3: The Pull of Projects"
date: 2026-07-13
tags: [week-3, python, data-engineering, project, github, ml-ecosystem]
excerpt: "Three weeks in and the projects are already winning against the learning track. I know it's happening and I keep going anyway — which tells me something I need to sit with."
---

## The thing that actually stuck with me this week

I'm already starting to lag on the learning track two weeks in. Not because the material is too hard — because the projects are too interesting.

That's a more honest version of the problem than "I got distracted." The IronVault finalization took most of the first half of the week. The second half went entirely into designing the next project. No 3B1B. No Strang. No new technical material at all.

I knew this was happening as it was happening. I kept going anyway. That tells me something about where my actual energy is right now — and it's something I need to manage carefully before the backlog compounds into something harder to recover from.

---

## What was actually hard

Designing a project in a field I don't fully understand yet.

The new project is a data analysis study — no models, no training, purely statistical and descriptive methods to answer a set of questions I genuinely care about. The domain is the ML ecosystem on GitHub. More on that below.

The design process surfaced a problem immediately: my original idea was too generic. The dataset that existed for it was too generic too. So the scope expanded — not from feature creep this time, but from intellectual honesty. A generic dataset wouldn't properly answer the questions I had. That meant building a proper data pipeline first: acquiring the data, cleaning it, validating it thoroughly before touching any analysis.

I locked the scope during the design stage this time and I'm holding it there. That's the Week 2 lesson applied.

The harder thing was designing something that uses statistical and probabilistic methods I haven't formally studied yet. My math track is still in linear algebra — statistics is a week or two away. So I'm designing with concepts I'll have to learn as I implement them. I made that call deliberately, but it's worth saying out loud because I'm genuinely uncertain whether it's the right one.

I also want to be transparent about the design process itself. I used Claude to work through the architecture — the same way I did with IronVault. Purely as a thinking partner: I bring the questions, the decisions, and the domain interest; it helps me reason through the design without handing me answers. There's a lot in this project's blueprint that I don't fully understand yet — statistical methods, probability concepts, things that are two weeks ahead of where my math curriculum is right now. I designed with them anyway, knowing I'll have to learn them properly before I implement. Whether that's the right call is something I'm genuinely uncertain about.

---

## What I'm proud of, honestly

The scope decision. The project grew during design — it always does — but I drew the line earlier this time and held it. The pipeline is scoped. The analysis questions are fixed. I'm not adding to them.

The other thing: recognising that data engineering is not a side quest. From everything I've seen and understood so far, the mass majority of time in real ML work goes into getting, validating, and cleaning data — not building models. Choosing to do this properly rather than grab a clean Kaggle dataset and skip straight to analysis feels like the right call for what this sprint is supposed to be building.

---

## Where I diverged from the plan

No learning this week. Zero. That's the plain version.

I can explain it — IronVault finalization, two rest days at the start of the week, project design consuming the back half — but the explanation doesn't change the ledger. Three weeks in and the learning track has been consistently losing to the project track. That has to change this week. The library learning for the new project (NumPy, Pandas, Seaborn) will count toward the learning track, but the core math curriculum cannot keep slipping.

---

## What exists now that didn't last week

IronVault is fully finalized — documented, packaged, posted. The new project has a complete design blueprint: data pipeline architecture, analysis questions, statistical methods to apply, visualization approach, and a clear scope boundary I'm committing to publicly.

---

## Heading into next week

The data pipeline gets built this week. NumPy, Pandas, Seaborn get learned as I use them — not before. Linear algebra continues in parallel. Both have to happen. Neither is optional.

What I'm feeling: pulled in two directions and aware of it. The sprint works when learning and building happen together. Right now building is winning by too much.

---

*← [IronVault — My First Software Engineering Project](/2026/07/09/ironvault-my-first-software-engineering-project/)*

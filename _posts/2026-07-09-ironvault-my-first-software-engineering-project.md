---
layout: post
title: "IronVault: My First Software Engineering Project"
date: 2026-07-09
tags: [project, python, oop, software-engineering, ironvault, rpg]
excerpt: "Not a tutorial follow-along. Not a course assignment. An honest account of how my first real software engineering project got made, what it cost, and why it mattered more than I expected."
---

## What this post is

This isn't a technical deep dive into IronVault. For that, the repo is linked at the bottom — the README documents the architecture, design decisions, and module structure in full detail. What this post is, is an honest account of how this project actually got made, what it cost, and why it mattered more than I expected.

---

## Where it started

The original scope was simple: build something clean that demonstrates the OOP concepts I'd just learned. Classes, instances, inheritance, polymorphism — show that I understood them properly, not just knew their definitions.

I've considered myself reasonably fluent in Python for a few years now. I started learning it in 11th grade, fell in love with it immediately, and had been using it confidently since. So I assumed this would be the easy part of the sprint.

Boy was I wrong.

---

## Finding the concept

I knew what I wanted to demonstrate technically but not what I actually wanted to build. The overall concept was missing. So like most people in 2026, I went to Claude, cross-referenced with ChatGPT and Gemini, and one idea stood out immediately: an RPG inventory management system.

This wasn't accidental. I'd told the AI to connect the project to my interests if possible. And the moment I saw it, I understood why it fit — every core OOP concept maps cleanly onto an RPG engine. Items, characters, inventory, combat — each one a class, each one with its own responsibilities, each one inheriting and composing naturally. I finally understood why these concepts were designed the way they were, not just what they were called.

---

## The scope problem

I couldn't stop there. That's the honest version.

I sat down with Claude and told it to act only as a thinking partner — no unnecessary information, no code, just help me think through the design. What started as a clean OOP demonstration slowly became something much larger. Four modules. A main entry point. Multiple test files. A GitHub Actions workflow for type checking and linting. A pyproject.toml for proper packaging. A loot drop generator, character classes, a combat system where inventory items actually affect gameplay.

Each addition felt justified in the moment. Each one was justified. But the scope had drifted far beyond what I originally planned, and the time cost was real — basically an entire week of the sprint.

I noted this in the Week 2 post. I'll say it again here: rigid scoping at the start is a skill. I don't fully have it yet.

---

## What IronVault actually is

IronVault is a modular, turn-based RPG engine written in modern Python. It uses an RPG inventory and combat system as a vehicle for demonstrating professional software engineering practices.

Four systems at its core:

**Items** define every object in the game world — weapons, armour, accessories, potions, repair kits.

**Inventory** manages item ownership, weight limits, equipment slots, and loot generation while protecting its internal state.

**Characters** combine base statistics, inventories, equipment, leveling, and progression into a single playable entity representing both players and enemies.

**Combat** uses interchangeable damage strategies to resolve battles while handling durability, equipment degradation, experience rewards, and victory conditions.

All four communicate through a strict one-way dependency architecture. Items never modify inventories directly. Characters own equipment slots instead of weapons owning character state. Combat knows nothing about save files. Each module has exactly one responsibility, and every feature lives where it naturally belongs.

![IronVault running — combat system and inventory in action](/assets/images/ironvault-terminal-demo.png)

---

## What it taught me

I hadn't scratched the surface of Python. That's what this project showed me.

In the span of building IronVault I learned about pytest, mypy, ruff, logging, unittest.mock, json serialization, enums, dataclasses, type hints, context managers, the Factory Pattern, the Strategy Pattern, custom exceptions, and proper Python packaging. I type-hinted every function properly for the first time. I wrote tests that use mock instances so I could verify behaviour without rebuilding the whole system from scratch every time.

Testing was a genuine revelation. The idea that I can make a change anywhere in the codebase and immediately verify nothing broke — that nothing is load-bearing in a hidden way — changed how I think about writing code.

For the first time, I felt like a software engineer rather than just a Python programmer. That transition had to happen before the ML engineering transition could mean anything.

---

## A note on using AI

I used Claude throughout this project. I want to be transparent about how.

It was used first to generate a design blueprint — a thinking partner, not a code generator. Then as I built, I used it to learn how to structure code properly, to debug errors, and to teach me about libraries and patterns I hadn't encountered before. The README was generated by Claude, but from the design I created with it and shaped through every implementation decision we worked through together.

Not a single line of code in IronVault was written by AI. Every function, every class, every module is mine. I'm noting that not as a disclaimer but because the distinction matters — using AI to think more clearly is different from using it to avoid thinking.

---

## The part that's harder to explain

I've played games my entire life. RPGs especially — from 1st grade straight through to now. When I wasn't playing them I was watching playthroughs, mostly from Jacksepticeye. My dad, during the times I'd rather be gaming than studying, would say something close to: *"Study well and you'll be making those games instead of just playing them."*

IronVault is a tiny, text-based, unfinished subsystem of a game engine. But it is something I built with my own hands. That's new. And it's closer to my dad's words than anything I've done before.

---

## One honest note before the link

This project took a lot out of me — more than I expected for something that sits outside the core ML curriculum. After finishing the implementation I took two days off before coming back to finish the documentation, final checks, and this post. That rest was necessary. I'm noting it because the sprint log should be accurate, and those two days happened.

If you're interested in the architecture, the design decisions, or just want to poke around the code, the repo is below. Star it if you think it's a reasonable first software engineering project. And if you have ideas — technically or as a game mechanic — leave them in the comments. I'll come back to IronVault in the future.

[IronVault on GitHub](https://github.com/Rohitchandramouli/ironvault)

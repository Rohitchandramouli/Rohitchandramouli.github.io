---
layout: post
title: "Week 4: Learning in Service of Something"
date: 2026-07-20
tags: [week-4, python, numpy, pandas, data-engineering, project]
excerpt: "Learning NumPy and Pandas this week felt completely different from Week 1 — knowing exactly what you're going to use something on changes how fast it sticks."
---

## The thing that actually stuck with me this week

Something shifted in how the library learning felt this week compared to how the OOP learning felt in Week 1.

In Week 1 I was learning Python concepts in the abstract — classes, inheritance, decorators — and applying them to a project I designed afterward. This week I'm learning NumPy and Pandas knowing exactly what I'm going to use them on. Every function I run in a Jupyter notebook, I'm already thinking about where it slots into the pipeline.

Learning in service of something specific feels completely different. It's faster, it sticks better, and I'm actually impatient to get to the implementation phase rather than just completing the material.

---

## What was actually hard

The data engineering pipeline is the hardest thing I've built so far — not technically, but structurally. The GitHub API has rate limits, which means I can't just hammer it with requests. The pipeline has to be designed to resolve errors gracefully, save and load its state between runs, go to sleep when it hits the rate limit, and wake back up. It's the first time I've had to think about a system that runs over hours rather than seconds.

The math track is still abandoned. I haven't caught up and I'm not pretending otherwise.

---

## What I'm proud of, honestly

The data engineering is shaping up well. The pipeline architecture is solid — I went deeper on this than I originally planned because LinkedIn kept confirming what I was already starting to believe: the work before the models matters more than the models themselves. Post after post from experienced ML engineers saying the same thing. I'd rather learn it properly now than treat it as infrastructure I rush past.

Jupyter notebooks for the first time this week too. Getting comfortable in that environment is its own small thing — it's where the actual analysis work will happen.

---

## Where I diverged from the plan

Math track: still not resumed. That's three weeks running now and I'm naming it plainly rather than finding softer language for it. It starts again next week without exception.

The project is earlier than I'd like to admit. The raw data collection pipeline is close to done — but that's roughly a quarter of the full project, not most of it. The processing pipeline, analysis, and visualisation phases are all still ahead. Matplotlib is also still pending from this week's learning plan.

---

## What exists now that didn't last week

A nearly complete raw data collection pipeline. NumPy and Pandas covered properly in Jupyter notebooks — not yet applied to real data, but solid enough to build on when the time comes.

**Libraries covered this week:**

*NumPy:*
- Arrays as fixed-type contiguous memory blocks. Creating with `np.array()`, `np.zeros()`, `np.ones()`, `np.arange()`, `np.linspace()`.
- dtypes — `int32`, `float64`, `bool`. Why dtype matters for memory and computation. Type casting with `.astype()`.
- Broadcasting — operations between different-shaped arrays without copying data. Dimensions compared trailing to leading, size-1 stretches to match.
- ufuncs — vectorised operations like `np.add`, `np.sin`, `np.exp`. Aggregations: `np.sum`, `np.mean`, `np.std` with the `axis` argument.
- Masking and boolean indexing — filtering with comparisons, combining conditions, `np.where()` for conditional selection.

*Pandas:*
- Series as a labelled 1D array. DataFrame as a collection of Series sharing an index.
- `.loc[]` for label-based indexing, `.iloc[]` for integer position-based.
- `groupby()` — split-apply-combine. Grouping by columns, applying aggregations, getting results back as a DataFrame.
- `merge()` — joining DataFrames on keys, inner/outer/left/right joins.
- Missing data — `NaN` as the sentinel. `.isna()`, `.dropna()`, `.fillna()`. Why this has to come before any analysis.

---

## Heading into next week

Matplotlib gets finished. The data collection pipeline completes and processing begins. The math track restarts — no more slipping.

What I'm actually feeling: impatient. The data collection phase has been slower than I wanted and I want to see what the data actually shows. The analysis phase is where the project stops being infrastructure and starts being interesting.

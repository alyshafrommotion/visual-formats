---
name: listicle-classification
description: How to identify whether an ad should be classified/named as the Listicle visual format. Use when naming an ad (resolving the Visual Format taxonomy token) or auditing an existing ad's format tag. Distinct from execution-sop.md, which governs how to build one.
---

# Listicle — Classification Guide

## Definition

Content structured as an **ordered/bulleted list of discrete points**, most often delivered across multiple slides (one point per slide), but sometimes stacked as a short list in a single frame. It's a **structure** ("how is the content organized"), not a device ("what does each point look like").

The device carrying each point (a Notes card, a handwritten note, plain text, an icon+label row, a photo caption) is a separate dimension. **A multi-slide Listicle usually also carries a device-format tag** (commonly `Notes App`, but also `Post-it`, `Instagram Text Overlay`, etc.), tagged as two `vf:` values.

> **Open taxonomy note (2026-08-29):** Listicle was originally defined as strictly multi-slide. We've broadened it to also cover **single-frame benefit lists** (e.g. an icon + one-line benefit stacked 3–5 times beside a product) because they're the same "list of points" structure and don't fit `feature-benefit-pointout` (which points *at* the product). If the team prefers, the single-frame version can be split into its own `benefit-list` format later.

## The thing that must be true

There is an **ordered or bulleted set of discrete points (2+)**, either:
- across **2+ sequential slides/frames**, one point per slide (the classic Listicle), or
- stacked as a short **single-frame list** of points (each a line/row), where the list itself is the structure.

## Quick test

Is the content organized as a list of separate points I read through (whether by swiping slides or scanning stacked rows)? If yes, Listicle.

## Commonly confused with

- **Feature Benefit Pointout:** also enumerates points, but they are **call-outs that point *at* specific parts of the product** (lines/arrows to features). If the list does **not** point at the product and just stacks benefits/points beside or over it, it's Listicle, not feature-benefit-pointout.
- **Us Vs Them:** a two-column comparison table, not a one-direction list of points.
- **Notes App:** the device often paired with the multi-slide structure — check `notes-app/classification.md` separately.

## What to look for as supporting signals

- Multi-slide: visual consistency across slides, a cover/title slide, numbers or ordering language ("1.", "first,")
- Single-frame: a stacked set of icon+label or bulleted benefit rows, no arrows pointing at the product

Example in this folder: Merit "SPF that doubles as a blur filter" — a single-frame list of four benefit rows (Blurs pores, Evens skin tone, Shields with mineral SPF, Feels like nothing) beside the product, none of them pointing at it.

See `execution-sop.md` in this same folder for the full build rules.

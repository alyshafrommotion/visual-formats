---
name: listicle-classification
description: How to identify whether an ad should be classified/named as the Listicle visual format. Use when naming an ad (resolving the Visual Format taxonomy token) or auditing an existing ad's format tag. Distinct from execution-sop.md, which governs how to build one.
---

# Listicle — Classification Guide

## Definition

Content structured as a **sequential, ordered list delivered across multiple slides or frames, one point per slide**, regardless of what visual device carries each point.

This is a **structure**, not a device. It answers "how is the content organized," not "what does each slide look like." The device used to present each point (a Notes card, a handwritten note, plain text, a numbered callout, a photo caption) is a separate dimension. **Most Listicle ads will also carry a device-format tag** (most commonly `Notes App`, but potentially `Post-it`, `Instagram Text Overlay`, or others), tagged as two `vf:` values.

## The one thing that must be true

There are **2+ sequential slides/frames, each delivering exactly one discrete item in an ordered list** (numbered or clearly sequential). A single-slide ad with a bulleted list crammed into one frame is not this format, it needs the swipe/sequence structure.

## Quick test

Ask: *is this a swipeable or sequential carousel where each slide gives me one point of a list, and I have to go through several slides to get the whole list?* If yes, Listicle.

## Commonly confused with

- **Feature Benefit Pointout:** also enumerates multiple points, but they're all visible at once as call-outs on a single static image, not spread across a sequence of slides.
- **Us Vs Them:** also a multi-row structure, but it's a two-column comparison table on one static, not a sequential one-point-per-slide carousel.
- **Notes App:** the device that's often paired with this structure, check `notes-app/classification.md` separately, since a Listicle can use a different device (or no distinct device format at all) to carry its points.

## What to look for as supporting signals

- Visual consistency across slides (same crop/treatment per point)
- A cover/title slide before the numbered points
- Numbers or clear ordering language ("1.", "first,", etc.)

See `execution-sop.md` in this same folder for the full build rules.

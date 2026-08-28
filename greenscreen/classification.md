---
name: greenscreen-classification
description: How to identify whether an ad should be classified/named as the Greenscreen visual format. Use when naming an ad (resolving the Visual Format taxonomy token) or auditing an existing ad's format tag. Distinct from execution-sop.md, which governs how to build one.
---

# Greenscreen — Classification Guide

Use this when you need to decide **whether a given ad is a Greenscreen** so you can assign the correct Visual Format value when naming it (or auditing/re-tagging an existing ad).

## Definition

A **Greenscreen** ad has a creator placed (usually cut-out/greenscreened) in front of a full-frame piece of external "evidence" — a screenshot, article, product page, review, chart, comment, or competitor's site — and the creator **reacts to and narrates that evidence in real time** while it stays visible on screen.

## The three things that must all be true

1. **There is real, external evidence on screen.** A screenshot, article, page, chart, review, DM, or similar — not the brand's own product shot, not a lifestyle scene, not plain text overlay with no underlying "document."
2. **The creator is composited in front of it**, not standing beside a physical object or in a normal environment. The evidence fills the frame behind them.
3. **The creator reacts to and points at the evidence** ("wait, look at this") rather than just talking to camera with the evidence as decoration. The screen is doing persuasive work, not just filling background space.

If any of these three is missing, it is probably a different format (see below).

## Quick test

Ask: *if you muted the audio and just watched, would you say "this person is showing me proof of something on their screen and reacting to it"?* If yes, it's Greenscreen. If the answer is "this person is just talking" or "this is a product demo," it's not.

## Commonly confused with

- **Comment-screenshot format:** also features a screenshot (a comment/comment thread), but the creator is not necessarily greenscreened reacting to it live, it's often the comment itself as the hero with less live reaction framing. If the comment screenshot is the entire visual and there's no reacting creator overlaid, classify as `comment-screenshot`, not Greenscreen.
- **Comment-response format:** built to look like a native story reply (a question box over a selfie/lifestyle image, answered via text overlay) — no creator reacting to *external* evidence, classify as `comment-response`.
- **Yapper:** creator talking straight down the barrel of the camera with no on-screen evidence to react to, that's `yapper`, not Greenscreen. If a yapper-style ad cuts to a screenshot occasionally but spends most of its runtime on unmediated talking-head, judge by which one carries the persuasive weight.
- **Founder:** founder-to-camera storytelling. If the founder is greenscreened reacting to real evidence (reviews, press, data), it can still be Greenscreen; if they're just telling their story to camera with no on-screen evidence, it's `founder`.

## What to look for as supporting signals (not required, but common)

- Fast cuts as the evidence changes (new claim = new screenshot)
- Highlighting, circling, or zooming on specific lines/sections of the evidence
- Casual, low-effort visual treatment (this is often intentional in the format, not a production shortcut)

See `execution-sop.md` in this same folder for the full build/scripting rules if you're producing one rather than classifying one.

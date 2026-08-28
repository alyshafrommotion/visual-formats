---
name: instagram-text-overlay-classification
description: How to identify whether an ad should be classified/named as the Instagram Text Overlay visual format. Use when naming an ad (resolving the Visual Format taxonomy token) or auditing an existing ad's format tag. Distinct from execution-sop.md, which governs how to build one.
---

# Instagram Text Overlay — Classification Guide

## Definition

An ad that wears **Instagram's own native text styling** (the story "add text" look, or the classic caption-under-post look, native fonts, optional colored highlight boxes) laid directly over a photo or clip, with no other app-UI elements (no comment chrome, no question sticker).

## The two things that must both be true

1. **The text treatment specifically mimics an Instagram-native styling convention** (story text tool, caption placement), not a generic bold text-over-image static.
2. **There's no other native-UI element carrying the message** (no username/avatar/comment thread, no question-sticker box). It's just IG-styled text over an image/clip.

## Quick test

Ask: *if you removed the branding, would this look like someone's own Instagram story or caption?* And: *is the text just IG-styled overlay, with no comment or question-sticker UI attached?* If both are yes, this format.

## Commonly confused with

- **Comment Response:** has a question-sticker UI element (black bar + question box) plus a reply. If there's a Q&A structure, it's `comment-response`, not this.
- **Comment-screenshot:** has comment-thread chrome (username, avatar, like count). If there's comment chrome, it's `comment-screenshot`, not this.
- **Post-it:** handwriting-styled note, not IG's native typed text convention.

## What to look for as supporting signals

- UGC-style, shot-on-phone base image
- Caption-voice copy (lowercase energy, contractions, line breaks pacing the read)
- Brand enters late and lightly

See `execution-sop.md` in this same folder for the full build/scripting rules.

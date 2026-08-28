---
name: comment-response-classification
description: How to identify whether an ad should be classified/named as the Comment Response visual format. Use when naming an ad (resolving the Visual Format taxonomy token) or auditing an existing ad's format tag. Distinct from execution-sop.md, which governs how to build one.
---

# Comment Response — Classification Guide

## Definition

A static built to look like an organic story reply: an Instagram-style **question sticker** (short prompt in a black bar, a user-typed question in the white section below it) sitting over a selfie/POV/lifestyle image, **answered by the account owner in free-placed native text overlay**.

## The two things that must both be true

1. **There's a question-sticker UI element** (the black-bar-plus-white-box "Ask me anything" style sticker), not just any text.
2. **There's a written reply in free-placed text blocks** answering that question, laid over the same image.

If either is missing, it's a different format.

## Quick test

Ask: *does this look like a screenshot of an Instagram Q&A sticker being answered?* If yes, Comment Response. If there's no sticker UI at all, or the "reply" is really a caption/hook rather than an answer to a posed question, it's something else.

## Commonly confused with

- **Instagram Comment:** also uses real-feeling social UI, but the hero element is a **screenshotted comment** (username, avatar, like count, timestamp), not a question-sticker-and-reply. If you see comment-thread chrome instead of a question box, classify as `instagram-comment`.
- **Instagram Text Overlay:** uses IG's native caption/story text styling, but there's no question being posed and answered, it's a single native-styled statement. If there's no Q&A structure at all, it's `instagram-text-overlay`.
- **Post-it:** also has handwritten-feeling personal text, but it's a physical sticky note/scrawl over a scene, not an app-UI question sticker.

## What to look for as supporting signals

- Casual, mid-life, non-studio image (selfie, mirror selfie, POV product-in-hand)
- Free-placed text blocks with visible gaps (not one paragraph block)
- The reply reads verdict-first, story-driven, in first person

See `execution-sop.md` in this same folder for the full build/scripting rules.

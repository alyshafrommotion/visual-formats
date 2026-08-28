---
name: instagram-comment-classification
description: How to identify whether an ad should be classified/named as the Instagram Comment visual format. Use when naming an ad (resolving the Visual Format taxonomy token) or auditing an existing ad's format tag. Distinct from execution-sop.md, which governs how to build one.
---

# Instagram Comment — Classification Guide

## Definition

A static whose hero element is a **screenshotted social comment** (Instagram, TikTok, or Facebook comment UI: username, avatar, comment text, like count, "Reply", relative timestamp), either standing alone as social proof or paired with a brand reply underneath it.

## The one thing that must be true

There is a **comment-thread UI element** as the visual hero, complete with commenter identity chrome (handle/avatar) and platform comment styling (like count, reply link, timestamp). This is not a question-and-answer sticker, and not a plain block of native-styled text, it specifically looks like a comment on a post.

## Quick test

Ask: *does this look like a screenshot of someone else's comment on a post?* If yes, Instagram Comment. If it looks like a question sticker being answered, or a caption/story text treatment with no comment-thread chrome, it's something else.

## Commonly confused with

- **Comment Response:** also features social-feeling UI and often a reply, but the hero is a **question sticker** (black bar + white question box), not a comment thread. If there's no visible question-sticker element, it's `instagram-comment`, not `comment-response`.
- **Instagram Text Overlay:** uses IG's native caption/story text styling directly over an image, no comment-thread chrome (no username/avatar/like count) at all.
- **Greenscreen:** can also feature a screenshot as evidence, but the creator is composited over it reacting live on video; Instagram Comment is a static comment screenshot, no reacting creator overlay required.

## What to look for as supporting signals

- Believable, non-brand-adjacent username/handle
- Casual typed register in the comment text (lowercase starts, contractions)
- Optional verified-brand reply indented underneath

See `execution-sop.md` in this same folder for the full build/scripting rules.

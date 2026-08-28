---
name: comment-response-classification
description: How to identify whether an ad should be classified/named as the Comment Response visual format. Covers Instagram and TikTok, static or video. Use when naming an ad (resolving the Visual Format taxonomy token) or auditing an existing ad's format tag. Distinct from execution-sop.md, which governs how to build one.
---

# Comment Response — Classification Guide

## Definition

An ad built to look like a creator **acknowledging and answering a real social comment or question** from Instagram or TikTok. The comment or question comes from native platform UI (an Instagram question sticker or comment bubble, or a TikTok comment bubble), and the whole move of the ad is "someone asked/said this, here's my reply." It can run as a **static** with a free-placed text-overlay reply, or as a **video** where the creator's on-camera response is the content.

## The two things that must both be true

1. **A real-looking comment or question from Instagram or TikTok is present as the thing being responded to** — an IG question sticker, an IG comment bubble, or a TikTok comment bubble. Not just any text: it has to read as a genuine social comment/question.
2. **The ad acknowledges and replies to it**, in one of two ways:
   - **Text overlay** that answers the comment/question, laid over the frame (static or video), OR
   - **The video itself is the acknowledgement/response** — the creator pulls up, reads, or references the comment and answers it on camera.

If there's no comment/question being answered, or the "reply" is really a generic hook/caption rather than an answer to that specific comment, it's a different format.

## Quick test

Ask: *does this look like a creator answering one specific comment or question from Instagram or TikTok?* If yes, Comment Response, whether the reply is written over the frame or spoken in the video. If nothing specific is being addressed and answered, it's something else.

## Platform + format variants (all still Comment Response)

- Instagram question sticker (AMA) answered in free-placed text overlay — the original static form.
- An Instagram or TikTok comment bubble shown, then answered — in text overlay or on camera.
- A video where the creator reads/references a comment and responds to it as the body of the ad (e.g. the Javvy example in this folder).

## Commonly confused with

- **Instagram Comment:** uses a screenshotted comment as the static hero, but is not built around acknowledging and answering it. If the comment is the visual centerpiece with no reply/answer move, classify as `instagram-comment`. The moment there's a clear "here's my answer to that," it's Comment Response.
- **Instagram Text Overlay:** native-styled text with no comment/question being posed and answered. No Q&A/reply structure means `instagram-text-overlay`.
- **Yapper:** a straight-to-camera monologue with no specific comment being answered is `yapper`. A Comment Response video must be anchored to a specific comment/question it is replying to.
- **Post-it:** handwritten-feeling personal text over a scene, not a platform comment/question UI.

## What to look for as supporting signals

- Native Instagram/TikTok comment or question UI (bubble, avatar/username, like/timestamp chrome, or question-sticker styling)
- Casual, non-studio setting (selfie, mirror selfie, POV product-in-hand, or talking head)
- The reply reads verdict-first, first person, answering the specific comment
- For video: the creator explicitly references the comment ("someone asked…", "you said…", "replying to @…") before answering

See `execution-sop.md` in this same folder for the full build/scripting rules.

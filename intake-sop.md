# Visual Format Inspo Intake SOP

How to handle it when a team member shares an inspiration example (a Motion inspo link, a link to social content, or a screenshot) that should go into the Visual Formats library at `/agent/brain/2. ideation/visual-formats/`.

This process doc lives at the root of the `visual-formats` library, next to `index.md`, and ships in the public mirror so contributors can follow the same intake steps.

## Trigger

Any time someone shares an inspo/ad link, a link to a piece of social content, or a screenshot and wants it kept as a reference example (or it is clearly meant for the library). If they did not say which format it is, classify it yourself and propose it.

## Steps

1. **Get the actual creative.**
   - Motion inspo/ad link (`projects.motionapp.com/.../inspo/ad/<id>`) or an ad-library creative id: run `motion meta competitor-ad-insights --ad-library-creative-id <id>`. Media is at `.creative.fileUrl`, brand at `.creative.brand.name`, media type at `.creative.format`.
   - Other social link (TikTok, Instagram, etc.): download the actual creative media from the link.
   - Screenshot (an uploaded image): the upload itself is the asset.

2. **Suggest the visual format (if not told).** Compare against the `classification.md` files in the library and propose the best-fit format, with one short line on why. A creative can carry up to two format tags per the dual-format tagging rule in `/agent/brain/6. launch/naming-convention.md`. If the person already named the format, use that.

3. **Get approval before saving.** State the proposed format, destination folder, and filename, then wait for a yes or a correction. Do not save anything until it is approved.

4. **Prepare the media.**
   - If it is a **screenshot**, crop out all platform UI so only the creative remains (status bar, like/comment/share bars, profile header, caption, link/CTA card, next post, scrollbars). Verify the crop before saving.
   - Otherwise, **download** the creative and save it as-is.

5. **Name it by the brand.** Brand name, lowercase, words separated by single dashes. Strip punctuation (apostrophes, periods, commas): `the farmer's dog` becomes `the-farmers-dog`. Transliterate accented or non-ascii characters to plain ascii: `grüns` becomes `gruns`. Spell `&` as `and` (`Mott & Bow` becomes `mott-and-bow`). Keep the brand's true spelling otherwise (`comfrt`, not `cmfrt`). Use the extension that matches the media (`.jpg`, `.jpeg`, `.png`, `.mp4`).

6. **Save + sync.** Put the file in the matching format folder, update the format's count in `index.md`, and push the library to the public GitHub mirror so brain and repo stay in sync.

7. **Multiple examples from one brand / duplicates.** If you're *replacing* an existing example, do not overwrite or delete anything — ask which one to keep. If you're intentionally keeping more than one example from the same brand in the same format (to show different variations), number them in the order they were shared: `brand-1`, `brand-2`, and so on (e.g. `spacegoods-1`, `spacegoods-2`). Never overwrite or delete an existing example to resolve a collision without an explicit instruction on which to keep.

## Notes

- Never save without step 3 approval.
- Never delete an existing example to resolve a duplicate without an explicit instruction on which to keep.

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

5. **Name it `brand_format`.** Combine the brand and the format folder name, separated by an underscore. Use dashes for spaces *within* a term, and underscores only to separate the brand from the format (and from a trailing number). Example: a Honeylove ad in the `matching-chart` folder becomes `honeylove_matching-chart.jpg`.
   - **Brand:** lowercase, dashes for spaces. Strip punctuation (`the farmer's dog` → `the-farmers-dog`). Transliterate accents to plain ascii (`grüns` → `gruns`). Spell `&` as `and` (`Mott & Bow` → `mott-and-bow`). Keep the brand's true spelling otherwise (`comfrt`, not `cmfrt`).
   - **Format:** the folder name exactly as it appears (already dash-formatted), e.g. `instagram-text-overlay`, `comment-response`, `us-vs-them`.
   - **Extension:** match the media (`.jpg`, `.jpeg`, `.png`, `.mp4`).

6. **Save + sync.** Put the file in the matching format folder, then keep the counts aligned: update the format's example count in `index.md` **and** its `Examples` number in the Notion Visual Format database, and push the library to the public GitHub mirror so brain and repo stay in sync.

7. **Multiple examples from one brand in the same format / duplicates.** If you're *replacing* an existing example, do not overwrite or delete anything — ask which one to keep. If you're intentionally keeping more than one example from the same brand in the same format folder, append a number with an underscore, in the order they were added: `honeylove_matching-chart_1`, `honeylove_matching-chart_2`, and so on. A single example needs no number. Never overwrite or delete an existing example to resolve a collision without an explicit instruction on which to keep.

## Notes

- Never save without step 3 approval.
- Never delete an existing example to resolve a duplicate without an explicit instruction on which to keep.
- Naming shorthand: **dashes = spaces within a term, underscores = separators.** So `brand_format`, or `brand_format_N` when a brand has more than one example in the same format.

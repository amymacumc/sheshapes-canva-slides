# Workflow and QA

## Intake and executable brief

1. Prefer a Markdown brief that Codex can execute directly.
2. When the source is a loose idea, ask ChatGPT to create the `.md` brief first.
3. Include the goal, audience, slide count, page plan, source facts, intentional
   placeholders, brand requirements, desired output, and delivery destination.
4. Keep the Markdown brief as a reusable input artifact so the same content can
   be regenerated with a new version or another approved brand system.

## Output routing

- Choose `pptx-only` when the user needs a downloadable, editable source or the
  Canva Plugin is unavailable.
- Choose `pptx-and-canva` when the user explicitly requests Canva and the Canva
  Plugin is installed and authorized.
- Choose `asset-pack` when the request is for reusable backgrounds, logos,
  illustrations, or components rather than a complete deck.
- Always keep the validated PPTX when delivering to Canva; it is the source and
  fallback artifact.

## Content transformation

1. Extract source content without changing facts.
2. Identify the audience, decision, and desired action.
3. Group the material into a narrative with one message per page.
4. Write concise slide copy before laying out elements.
5. Preserve citations, units, dates, names, and direct quotes.
6. Mark missing or unverified facts instead of inventing them.

## Production

1. Create a versioned 16:9 PPTX as the primary editable source.
2. Use the bundled gradients and SVG elements.
3. Place the correct logo variant on every page.
4. Keep user-supplied media replaceable.
5. Add speaker notes when detail does not fit the page.
6. Keep raw SVG and logo assets separate from the deck so they can be reused in
   other Canva projects.

## Visual QA

Render every page and check:

- title and body overflow;
- clipped or stretched imagery;
- safe margins;
- consistent logo size and variant;
- contrast on dark and light gradients;
- card alignment and equal spacing;
- duplicated or missing pages;
- placeholders that should have been replaced;
- accidental black, neon, robot, or cyberpunk imagery;
- content density and narrative continuity.

Inspect both:

- a contact sheet for rhythm and consistency;
- full-size renders for text and edge defects.

## Canva delivery

### Prerequisites

1. Confirm that the Canva Plugin is installed in Codex.
2. Confirm that the intended Canva account is connected and authorized.
3. Resolve the target design or folder from the user-provided link or ID.
4. If the Plugin is unavailable, return the PPTX and manual import guidance.

### Delivery steps

1. Import the validated PPTX as a Canva Presentation.
2. Upload only new reusable assets separately.
3. Move all requested items into the target folder.
4. List the target folder and verify exact names and counts.
5. Confirm the imported page count and design title.
6. Return both the Canva link and local PPTX source.

If an upload partially fails, list the folder before retrying. Retry only
missing items to avoid duplicates.

Do not claim that SVG gradients or grouped illustrations can always be
ungrouped in Canva.

## Versioning and stewardship

- Use versioned filenames such as `v0.1`, `v0.2`, and `v1.0`.
- Do not overwrite an approved source or Canva design without explicit consent.
- Recommend `Built with the SheShapes AI Slide System` for public adaptations.
- Welcome reuse by the SheShapes AI 2026 committee and fellows, and by future
  SheShapes AI continuation projects.
- Do not imply that the community reuse statement authorizes resale of the
  bundled brand assets.

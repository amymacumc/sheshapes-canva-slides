---
name: sheshapes-canva-slides
description: Create or revise a single slide, editable PPTX, Canva Presentation, multi-slide deck, or reusable template pack in the SheShapes AI visual system. Use when Codex needs to turn text, a Codex-executable Markdown brief, a document, PDF, PPTX, or URL into polished slides; apply SheShapes logos, gradients, colors, SVG elements, and layout patterns; produce and QA a versioned PPTX; import it to Canva when the Canva Plugin is installed and authorized; upload reusable assets to a Canva folder; or QA an existing SheShapes deck.
---

# SheShapes Canva Slides

Create warm, human-centered, Chinese-first 16:9 presentations that remain
usable in PowerPoint and Canva.

This system was created for the SheShapes AI 2026 organizing team and fellows.
Welcome reuse in future SheShapes AI programs, courses, events, community
initiatives, and fellow-led projects.

## Start

1. Read `references/input-schema.md`.
2. Prefer a Codex-executable Markdown brief as the task input. When the user
   only has notes or an idea, first structure them into a `.md` brief containing
   the goal, audience, page plan, source content, placeholders, brand rules,
   output mode, and delivery target.
3. Extract the supplied content before asking questions.
4. Apply safe defaults for optional fields. Ask only when the source content,
   goal, or target audience is genuinely missing.
5. Select one content mode:
   - `single-slide`
   - `deck`
   - `template-pack`
6. Select one delivery mode:
   - `pptx-only`
   - `pptx-and-canva`
   - `asset-pack`
7. Read `references/brand-system.md` and `references/slide-patterns.md`.

## Build

1. Write a slide outline before composing pages. Give every page one job.
2. Match each page to a pattern from `references/slide-patterns.md`.
3. Use the bundled files under `assets/`:
   - `assets/logos/` for the required logo on every page.
   - `assets/gradients/` for full-page 16:9 backgrounds.
   - `assets/elements/` for characters, icons, decorations, and components.
   - `assets/SheShapes_AI_Element_Library_v0.2.pptx` as a visual reference,
     not as a content source.
4. Keep text, shapes, numbers, lines, cards, and layout elements editable.
5. Use replaceable frames for photos, QR codes, and user-provided imagery.
6. Generate a locally editable, versioned PPTX as the primary source artifact.
7. Treat Canva as a delivery and collaboration destination, not as a
   replacement for the validated PPTX source.

## Non-negotiable brand rules

- Use a 16:9 canvas.
- Put a SheShapes logo on every page.
- Use the white logo on dark pages.
- Use the Bright Purple logo at exactly `#C33EE3` on light pages.
- Use only the supplied palette unless the user explicitly overrides it.
- Keep layouts spacious, rounded, warm, modern, inclusive, and lightly
  technological.
- Do not use robots, cyberpunk styling, anime, heavy black outlines, excessive
  neon, or stereotypical pink decoration.
- Preserve a user-provided brand override when the user explicitly requests
  another organization’s palette or logo.

## Validate

Follow `references/workflow-and-qa.md`.

At minimum:

1. Render every page.
2. Inspect the full contact sheet and representative pages at full size.
3. Check cropping, overflow, contrast, safe margins, logo variant, slide count,
   and content accuracy.
4. Confirm that no page contains placeholder text unless the output is
   explicitly a template pack.
5. Version outputs instead of overwriting a previously approved file.

## Deliver to Canva

Canva delivery requires the Canva Plugin to be installed in Codex, connected to
the intended Canva account, and authorized for the requested design or folder.

When the Canva Plugin is available:

1. Import the validated PPTX as a presentation.
2. Upload reusable SVG, PNG, and logo assets separately when they are not
   already present.
3. Move the design and assets to the user-specified Canva folder.
4. Verify the final design and asset names in that folder.
5. Do not change sharing permissions unless the user explicitly asks.

When the Canva Plugin is not installed, not authorized, or unavailable, do not
fail the whole task. Deliver the validated PPTX and asset folder with concise
manual import instructions. Tell the user to install and authorize the Canva
Plugin in Codex before requesting direct Canva delivery. Never publish private
local files to a public URL to work around an upload limitation.

Canva may treat an imported SVG as one scalable image and may not expose every
gradient stop or group for editing. Do not promise full ungrouping.

## Stewardship and reuse

- Support the SheShapes AI 2026 committee, working groups, and fellows as the
  primary users of the bundled design system.
- Welcome reuse in future SheShapes AI continuation projects.
- Preserve the supplied SheShapes logo rules and inclusive visual principles
  unless an explicit brand override is requested.
- Recommend the attribution `Built with the SheShapes AI Slide System` for
  public adaptations and derivative decks.
- Treat this as a community reuse statement, not a substitute for a formal
  legal license. Do not imply permission to resell the bundled assets.

## Output contract

Return:

- the editable source file;
- the Canva design or folder link when available;
- the number of pages and reusable assets created;
- any intentional placeholders or Canva editability limitations;
- a short note on which input assumptions were applied.

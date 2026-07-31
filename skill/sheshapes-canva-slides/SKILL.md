---
name: sheshapes-canva-slides
description: Create or revise a single Canva slide, a multi-slide presentation, or a reusable template pack in the SheShapes AI visual system. Use when Codex needs to turn text, a brief, Markdown, a document, PDF, PPTX, or URL into polished Canva-ready slides; apply SheShapes logos, gradients, colors, SVG elements, and layout patterns; build an editable PPTX before Canva import; upload reusable assets to a Canva folder; or QA an existing SheShapes deck.
---

# SheShapes Canva Slides

Create warm, human-centered, Chinese-first 16:9 presentations that remain
usable in PowerPoint and Canva.

## Start

1. Read `references/input-schema.md`.
2. Extract the supplied content before asking questions.
3. Apply safe defaults for optional fields. Ask only when the source content,
   goal, or target audience is genuinely missing.
4. Select one mode:
   - `single-slide`
   - `deck`
   - `template-pack`
5. Read `references/brand-system.md` and `references/slide-patterns.md`.

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
6. Prefer a locally generated editable PPTX as the Canva import artifact.

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

When a Canva connector is available:

1. Import the validated PPTX as a presentation.
2. Upload reusable SVG, PNG, and logo assets separately when they are not
   already present.
3. Move the design and assets to the user-specified Canva folder.
4. Verify the final design and asset names in that folder.
5. Do not change sharing permissions unless the user explicitly asks.

When no Canva connector is available, deliver the PPTX and asset folder with
concise manual import instructions. Never publish private local files to a
public URL to work around an upload limitation.

Canva may treat an imported SVG as one scalable image and may not expose every
gradient stop or group for editing. Do not promise full ungrouping.

## Output contract

Return:

- the editable source file;
- the Canva design or folder link when available;
- the number of pages and reusable assets created;
- any intentional placeholders or Canva editability limitations;
- a short note on which input assumptions were applied.


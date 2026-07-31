# Input schema

Accept natural-language instructions or the structured fields below.

## Required information

- `source`: content, notes, attachment, document, or URL to transform.
- `goal`: what the audience should understand, feel, or do.
- `audience`: who will see the slides.

If one of these cannot be inferred, ask one concise question.

## Optional fields and defaults

| Field | Accepted values | Default |
| --- | --- | --- |
| `mode` | `single-slide`, `deck`, `template-pack` | `deck` |
| `language` | Chinese, English, bilingual | Match the source; Chinese first when mixed |
| `slide_count` | Number or range | 8–12 for a deck |
| `tone` | Warm, technical, editorial, energetic, formal | Warm editorial |
| `presentation_context` | Workshop, keynote, pitch, report, training, social | Infer from source |
| `must_include` | Quotes, data, CTA, names, links, sections | Preserve all explicit requirements |
| `imagery` | User images, documentary photos, SVG-only, no photos | SVG-first; use photos only when they add meaning |
| `brand_mode` | SheShapes, custom override | SheShapes |
| `canva_target` | Folder or design URL/ID | Ask only before final Canva delivery |
| `output` | PPTX, Canva, SVG assets, PDF preview | PPTX + Canva when connected |

## Content-density defaults

- Use one key message per page.
- Limit titles to two lines.
- Limit standard pages to three content groups.
- Keep Chinese body copy near 70 characters or fewer per page.
- Keep English body copy near 45 words or fewer per page.
- Move detail to speaker notes or an appendix when needed.

## Structured brief

```yaml
mode: deck
topic:
goal:
audience:
language:
slide_count:
presentation_context:
source:
must_include:
call_to_action:
imagery:
brand_mode: SheShapes
brand_overrides:
canva_target:
output:
```


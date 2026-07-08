---
name: ppt-editable
description: Create editable PowerPoint decks from outline documents, pasted text, markdown, notes, PPT screenshots/images, or mixed copy-and-image materials. Use when the user asks to upload an outline document and automatically detect outline copy plus image arrangement, arrange a PPT according to a document outline, convert PPT images/screenshots into editable PowerPoint, or directly generate an editable .pptx from text.
---

# Editable PPT

## Overview

Build real editable `.pptx` files, not flattened image decks. The final deck should use native PowerPoint text boxes, shapes, tables, charts, and editable layout objects wherever practical, while using photos/illustrations as image assets when they are content rather than slide structure.

## Route The Request

Choose the workflow before authoring:

- **Outline document to PPT**: user uploads or points to a Word/PDF/Markdown/TXT outline document and wants the deck arranged by that outline. Read `references/outline-document-to-ppt.md`.
- **Copy and image auto arrangement**: user supplies outline copy plus image assets, or asks to automatically detect which text belongs with which images. Read `references/copy-image-arrangement.md`.
- **PPT image to editable deck**: user supplies screenshots, slide images, PDF renders, or exported slide PNG/JPG files and wants an editable PowerPoint. Read `references/image-to-editable-ppt.md`.
- **Text to editable deck**: user supplies text, outline, markdown, notes, topic, or raw content and wants a new editable PPT. Read `references/text-to-editable-ppt.md`.
- **Existing PPTX edit or template following**: use the Presentations skill's template-following workflow, then apply this skill's editability requirement.

## Non-Negotiables

- Use the Presentations skill to create, edit, render, inspect, and validate `.pptx` files.
- Do not deliver a deck made of full-slide screenshots unless the user explicitly asks for a visual-only facsimile. Full-slide images may be used temporarily as tracing/reference backgrounds, but remove or hide them before final delivery unless needed as non-editable source evidence.
- Keep visible slide text audience-facing. Do not expose reconstruction notes, prompt scaffolding, or internal planning text in the final slides.
- Validate visually before delivery: render all slides, inspect for overlap, clipping, unreadable text, missing objects, and accidental rasterized slide backgrounds.
- Save the final `.pptx` under the requested path, otherwise under the workspace `outputs/` directory.
- If the source has both an outline and image assets, preserve the outline's section order first, then place images by semantic match, filename/order hints, captions, EXIF/order proximity, and visual relevance.

## Editability Standard

Treat these as editable:

- Text as PowerPoint text boxes with real fonts and editable content.
- Rectangles, lines, arrows, icons, labels, callouts, and simple diagrams as native shapes.
- Tables as PowerPoint tables when the grid and text are legible.
- Charts as editable charts when data can be inferred or provided; otherwise recreate with native shapes and clearly note uncertainty to the user.
- Photos, logos, screenshots inside a slide, and complex illustrations can remain images if they are semantically image assets rather than slide structure.

## Delivery Checklist

- Final artifact is `.pptx`, not PDF or images only.
- Rendered slide previews have been inspected.
- All slide-level text that should be editable is editable.
- The deck follows the document outline unless the user explicitly asked for a different narrative order.
- Image placement choices are consistent with the outline and do not bury important text.
- Final response links only the delivered `.pptx`, plus a brief note about any source image/text limitations.

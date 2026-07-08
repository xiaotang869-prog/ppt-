# PPT Image To Editable Deck

Use this workflow when the user supplies slide screenshots, slide images, exported PDF pages, or other flattened PPT visuals and asks for an editable PowerPoint.

## Workflow

1. Inventory inputs: count images/pages, identify intended slide size, order, language, and any repeated master elements.
2. Inspect each source image visually. If text is blurry or too small, ask for a higher-resolution source or state the uncertainty before final delivery.
3. Create a reconstruction plan per slide:
   - canvas size and background color or image region
   - text blocks, hierarchy, font approximation, and alignment
   - native shapes, lines, arrows, charts, tables, icons, and image assets
   - elements that will remain raster assets because they are photos/logos/complex illustrations
4. Rebuild each slide as native editable objects using the Presentations skill. Use the source image only as a temporary tracing reference; remove it before final export unless explicitly kept.
5. Preserve visual fidelity enough to match layout, hierarchy, and meaning. Prefer editability over pixel-perfect recreation when the two conflict.
6. Render the rebuilt deck and compare against the source images. Fix obvious spacing, text wrapping, color, and object placement differences.

## OCR And Text

- Prefer real text boxes. Do not leave source text baked into a screenshot.
- If OCR is available, use it as a first pass but manually verify against the image.
- Preserve the user's language, punctuation, numbers, units, and line breaks when legible.
- If a word or number is uncertain, mark it in a temporary notes file and ask or disclose; do not silently invent.

## Shape Reconstruction

- Use native rectangles, rounded rectangles, lines, arrows, connectors, and simple icons for slide structure.
- Use PowerPoint tables for clear grid/table content.
- Use editable charts only when the source data is legible or supplied. If the chart is only visually inferable, recreate the appearance with shapes and tell the user it is not data-backed.
- Keep logos/photos/screenshots as cropped image objects.

## QA

Before delivery:

- Render every slide and inspect full-size previews or a contact sheet.
- Confirm no full-slide source screenshot remains as the only content layer.
- Check that editable text can be selected in the generated PPTX.
- Check for overlap, clipping, accidental two-line title wraps, missing icons, and unreadable small text.

# Copy And Image Auto Arrangement

Use this workflow when the user provides copy plus image assets and asks Codex to automatically detect the outline, match text to images, and arrange a polished editable PPT.

## Asset Inventory

1. List every text source and image source.
2. For each image, inspect the visible subject, orientation, aspect ratio, dominant colors, embedded text, and likely use:
   - hero/background
   - supporting visual
   - product screenshot
   - icon/logo
   - evidence/photo
   - chart/diagram source
3. Use filenames, folder order, timestamps, captions, nearby text, and user-provided numbering as hints, not absolute truth.

## Matching Copy To Images

Match images to outline sections by:

- semantic relevance between image content and section topic
- caption or filename keywords
- document order proximity
- repeated visual motifs across a section
- aspect ratio fit for the intended slide layout
- whether the image contains essential readable detail

If a match is uncertain, choose the least risky placement and note the uncertainty only in the final response if it affects correctness.

## Layout Decisions

- Use one clear visual role per slide: hero image, supporting side image, full-bleed background, comparison image pair, process screenshot, or small evidence thumbnail.
- Do not crowd multiple unrelated images onto one slide.
- Crop intentionally: preserve faces, product details, important labels, and chart axes.
- Keep essential text editable. Do not bake headings or bullet text into images.
- Use consistent image treatment across the deck: radius, border, shadow, caption style, and placement rhythm.

## When Images Are Insufficient

- If no suitable image exists for a section, use native shapes, tables, or a simple diagram.
- If an image is too low-resolution for full-slide use, place it smaller or ask for a higher-resolution source.
- If a screenshot includes important UI text, keep it as an image but add editable annotations/callouts where useful.

## QA

Before delivery:

- Render every slide and inspect image crops.
- Confirm images support the slide's point rather than decorating randomly.
- Check that text remains readable and editable.
- Check that repeated sections have a consistent visual rhythm without becoming monotonous.

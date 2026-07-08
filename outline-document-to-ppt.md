# Outline Document To PPT

Use this workflow when the user uploads or references a document and asks to generate a PPT according to the document outline, chapter structure, headings, or proposal/report framework.

## Input Handling

1. Identify the source type: `.docx`, `.pdf`, `.md`, `.txt`, `.xlsx`, images with text, or pasted content.
2. Extract the document hierarchy:
   - title, subtitle, author/date if present
   - heading levels or numbered outline levels
   - section summaries, bullets, tables, figures, and captions
   - mandatory items such as conclusions, requirements, deliverables, or timeline
3. If the file has no explicit heading structure, infer one from numbering, typography, paragraph breaks, table of contents, or repeated section labels.
4. Keep a temporary outline map with source section names and planned slide numbers. Do not put this map into the final deck.

## Deck Planning

- Preserve the source outline order unless it produces a weak story. If reordering materially improves the deck, state the assumption in the final response.
- Convert each major section into one or more slides based on density.
- Use section divider slides only when the deck is long enough to benefit from them.
- Keep visible slide copy short and audience-facing. Move detail into speaker notes only if requested.
- Turn lists into comparison tables, timelines, process diagrams, or grouped callouts when that improves readability.

## Slide Allocation

Use this default mapping, then adapt:

- Document title and purpose -> title slide
- Executive summary or abstract -> overview slide
- Level-1 headings -> sections or slide groups
- Level-2 headings -> slide titles
- Level-3 headings and paragraphs -> bullets, callouts, tables, or notes
- Tables -> editable PowerPoint tables where practical
- Figures/images -> placed near the related section
- Conclusions/recommendations -> final summary or next steps

## QA

Before delivery:

- Check that every important source section is represented or intentionally omitted.
- Check slide order against the outline map.
- Render the deck and inspect for overlap, clipping, small text, and weak hierarchy.
- Mention any source sections that were condensed or omitted due to density.

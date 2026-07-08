# Text To Editable PPT

Use this workflow when the user supplies text, markdown, notes, an outline, a topic, or pasted material and asks for an editable PowerPoint without a separate source document file.

## Workflow

1. Clarify only essential missing constraints: audience, purpose, language, approximate slide count, and visual style. If the user gave enough context, proceed with reasonable assumptions.
2. Convert the source text into a narrative deck plan:
   - title slide
   - context or problem
   - key points or sections
   - evidence/examples
   - conclusion, recommendation, or next steps
3. Write audience-facing slide copy. Shorten dense source text instead of shrinking fonts.
4. Create the deck using the Presentations skill. The output must be editable native PowerPoint: real text boxes, shapes, tables, charts, and image placeholders/assets.
5. Use a coherent theme. If no brand/style is provided, choose a restrained professional visual direction that fits the content.
6. Render and inspect every slide. Fix overlap, clipping, weak hierarchy, inconsistent spacing, and title wrapping.

## Content Rules

- Do not dump paragraphs onto slides. Turn text into concise headings, bullets, diagrams, tables, or section layouts.
- Keep each slide focused on one idea.
- Use speaker notes only if the user asks.
- Do not expose planning labels such as "HOOK", "BODY", or "CTA" as visible slide content unless they are part of the requested deck.
- Preserve important terminology, names, dates, numbers, and claims from the source text.
- If the text is already an outline, preserve its section order unless the user asks for a more persuasive narrative rewrite.

## Editability Requirements

- All generated copy must be editable text.
- Process diagrams and callouts should use native PowerPoint shapes.
- Tables should be editable PowerPoint tables where practical.
- Charts should be editable when source data is provided; otherwise use clearly labeled visual summaries and note the limitation.
- Decorative images may be raster assets, but they should not contain essential editable text.

## QA

Before delivery:

- Render the final `.pptx`.
- Inspect all slides for overlap and text wrapping.
- Confirm the deck tells a coherent story from the user's source text.
- Return the final `.pptx` path and mention any assumptions.

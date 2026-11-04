---
name: pdf-consistency-review
description: Review a user-provided PDF for inconsistencies between paragraphs and between paragraph text and text embedded in images. Use when asked to check a PDF for consistency.
---

# PDF consistency review

Review the PDF supplied by the user. Apply any additional review skills or
explicit rules the user provides. Those rules define specialized checks; do not
invent domain-specific requirements or treat every variation in wording as an
inconsistency.

## Review procedure

1. Confirm which PDF is being reviewed. If no PDF is available, ask the user to
   provide it.
2. Read the document in page order. Extract its text and inspect page images,
   figures, charts, tables, screenshots, and scanned content for text that can
   be compared with the prose. Use available OCR or visual inspection when
   needed.
3. Compare claims across paragraphs and sections. Check relevant details such
   as names, dates, quantities, units, definitions, and relationships. Also
   compare claims in paragraphs with text found in images, including labels,
   captions, legends, and values.
4. Apply each supplied rule skill to the same document. If rules disagree,
   identify the conflict and ask the user how to proceed rather than silently
   choosing one.
5. Verify each candidate finding against its source locations and surrounding
   context. Distinguish a direct contradiction from an ambiguity, omission, or
   possible inconsistency. Do not infer facts that the document does not state.

## Report

Return a concise report containing:

- **Finding:** what appears inconsistent and whether it is a contradiction,
  ambiguity, or possible inconsistency.
- **Evidence:** short exact quotations from both statements, with page numbers
  and section, paragraph, or image labels when available.
- **Why it matters:** the specific difference, without guessing which statement
  is correct.

If no issues are found, say so and summarize what was reviewed. State any
limitations, such as pages that could not be read, text in images that could
not be extracted, or review rules that could not be applied. Never claim to
have reviewed unreadable content, and do not modify the source PDF.

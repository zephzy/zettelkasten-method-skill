---
name: zettelkasten-method
description: Turn source material into Zettelkasten-style knowledge assets. Use when the user wants to process articles, papers, transcripts, lecture notes, book excerpts, or rough notes into fleeting notes, literature notes, permanent notes, meaningful note links, bottom-up outlines, drafts, and quality reports with source traceability.
---

# Zettelkasten Method

## Overview

Transform raw material into reusable, traceable, atomic, and linkable knowledge notes. Do not produce a one-off summary. Build a small knowledge system that can support future thinking and writing.

把素材处理成可以继续积累、链接和写作的知识卡片，而不是只给一次性总结。

## Inputs

Accept any of the following:

- source material: article, paper excerpt, transcript, lecture note, book passage, web page excerpt, or rough note
- optional metadata: title, author, URL, publication date, page, timestamp, repository, or file path
- optional goal: learning, research review, exam prep, article writing, project documentation, or knowledge-base building
- optional language preference: English, Chinese, or bilingual

If source metadata is missing, mark it as `unknown`. Do not invent metadata. If the user gives only a URL and the environment cannot fetch it, ask for the relevant excerpt.

## Workflow

Run the workflow in this order:

1. Create a source snapshot with only enough context for traceability.
2. Capture fleeting notes for observations, questions, and possible directions.
3. Create literature notes that explain what the source says and preserve source fields.
4. Convert the strongest source-grounded ideas into permanent notes.
5. Propose meaningful links between permanent notes.
6. Build a topic outline from the linked notes.
7. Draft from the note network.
8. Run a quality report against Zettelkasten principles.
9. Suggest next actions.

## Output Contract

Produce Markdown with these sections in order:

1. `Source Snapshot`
2. `Fleeting Notes`
3. `Literature Notes`
4. `Permanent Notes`
5. `Proposed Links`
6. `Topic Outline`
7. `Short Draft`
8. `Quality Report`
9. `Next Actions`

Use stable note IDs:

- fleeting notes: `F-001`, `F-002`
- literature notes: `L-001`, `L-002`
- permanent notes: `P-001`, `P-002`

When drafting, cite supporting note IDs in parentheses, such as `(P-001, L-002)`.

## Note Rules

### Fleeting Notes

- Keep them short and rough.
- Capture why the idea caught attention.
- Do not turn them into final claims.

Use this shape:

```markdown
### F-001
- Capture:
- Why it caught attention:
- Possible direction:
```

### Literature Notes

- Preserve source information.
- Rewrite source claims in clear language.
- Separate source claims from interpretation.
- Avoid long direct quotes.

Use this shape:

```markdown
### L-001
- Source:
- Location:
- Source claim:
- Rewritten explanation:
- Useful for:
```

### Permanent Notes

- One note, one idea.
- Write in the user's own words.
- Make the note understandable without rereading the source.
- Use descriptive titles, not vague labels like "important idea".

Use this shape:

```markdown
### P-001 - Descriptive note title
- Claim:
- Explanation:
- Example:
- Source basis:
- Possible links:
```

## Link Rules

Each proposed link must explain the relationship between ideas. Prefer these relationship types:

- cause and effect
- tension or contradiction
- application
- analogy
- general principle to concrete example
- method to quality check

Do not output tag-only links.

Use this shape:

```markdown
- `P-001` -> `P-002`
  - Relationship:
  - Why this link matters:
```

## Quality Rules

In the quality report, check:

- Atomicity: each permanent note has one main idea.
- Own-words rewriting: source ideas are rewritten, not copied.
- Source traceability: literature notes preserve source fields.
- Link quality: links explain relationships.
- Bottom-up synthesis: outline and draft grow from notes.
- Unsupported claims: draft claims can be traced back to note IDs.
- Revision targets: notes to split, merge, rename, or support better.

## Failure Modes

Avoid these failures:

- producing only a fluent summary
- creating permanent notes that contain multiple ideas
- inventing source metadata
- copying long source passages
- treating tags as links
- drafting claims that cannot be traced back to notes
- making an outline first and forcing notes into it afterward

## Optional References

Use the repository templates only when the user wants reusable files or stricter formatting:

- `../../templates-and-examples/templates/`
- `../../templates-and-examples/examples/`


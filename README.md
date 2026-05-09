# LLM Wiki

A personal knowledge base maintained by Kimi Code.
Based on Andrej Karpathy's LLM Wiki pattern.

## Purpose

This wiki is a structured, interlinked knowledge base for electricity bill analysis.
Kimi maintains the wiki. The human curates sources, asks questions, and guides the analysis.

## Folder structure

```
raw/          -- source documents (immutable -- never modify these)
wiki/         -- markdown pages maintained by Kimi
wiki/index.md -- table of contents for the entire wiki
wiki/log.md   -- append-only record of all operations
```

## Ingest workflow

When the user adds a new source to `raw/` and asks you to ingest it:

1. Read the full source document
2. Discuss key takeaways with the user before writing anything
3. Create a summary page in `wiki/` named after the source
4. Create or update concept pages for each major idea or entity
5. Add wiki-links ([[page-name]]) to connect related pages
6. Update `wiki/index.md` with new pages and one-line descriptions
7. Append an entry to `wiki/log.md` with the date, source name, and what changed

## Page format

Every wiki page should follow the structure shown in `wiki/index.md`.

## Rules

- Never modify anything in the `raw/` folder
- Always update `wiki/index.md` and `wiki/log.md` after changes
- Keep page names lowercase with hyphens (e.g., `machine-learning.md`)
- Write in clear, plain language

# Instructions for AI Agents

## Repository Purpose

This repository contains the LaTeX source code and bibliography for:

**Self-Improvements in Modern Agentic Systems: A Survey**

The primary goal is to maintain the paper, bibliography, figures, and
associated resources in a consistent and reproducible form.

## Canonical Files

- Main LaTeX entry point: `main.tex`
- Bibliography database: `references.bib`
- Figures: `figures/`
- Section source files: `sections/`
- Compiled manuscript: `paper.pdf`

Treat `main.tex` and `references.bib` as canonical source files.

## Compilation

Compile the manuscript using:

```bash
latexmk -pdf main.tex
````

Alternatively:

```bash
pdflatex main.tex
bibtex main
pdflatex main.tex
pdflatex main.tex
```

The final PDF must compile without undefined citations or references.

## Bibliography Rules

1. Add all new references to `references.bib`.
2. Do not manually type bibliographic information into the LaTeX text.
3. Preserve existing BibTeX citation keys unless correcting an error.
4. Before adding a new entry, check whether the work already exists in
   `references.bib`.
5. Prefer authoritative metadata from the publisher, conference, journal,
   DBLP, Crossref, or the official preprint page.
6. Preserve DOI, URL, publication venue, year, and author information when
   available.
7. Do not invent missing bibliographic fields.
8. Do not cite a paper that has not been verified.

## Editing Rules

* Preserve the paper title, author order, affiliations, and corresponding
  author information unless explicitly instructed otherwise.
* Preserve the existing LaTeX style and notation.
* Do not remove citations solely to shorten the manuscript.
* Do not substantially change technical claims without supporting evidence.
* Do not add unverified performance numbers, dates, or publication status.
* Keep terminology consistent throughout the manuscript.
* Do not introduce TMLR submission identifiers or private review information.

## Figure Rules

* Store source figures in `figures/`.
* Do not replace vector PDF figures with low-resolution screenshots.
* Ensure all figure files referenced in LaTeX are included in the repository.
* Preserve figure labels and cross-references when editing captions.

## Validation Checklist

After making changes:

1. Compile the complete manuscript.
2. Check for undefined citations.
3. Check for undefined references.
4. Check for duplicate BibTeX entries.
5. Confirm that all figures render correctly.
6. Confirm that author names and affiliations remain unchanged.
7. Review the Git diff and avoid unrelated formatting changes.

## Files That Must Not Be Committed

Do not commit:

* `.aux`
* `.log`
* `.out`
* `.bbl`
* `.blg`
* `.fls`
* `.fdb_latexmk`
* `.synctex.gz`
* private review correspondence
* submission IDs
* API keys or credentials
* Overleaf history or temporary files

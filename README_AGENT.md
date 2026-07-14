# Instructions for AI Agents

## Scope

This file provides instructions for AI agents working with the manuscript
source under the `Paper/` directory.

Unless explicitly requested otherwise:

- Modify only files under `Paper/`.
- Do not modify the repository-level `README.md`.
- Do not modify the repository-level curated resource list.
- Do not modify website files, assets, workflows, or other project resources.
- Do not reorganize the repository structure.

Before editing the manuscript, inspect the existing directory structure and
read the relevant source files.

## Repository Context

This repository contains resources associated with:

**Self-Improvements in Modern Agentic Systems: A Survey**

The repository serves more than one purpose. Its root directory contains the
project description and curated resources, while `Paper/` contains the LaTeX
source code, bibliography, figures, and supporting files for the manuscript.

The goal of work under `Paper/` is to maintain the manuscript in a consistent,
verifiable, and reproducible form.

## Canonical Files and Directories

The canonical manuscript files are:

- Main LaTeX entry point:
  `Paper/colm2025_conference.tex`
- Bibliography database:
  `Paper/colm2025_conference.bib`
- Section source files:
  `Paper/tex/`
- Figures and figure-related LaTeX files:
  `Paper/fig/`
- Shared mathematical commands:
  `Paper/math_commands.tex`
- Document style:
  `Paper/colm2025_conference.sty`
- Bibliography style:
  `Paper/colm2025_conference.bst`
- Local package dependencies:
  `Paper/natbib.sty` and `Paper/fancyhdr.sty`

The normally generated manuscript is:

```text
Paper/colm2025_conference.pdf
```

The generated PDF is a build artifact rather than a canonical source file.

Do not assume that files or directories named `main.tex`, `references.bib`,
`sections/`, or `figures/` exist.

## Compilation

Run compilation commands from the `Paper/` directory.

Preferred workflow:

```bash
cd Paper
latexmk -pdf -interaction=nonstopmode -halt-on-error colm2025_conference.tex
```

Manual alternative:

```bash
cd Paper
pdflatex -interaction=nonstopmode -halt-on-error colm2025_conference.tex
bibtex colm2025_conference
pdflatex -interaction=nonstopmode -halt-on-error colm2025_conference.tex
pdflatex -interaction=nonstopmode -halt-on-error colm2025_conference.tex
```

To remove ordinary build artifacts:

```bash
cd Paper
latexmk -c colm2025_conference.tex
```

Do not claim that compilation succeeded unless the compilation command
completed successfully.

If LaTeX, BibTeX, required fonts, or other dependencies are unavailable,
report the missing dependency clearly instead of claiming that the manuscript
has been validated.

## Editing Rules

- Preserve the paper title unless a title change is explicitly requested.
- Preserve author names, author order, affiliations, email addresses, and
  corresponding-author designations unless explicitly instructed otherwise.
- Preserve the existing LaTeX style, notation, labels, and directory layout.
- Keep changes minimal and limited to the requested task.
- Do not perform unrelated rewriting or reformatting.
- Do not rename source files, citation keys, labels, or figure files without a
  compelling reason and corresponding updates to every reference.
- Avoid modifying `.sty`, `.bst`, and local package files unless the requested
  task specifically concerns formatting or compilation.
- Do not remove citations solely to shorten the manuscript.
- Do not substantially change technical claims without supporting evidence.
- Do not add unverified performance numbers, publication dates, acceptance
  status, or bibliographic information.
- Keep terminology and mathematical notation consistent throughout the paper.
- Do not introduce private TMLR review information, submission identifiers,
  reviewer comments, or confidential correspondence.
- Do not state that the paper has been accepted or peer reviewed unless this
  status has been verified and the maintainers explicitly request the update.
- Do not assume that the repository-level license automatically determines the
  license of the manuscript, figures, or third-party materials.
- Do not alter copyright or licensing notices without maintainer approval.

## Bibliography Rules

1. Add new references to `Paper/colm2025_conference.bib`.
2. Do not manually write complete bibliographic records in the manuscript
   body.
3. Preserve existing BibTeX citation keys unless correcting an error.
4. Before adding an entry, check for duplicates using the title, DOI, arXiv ID,
   and author list.
5. Prefer metadata from authoritative sources such as:
   - the publisher;
   - the official conference or journal website;
   - DBLP;
   - Crossref;
   - the official arXiv page;
   - the authors' official project page.
6. Preserve author names, title capitalization, venue, year, page numbers,
   DOI, URL, and arXiv identifiers when available.
7. Use braces in BibTeX titles when needed to preserve capitalization of terms
   such as `LLM`, `AI`, `GPT`, and proper names.
8. Do not invent missing bibliographic fields.
9. Do not cite a paper that has not been verified.
10. Do not silently replace a cited paper with a different work.
11. When replacing a preprint record with its published version, verify that
    both records refer to the same work.
12. Preserve the existing citation key when updating a preprint to its
    published version whenever practical.
13. Do not change an author's name spelling merely to normalize formatting
    without checking the authoritative publication record.

## Figure Rules

- Store manuscript figures and figure-related source files under `Paper/fig/`.
- Treat existing PDF files under `Paper/fig/` as source assets, not disposable
  build artifacts.
- Prefer vector PDF figures over low-resolution screenshots.
- Do not replace a vector figure with a rasterized version unless explicitly
  requested.
- Ensure that every figure referenced by LaTeX exists in the repository.
- Preserve figure filenames, labels, captions, and cross-references unless the
  requested change requires updating them.
- Do not add third-party figures without checking their license and reuse
  permissions.
- Do not crop, compress, recolor, or redraw figures in a way that changes their
  scientific meaning.
- Do not delete apparently unused figures without verifying that they are not
  referenced indirectly by an included LaTeX file.

## Validation Checklist

After making changes:

1. Compile the complete manuscript.
2. Check the build log for LaTeX errors.
3. Check for undefined citations.
4. Check for undefined references.
5. Check for duplicate BibTeX entries.
6. Confirm that all figures render correctly.
7. Confirm that the table of contents and cross-references are updated.
8. Confirm that author names, author order, and affiliations remain unchanged
   unless their modification was explicitly requested.
9. From the repository root, run:

   ```bash
   git diff --check
   git status --short
   ```

10. Review the complete Git diff.
11. Remove unrelated formatting and whitespace changes.
12. Confirm that no files outside `Paper/` were modified unless explicitly
    requested.
13. Report warnings, unresolved issues, and checks that could not be completed.

## Generated Files

Do not commit ordinary temporary LaTeX build files, including:

```text
Paper/*.aux
Paper/*.blg
Paper/*.fdb_latexmk
Paper/*.fls
Paper/*.log
Paper/*.lof
Paper/*.lot
Paper/*.out
Paper/*.synctex.gz
Paper/*.toc
```

Do not commit the following unless explicitly requested:

```text
Paper/colm2025_conference.pdf
Paper/*.bbl
Paper/*.dvi
Paper/*.ps
```

A `.bbl` file may occasionally be required by a submission platform. Commit it
only when the maintainers explicitly request it.

PDF files under `Paper/fig/` are manuscript source figures and must not be
deleted or ignored merely because they use the `.pdf` extension.

## Sensitive and Private Files

Never commit:

- private review correspondence;
- reviewer identities or comments;
- confidential TMLR submission information;
- submission-system screenshots;
- private submission identifiers;
- API keys, passwords, tokens, or credentials;
- private Overleaf history;
- local backup files;
- local editor settings containing personal information;
- unpublished author correspondence;
- files containing information that the authors have not approved for public
  release.

## Completion Criteria

A task is complete only when:

- the requested change has been made;
- the manuscript compiles successfully, or missing build dependencies have
  been clearly reported;
- no new undefined citations or references were introduced;
- no unrelated files were modified;
- files outside `Paper/` were left unchanged unless explicitly requested;
- the final Git diff was reviewed;
- all remaining warnings and limitations were disclosed.

When reporting completion, briefly summarize:

1. what was changed;
2. which files were modified;
3. which validation commands were run;
4. whether compilation succeeded;
5. any unresolved warnings or limitations.

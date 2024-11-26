# Thesis Template

This repository contains the LaTeX template for a doctoral thesis. The template is organized into multiple files and folders to facilitate modular and maintainable document structure.

## Structure

### Files and Directories
- **`frontpage.tex`**: Contains the settings and layout for the first page of the thesis, i.e., the cover. This file is compiled separately when necessary.
- **`kappa/`**: Contains the main chapters of the thesis, including:
  - `abstract.tex`: Abstract of the thesis.
  - `contributionstatement.tex`: Statement outlining the author's contributions.
  - `acknowledgements.tex`: Acknowledgment section.
  - `introduction.tex`: Introduction to the thesis.
  - `background.tex`: Background section providing context for the research.
  - `conclusions.tex`: Summary of contributions and a discussion of future work.
- **`papers/`**: Contains the included papers that support the thesis. Each paper should be organized in its own subfolder with a `main.tex` file for its content.
- **`Thesis.bib`**: Bibliography file in BibTeX format. Additional BibTeX files can be used, but ensure no overlapping entries to avoid compilation errors.
- **`macros.tex`**: Custom LaTeX macros used across the document.

## Compilation Instructions

### Requirements
Ensure you have the following installed:
- A LaTeX distribution (e.g., TeX Live, MiKTeX, or MacTeX).
- BibTeX for bibliography management.

### Makefile Commands
The `Makefile` supports the following commands:
- **`make frontpage`**: Compiles only the `frontpage.tex` file to generate the cover page.
- **`make all`**: Compiles the entire thesis, including the frontpage, kappa, and papers.
- **`make clean`**: Removes all generated files, including the compiled PDFs.
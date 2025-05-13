# LaTeX Resume Project

This project contains LaTeX templates and content for generating a professional resume.

## Directory Structure

- **`/MTeck`**: Contains a modern, styled resume template (`resume.tex`) and the raw text content (`resume_content.txt`) used to populate it.
- **`/og`**: Contains an original, simpler resume template (`resume_og.tex`).

## Key Files

- **`MTeck/resume.tex`**: The main resume file using the MTeck styling. This is likely the primary resume you'll be using.
- **`MTeck/resume_content.txt`**: A plain text file containing the skills and experience details. This content is used to populate both `MTeck/resume.tex` and `og/resume_og.tex`.
- **`og/resume_og.tex`**: A resume file using a more traditional and simpler LaTeX format.
- **`README.md`**: This file, providing an overview of the project.
- **`requirements.txt`**: Lists the LaTeX packages used by the resume templates.

## Installing LaTeX

To compile LaTeX documents (`.tex` files) into PDFs, you need a LaTeX distribution installed on your system. A distribution bundles the LaTeX compiler with common packages and tools.

- **For macOS (Recommended):**
  [**MacTeX**](https://www.tug.org/mactex/) is a comprehensive TeX distribution specifically for macOS. It includes TeX Live (a full TeX system), the TeXShop editor, and other useful utilities.

- **Cross-Platform:**
  [**TeX Live**](https://www.tug.org/texlive/) is a major TeX distribution that works on most operating systems, including macOS, Windows, and Linux.

- **Primarily Windows (also available for macOS/Linux):**
  [**MiKTeX**](https://miktex.org/) is another popular TeX distribution, known for its on-the-fly package installation. It's primarily used on Windows but has versions for macOS and Linux.

Choose one and follow the installation instructions on its website. After installation, you should be able to use the `pdflatex` command from your terminal.

## How to Compile

To generate a PDF from the LaTeX files, you will need a LaTeX distribution installed (e.g., TeX Live, MiKTeX, or MacTeX for macOS).

Navigate to the directory containing the `.tex` file you want to compile and run the `pdflatex` command. For example:

1.  **To compile the MTeck resume:**
    ```bash
    cd MTeck
    pdflatex resume.tex
    ```
    You may need to run `pdflatex` twice to ensure all cross-references (like page numbers or citations, if any) are correctly generated.

2.  **To compile the original resume:**
    ```bash
    cd og
    pdflatex resume_og.tex
    ```
    Similarly, run twice if needed.

## LaTeX Dependencies

The LaTeX packages required for these templates are listed in `requirements.txt`. Most modern LaTeX distributions will either come with these packages pre-installed or will offer to install them automatically when you first compile a document that uses them. If you encounter errors related to missing packages, you may need to install them manually using your LaTeX distribution's package manager (e.g., `tlmgr` for TeX Live).

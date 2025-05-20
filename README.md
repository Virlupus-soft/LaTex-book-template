# Virlupus Book LaTeX Template v1.0

## ✨ Overview

This LaTeX template is designed for typesetting **popular science**, **literature**, and **educational books** in an elegant, professional format suitable for A5 paper. It supports both **print** and **digital (PDF)** formats while preserving high typographical quality.

## 📄 Document Class and Layout

- Based on the `book` class with `a5paper` and `12pt` font.
- Optimized margins via the `geometry` package.
- Beautiful typography using modern fonts (`mlmodern`, optionally `libertinus` or `romande`).

## 🔍 Key Features

### Typography

- Intelligent line-breaking (`nowidow`) for clean paragraphs.
- Multicolumn support (`multicol`)
- Longtable and advanced tabular environment with `longtable`, `array`.

### Indexing

- Uses `imakeidx` for advanced multi-level indexing.

- Sample index entries are included as a demonstration of good practices:

  ```latex
  \index{Physics!Laws!Newton first law}
  \index{Newton!gravity}
  \index{Theorems!pythagorean}
  ```

- Output index typeset using `\printindex`, optionally in a smaller font:

  ```latex
  {\small \printindex}
  ```

### Math and Science Support

- `amsmath`, `amssymb`, `amsfonts` for mathematics

- `physics`, `chemexec`, `physunits` for physical and chemical notation

- Custom operators and macros for clarity:

  ```latex
  \DeclareMathOperator{\tg}{tg}
  \newcommand{\DV}[2]{\frac{\Delta #1}{\Delta #2}}
  ```

### Visual Elements

- `tcolorbox` for framed environments: `remember`, `important`, `note`, etc.
- Theorem-like structures (`define`, `theorem`, `proof`) styled for readability.
- `quotchap` for elegant chapter openings with quotations.
- `fancyhdr` + `pgfornament` for decorative headers.

### Hyperlinks

- Full `hyperref` and `hypcap` support.

- Clean, non-intrusive links using:

  ```latex
  \hypersetup{
      pdfborder=0 0 0,
      colorlinks=true,
      linkcolor=DarkSlateGrey,
      urlcolor=DarkSlateGrey,
      citecolor=DarkSlateGrey
  }
  ```

- Works beautifully in both printed and digital form.

## 📘 Title Page Example

Simple, manual title page example is included. Modify freely:

```latex
\begin{titlepage}
  \begin{center}
    {\Huge The Sample of a Book}\\[5mm]
    {\large \textbf{PhDr. Mgr. Virlupus Volchv}}\\[10mm]
    \includegraphics[width=0.1\textwidth]{logo.png}\\
    {\small Schola Versipellem}\\
    {\footnotesize Jihlava}\\
    {\scriptsize \today}\\
    {\scriptsize version 1.0}
  \end{center}
\end{titlepage}
```

## 🎓 Target Audience

- Authors of educational materials
- Writers of essays or scientific overviews
- Small publishers and students
- Teachers preparing structured print/PDF handouts

## 🌐 Output Format

- Produces clean, hyperlinked PDFs.
- Suitable for print with margins and readability taken into account.
- Index, ToC, references and citations are supported natively.

## ⚙️ Requirements

- Modern TeX distribution (TeX Live 2023+, MiKTeX, etc.)
- Compilation via `pdfLaTeX`

## 💼 Licensing

- Distributed under **GNU GPL v2 or later**.
- Free for personal, academic, or commercial use.

## 💭 Notes

- Consider expanding the template with `biblatex` for bibliography.
- Support for `appendix`, glossary, or additional theorem environments is easy to add.
- Clean separation of content and layout helps new authors focus on writing.

------

© 2025 Virlupus Software. All authors welcome. Improve, fork, and share.
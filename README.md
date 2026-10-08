# SEPOC 2026 Beamer theme

A Beamer recreation of the supplied SEPOC 2026 PowerPoint template.

## Files

- `beamerthemeSEPOC2026.sty`: main theme
- `beamercolorthemeSEPOC2026.sty`: colors
- `beamerfontthemeSEPOC2026.sty`: typography
- `assets/`: images extracted from the supplied PPTX
- `main.tex`: minimal example

## Compilation

Use XeLaTeX or LuaLaTeX because the theme uses `fontspec` and Roboto:

```bash
xelatex main.tex
```

The document should be compiled from the theme directory so that `assets/` is found.

## Usage

```latex
\documentclass[aspectratio=169,11pt]{beamer}
\usetheme{SEPOC2026}

\title{Title}
\author{Author}
\institute{Institution}

\begin{document}
\begin{frame}\titlepage\end{frame}
\begin{frame}{Title}
  Content
\end{frame}
\end{document}
```

# Presentation Template Repository

This repository provides a structured LaTeX template for preparing presentations, handouts, and full-text documentation from a single source.

It includes three main files:

- **`slides.tex`**  
  This file is used to generate the main presentation using the [Beamer](https://ctan.org/pkg/beamer) class. It contains only the content that is shown during the talk.

- **`handout.tex`**  
  An article-style handout version of the presentation. It includes both the
  slide content and additional notes or commentary that are not visible in the
  actual presentation. This handout is intended to be distributed after the
  talk and should be self-contained and understandable even for those who did
  not attend the presentation.

- **`presentation.tex`**  
  This is the master source file that contains the full content of the talk.  
  - Content inside `\begin{frame}...\end{frame}` is included in both the
    presentation and the handout.  
  - Content outside of frames (e.g., commentary or explanations) is excluded
    from the slides but included in the handout.  

This structure allows you to maintain a single source of truth while producing both a polished presentation and an informative, reader-friendly version of the talk.

## Compile Instructions

You can compile the output files using any standard LaTeX distribution that includes Beamer and the necessary packages:

```bash
$ lualatex slides.tex
$ lualatex handout.tex
```

## HTML version






## License

Feel free to reuse or adapt this template for your own presentations.



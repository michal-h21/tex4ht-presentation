# Presentation Template Repository

This repository provides a structured LaTeX template for preparing presentations, handouts, and full-text documentation from a single source.

This template is designed for presentations that need more than just slides. It
lets you create both the talk itself and a more detailed handout with notes and
commentary. That way, you can generate everything from a single source—both the
material for the live talk and something meaningful for people who didn’t
attend.

It includes four main files:

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

- **`preamble.tex`**
  This file should include packages or define commands which are used in the presentaion.

## Compile Instructions

You can compile the output files using any standard LaTeX distribution that includes Beamer and the necessary packages.

To compile the presentation or the handout to PDF using LuaLaTeX, run the following commands:

```bash
$ lualatex slides.tex
$ lualatex handout.tex
```

## HTML version


You can also generate an HTML version of the handout using [TeX4ht](https://www.tug.org/tex4ht/):

```bash
$ make4ht -l handout.tex
```

The `-l` option ensures that LuaLaTeX is used as the compiler.



## License

Feel free to reuse or adapt this template for your own presentations.



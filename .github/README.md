# `collabcomment`

The `collabcomment` package makes leaving comments for your
collaborators a better experience. While many such packages already
exist, `collabcomment` is unique due to its simplicity and implementation in
LaTeX3, without losing the power of comparable packages. It supports the following
features:
- Leave coloured comments and to-dos in your LaTeX document.
- Create custom authors with their own colour.
- Comments and to-dos are numbered and fully compatible with `hyperref`.
- Collect all to-dos/comments into a hyperlinked list grouped by author.
- Use the `final` package option to get rid of all comments and lists.
- Mark to-dos as complete to remove them from the text, but still
appear in the to-do list.

# Installation
Run the following in the command line:
1. If collabcomment.ins is present:
    `pdflatex collabcomment.ins`
2. If collabcomment.ins is absent:
    `pdflatex collabcomment.dtx`

Move `.sty` and `.cls` files to a folder that TeX can find.

# Documentation
Run the following in the command line:
```
pdflatex collabcomment.dtx
makeindex -s gind.ist -o collabcomment.ind collabcomment.idx
makeindex -s gglo.ist -o collabcomment.gls collabcomment.glo
pdflatex collabcomment.dtx
pdflatex collabcomment.dtx
```
This automatically unpacks the package, as well.

If you are looking for comments or documentation, you won't find
any in the source. These packages make use of literate programming, which means
that the documentation is given in the form of a pdf file. You can
probably find collabcomment.pdf in this folder, by running "texdoc --view collabcomment"
in the command line, or Googling
"[your distribution] how to find package documentation".
If you're using MiKTeX, open MiKTeX console, go to
"Documentation" and look for "collabcomment".

---

&copy; 2026- Jesse Straat

License: [LPPL1.3c](https://www.latex-project.org/lppl.txt)

[GitHub Repository](https://github.com/JesseStraat/collabcomment)



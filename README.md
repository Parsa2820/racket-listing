# racket-listing
Racket language syntax highlighting for LaTex listings package

## Table of Content
- [How to Use?](How-to-Use?)

## How to Use?
There are two ways to use LaTeX package in your document.

1. Put `racket-listing.sty` file beside your document.
2. Put `racket-listing.sty` file in your TeX local texmf folder. `/usr/local/texmf-dist/tex/latex` on Unix-like and `C:\texlive\texmf-local\tex\latex` on Windows (These are default path for TeXLive). Then update file name database (Run `mktexlsr` for TeXLive).

I myself prefer the former way, because the latter one make your document less portable.

After placing `racket-listing.sty` using either methods, add `\usepackage{racket-listing}` command to the beginnig of your documnet. You can pass `overleafstyle` as option to set prepared style in the package (`\usepackage[overleafstyle]{racket-listing}`), Otherwise set your own style using [listings package](https://ctan.org/pkg/listings).

Now you can use `language=racket` option in any listings environment.

See an example code in [sample.tex](./sample.tex) and an example output in [sample.pdf](./sample.pdf).

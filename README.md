# Latex WSConfig

Hi! The main contribution of this project is a `TEX` file which can be included from your main `TEX` file.

When you do that, this file will use some packages to improve your document, and also will keep most of config and usepackages statements away from your text. The project organization and readability is better this way.

![](assets/2022-11-25-00-34-57.png)

## Usage

### Simplest way

Get the file `wsconfig.tex` and place in the same directory your main latex file is located. The minimum code to start is this:

```latex
\documentclass{article}
\input{wsconfig.tex}

\begin{document}
Hello World!
\end{document}
```

The customizations (like packages, preamble configurations, etc.) can be done inside the `wsconfig.tex`. 

### Cloning the GitHub repository

The developer use to create content in LaTeX using Visual Studio Code and the extension LaTeX Workshop.

The workflow is:

1. Clone the repo
2. Enter the directory
3. Rename the `blank.tex` file to whathever you need
4. Open the directory in VSCode (`$ code .`)
5. Edit the text file while see the preview in VSCode
6. A lot of files will be created, you can run `make` to remove them

## Document Types

As the developer is a Brazilian student who needs to write both in portuguese and english, this configuration supports the ABNT standard via the abntex2 class. The following classes have been tested:

- article
- memoir
- report
- abntex2

## Packages

This configuration includes some of the most used packages. This is the list:

- afterpage
- amsfonts
- amsmath
- amsthm
- array
- biblatex
- booktabs
- csquotes
- fancybox
- fancyhdr
- fetchcls
- fontenc
- geometry
- graphicx
- hyperref
- ifthen
- indentfirst
- inputenc
- lipsum
- listings
- lmodern
- microtype
- multirow
- nomencl
- pagecolor
- pgfplots
- setspace
- siunitx
- tabularx
- tcolorbox
- tikz
- url
- xcolor

If you have any question, please, fill-up an issue at GitHub.

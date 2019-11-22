# paper-template

A LaTex template for research papers.

## Setup

Use [`latexmk`](https://www.ctan.org/pkg/latexmk/?lang=en). My current workflow is to 1. write text in Vim; 2. run `latexmk -pvc` in the terminal with Skim setup to automatically refresh the document when changes are made:

```bash
# place this in the latexmkrc file
$pdf_mode = 1;
$postscript_mode = 0;
$dvi_mode = 0;
$pdf_previewer = "open -a /Applications/Skim.app";
$clean_ext = "paux lox pdfsync out";
```

There are a few more changes that need to be made to make this workflow confortable. A full description can be found at [Jeremy Kun's blog](https://jeremykun.com/2015/01/10/my-latex-workflow-latexmk-sharelatex-and-stackedit/). I typically link a new paper's github repository with overleaf.

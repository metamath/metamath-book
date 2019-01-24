# metamath-book

This is the LaTeX editable source of the book
_Metamath: A Computer Language for Pure Mathematics_,
also known as the Metamath book.
This book provides an in-depth understanding of the Metamath language and
program. The first part of the book also includes an easy-to-read informal
discussion of abstract mathematics and computers, with references to
other proof verifiers and automated theorem provers.

This material is released to the public domain (no copyright) worldwide.
However, although it is not a legal requirement, we do ask that you
give credit.

Note: In December 2018, the predicate calculus axioms were renumbered and
no longer match those in Sections 3.3.2 and 3.3.3 of the 2014 version
of the book. A cross reference between the new and old numbers can be
found in Appendix 8 of the Metamath Proof Explorer Home Page.

## Editing

To edit the text, simply edit file metamath.tex.

## Generating a PDF

The source is in LaTeX format.
To generate a PDF, you first need to install

- The programs pdflatex, bibtex, makeindex
- The style file anysize.sty

On Cygwin, you can install all prerequisites by installing these packages:

- texlive
- texlive-collection-latex
- texlive-collection-bibtexextra
- texlive-collection-latexrecommended

See the file "metamath.tex" for how to generate a PDF file.

## Citation

BibTeX citation:

~~~~
@Book{metamath,
author = {Norman D. Megill},
title = {Metamath: A Computer Language for Pure Mathematics},
year = {2007},
publisher = {Lulu Press},
address = {Morrisville, North Carolina},
note = {{\tt http://us.metamath.org/downloads/metamath.pdf}},
}
~~~~

## Narrow width screens

You can run ./make-narrow to generate "metamath-narrow.pdf",
a version of the PDF formatted for
narrow-width screens (such as mobile phones).
The program erases metamath.pdf, so you'll need to regenerate metamath.pdf
afterwards if you want it.

That work is based on
an old version of this book that was generated specifically for
narrow-width screens called the "Kindle version".
The changes that implemented the Kindle version are in
file kindle-changes.patch.  We keep the .patch file around so that
we can borrow future ideas in the future.

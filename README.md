# metamath-book

[![Build Status](https://api.travis-ci.com/metamath/metamath-book.svg)](https://travis-ci.com/metamath/metamath-book)

This is the LaTeX editable source of the book
_Metamath: A Computer Language for Pure Mathematics_,
also known as the Metamath book.
This book provides an in-depth understanding of the Metamath language and
program. The first part of the book also includes an easy-to-read informal
discussion of abstract mathematics and computers, with references to
other proof verifiers and automated theorem provers.

This material is released to the public domain (no copyright) worldwide per the
[Creative Commons CC0 1.0 Universal (CC0 1.0) Public Domain Dedication](https://creativecommons.org/publicdomain/zero/1.0/);
here is [our copy of the CC0 license](./LICENSE.md).
This license has the SPDX license identifier CC0-1.0.
However, although it is not a legal requirement, we do ask that you
give credit.

Note: In December 2018, the predicate calculus axioms were renumbered and
no longer match those in Sections 3.3.2 and 3.3.3 of the 2014 version
of the book. A cross reference between the new and old numbers can be
found in Appendix 8 of the Metamath Proof Explorer Home Page.

## Editing

To edit the text, simply edit file metamath.tex.

If you generate example displays from the Metamath program,
use 61 characters per line
(you can use the command `set width 61` to do this).

## Generating a PDF

The source is in LaTeX format.
To generate a PDF, you first need to install

- The programs pdflatex, bibtex, makeindex
- The style file anysize.sty

On Ubuntu, you can install all prerequisites by installing these packages:

- texlive-fonts-recommended
- texlive-latex-extra
- texlive-fonts-extra
- dvipng
- texlive-latex-recommended

On Cygwin, you can install all prerequisites by installing these packages:

- texlive
- texlive-collection-latex
- texlive-collection-latexextra
- texlive-collection-bibtexextra
- texlive-collection-latexrecommended

On a Unix-like system you can simply run the script `./generate-pdf`
to generate a normal PDF
(or `./make-narrow` to generate a narrow version).
To generate both, run the commands sequentially in this order
(you have to run make-narrow *first*):

~~~~
./make-narrow
./generate-pdf
~~~~

See the file `metamath.tex` for detailed instructions
how to generate a PDF file by hand.

## Citation

BibTeX citation:

~~~~
@Book{metamath,
author = {Norman D. Megill and David A. Wheeler},
title = {Metamath: A Computer Language for Pure Mathematics},
year = {2019},
publisher = {Lulu Press},
address = {Morrisville, North Carolina},
url = {http://us.metamath.org/downloads/metamath.pdf},
note = {{\tt http://us.metamath.org/downloads/metamath.pdf}},
}
~~~~

## Narrow width screens

You can run `./make-narrow` to generate "metamath-narrow.pdf",
a version of the PDF formatted for
narrow-width screens such as mobile phones.
The program erases metamath.pdf, so you'll need to regenerate metamath.pdf
afterwards if you want it also.
The program also manipulates some files, so you need to run these
programs sequentially (one at a time) if you are running them in the
same directory.

The narrow version is based on
an old version of this book that was generated specifically for
narrow-width screens called the "Kindle version"
by John D. Baker in 2011.
The changes that implemented the Kindle version are in
file kindle-changes.patch.  We keep the .patch file around so that
we might be able to borrow more of its ideas in the future.

## Contributions

We love contributions!
If you have an improvement for the text, or for generation
(such as improving how metamath-narrow.pdf works),
please create a pull request.
Contributions must be under the same license (release to the public domain
under CC0).

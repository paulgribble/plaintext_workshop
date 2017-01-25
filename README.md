*caution: still a work in progress*

# plaintext_workshop

A workshop on Scientific Writing using plaintext tools like LaTeX,
Markdown & pandoc

February 21, 2017, 12:00pm---5:00pm, NSC 245A

# Why?

- separates content from formatting
- universally readable
- platform independent
- future-proof
- free and open source
- version control

There are many blog posts out there about the virtues of using plaintext to do scientific (or more generally, academic) writing. Here are some:

- [Sustainable Authorship in Plain Text using Pandoc and Markdown](http://programminghistorian.org/lessons/sustainable-authorship-in-plain-text-using-pandoc-and-markdown)
- [Academic Writing With Markdown](http://dylanstorey.com/2015/12/Academic_Writing_With_Markdown.html)
- [Why (and How) I Wrote My Academic Book in Plain Text](http://wcm1.web.rice.edu/my-academic-book-in-plain-text.html)
- [Markdown vs Latex for Academic Writing](http://jabranham.com/blog/2015/09/rmarkdown-vs-latex/)
- [Writing Technical Papers with Markdown](http://blog.kdheepak.com/writing-papers-with-markdown.html)


# Software

If you're on MacOS it would be a good idea to
install [Homebrew](http://brew.sh), a package manager that gives you
easy access to installing all sorts of useful GNU/Linux tools.

- [LaTeX](https://www.latex-project.org)
  - MacOS: [MacTeX](http://www.tug.org/mactex/)
  - GNU/Linux: [TeX Live](https://wiki.debian.org/Latex)
  - Windows: [MiKTeX](https://miktex.org)
- [pandoc](http://pandoc.org/installing.html)

You will need a good text editor as well. There are many to choose
from. Here are a few:

- [Emacs](https://www.gnu.org/software/emacs/)
- [Vim](http://www.vim.org/download.php)
- [Sublime Text](https://www.sublimetext.com)
- [Atom](https://atom.io)
- [BBEdit](http://www.barebones.com/products/bbedit/index.html)
- [Notepad++](https://notepad-plus-plus.org)
- [Visual Studio Code](https://code.visualstudio.com)
- [Gedit]()

There are some GUI-based LaTeX editors as well:

- [TeXmaker]()
- [TeXstudio]()
- [TeXworks]()

There are online LaTeX editors/compilers/environments:

- [ShareLaTeX]()
- [Overleaf]()

And there are many Markdown editors, here are some:

- [iA Writer]()
- [Marked]()
- [MacDown]()
- [Bear]()
- [Ulysses]()
- [Typora]()
- [Mou](http://25.io/mou/)

## Markdown

- [Markdown](http://daringfireball.net/projects/markdown/): The
  original specification by John Gruber
- [Mastering Markdown](https://guides.github.com/features/mastering-markdown/):
  a brief tutorial by GithHub

- if you need a hard line break, put two or more spaces at the end of a line


## Pandoc

- [Getting started with pandoc](http://pandoc.org/getting-started.html)
- [Pandoc Demos](http://pandoc.org/demos.html)
- [Pandoc FAQs](http://pandoc.org/faqs.html)
- [Pandoc Manual](http://pandoc.org/MANUAL.html)
- [Pandoc crossref](https://github.com/lierdakil/pandoc-crossref) for
  numbering figures, equations, tables and cross-references to them
- [Pandoc citeproc](https://github.com/jgm/pandoc-citeproc) for
  citations & bibliographies
- [Citation Style Language (CSL) citation styles](https://github.com/citation-style-language/styles)

## LaTeX

- [LaTeX Font Catalogue](http://www.tug.dk/FontCatalogue/)

## Markdown vs LaTeX

- Markdown has arguably nicer looking syntax
- Markdown has more output formats (via pandoc)
- LaTeX provides more control over fine-grained appearance

With pandoc you can take advantage of both. Provide pandoc with a
LaTeX template, containing all of the formatting details you want, and
keep the content in Markdown format.


# Writing in Markdown

## Using Pandoc to create a pdf

[variables for LaTeX](http://pandoc.org/MANUAL.html#variables-for-latex)

Some examples:

Basic document creation with all of the LaTeX defaults:

	pandoc doc1.md -o doc1.pdf

Let's make the sections and subsections numbered:

	pandoc doc1.md -o doc1.pdf -N

Let's change the font to 12pt

	pandoc doc1.md -o doc1.pdf -N --variable fontsize=12pt

Let's change the font to Palatino (the default LaTeX font is called
Computer Modern):

	pandoc doc1.md -o doc1.pdf -N -V fontsize=12pt -V
    mainfont=Palatino --latex-engine=xelatex

The page margins are to small for us, let's make them 1-inch all around:

	pandoc doc1.md -o doc1.pdf -N -V fontsize=12pt -V
    mainfont=Palatino --latex-engine=xelatex -V geometry:margin=1in

## Where to put the formatting codes?

### on the command line

  pandoc doc1.md -o doc1.pdf -N -V fontsize=12pt -V
    mainfont=Palatino --latex-engine=xelatex -V geometry:margin=1in

Above we put various formatting codes (font, margins, etc) in the command-line command to run pandoc. There are other ways to do it.

### in a YAML header in the main document

    ---
    title: Hunting Replicants
    author: Rick Deckard
    date: November 1, 2019
    papersize: letter
    mainfont: "Myriad Pro"
    fontsize: 12pt
    geometry: margin=1.2in
    ---

Here we include, along with the title, author and date, various formatting options in the main document itself. Now to convert the plaintext document `ms.md` to pdf we can issue a simpler command:

    pandoc ms.md -o ms.pdf --latex-engine=xelatex

We include the `--latex-engine=xelatex` option in the pandoc command, because we are asking for a nonstandard font. When converting to pdf, pandoc does this via LaTeX using the `pdflatex` conversion engine as a default. Unfortunately `pdflatex` doesn't handle non-default fonts particularly well (or at least, it's not very flexible). The `xelatex` LaTeX conversion engine handles fonts much more flexibly and allows you to use any font that's installed on your computer. Above I chose `Myriad Pro`.

### in a separate file

We can put the formatting stuff into a separate file, called say `formatting.yaml`:

    ---
    papersize: letter
    mainfont: "Myriad Pro"
    fontsize: 12pt
    geometry: margin=1.2in
    ---

and leave the header of our main document for just the content, no formatting:

    ---
    title: Hunting Replicants
    author: Rick Deckard
    date: November 1, 2019
    ---

The advantage of this is we really do separate out content from formatting. Now the command to convert from `ms.md` to pdf would be:

    pandoc ms.md -o ms.pdf formatting.yaml --latex-engine=xelatex

We include `formatting.yaml` to tell pandoc to include the header info found in the file `formatting.yaml` when performing the conversion.









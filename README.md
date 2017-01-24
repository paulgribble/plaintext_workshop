*caution: still a work in progress*

# plaintext_workshop

A workshop on Scientific Writing using plaintext tools like LaTeX,
Markdown & pandoc

February 21, 2017, 12:00pm---5:00pm, NSC 245A

# Why?

- version control
- platform independence
- free and open source
- separates content from formatting
- universally readable
- future-proof

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
  
Just do a google search for `pandoc for scientific writing` and you
will see many useful blog entries, tutorials and manifestos. Here is
one:

  [Writing Technical Papers with Markdown](http://blog.kdheepak.com/writing-papers-with-markdown.html)

## Pandoc

- [Getting started with pandoc](http://pandoc.org/getting-started.html)
- [Pandoc Demos](http://pandoc.org/demos.html)
- [Pandoc FAQs](http://pandoc.org/faqs.html)
- [Pandoc Manual](http://pandoc.org/MANUAL.html)

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



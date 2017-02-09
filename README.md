
# plaintext_workshop

A workshop on Scientific Writing using plaintext tools like LaTeX,
Markdown & pandoc

February 21, 2017, 12:00pm---5:00pm, NSC 245A

# Why plaintext?

- separates content from formatting
- universally readable
- platform independent
- future-proof
- free and open source
- can easily use version control (e.g. [Git](https://git-scm.com) & [GitHub](https://github.com))
- can easily compare old vs new (e.g. opendiff (FileMerge) on OS X, e.g. [Meld](http://meldmerge.org) on Linux) 

There are many blog posts out there about the virtues of using plaintext to do scientific (or more generally, academic) writing. Here are some of them:

- [Sustainable Authorship in Plain Text using Pandoc and Markdown](http://programminghistorian.org/lessons/sustainable-authorship-in-plain-text-using-pandoc-and-markdown)
- [Academic Writing With Markdown](http://dylanstorey.com/2015/12/Academic_Writing_With_Markdown.html)
- [Why (and How) I Wrote My Academic Book in Plain Text](http://wcm1.web.rice.edu/my-academic-book-in-plain-text.html)
- [Markdown vs Latex for Academic Writing](http://jabranham.com/blog/2015/09/rmarkdown-vs-latex/)
- [Writing Technical Papers with Markdown](http://blog.kdheepak.com/writing-papers-with-markdown.html)

# Software

If you're on MacOS it would be a good idea to install [Homebrew](http://brew.sh), a package manager that gives you easy access to installing all sorts of useful GNU/Linux tools including some of the tools listed here.

First let's **install LaTeX**. It's a large download. If you're on a Mac, install LaTeX using the downloadable binary installer. If you're on Ubuntu or another debian-based GNU/Linux, `sudo apt-get install texlive-full`.

- [LaTeX](https://www.latex-project.org)
  - MacOS: [MacTeX](http://www.tug.org/mactex/)
  - GNU/Linux: [TeX Live](https://wiki.debian.org/Latex)
  - Windows: [MiKTeX](https://miktex.org)

Next let's **install pandoc** and some extras. 

If you're on a Mac, and if you've installed homebrew, you can install pandoc using: `brew install pandoc pandoc-citeproc pandoc-crossref`. On GNU/Linux, I'm sure you can figure it out. I think pandoc is available using `sudo apt-get install pandoc` but I'm not sure about pandoc-citeproc and pandoc-crossref. Some googling should bring you an answer.

- [pandoc](http://pandoc.org/installing.html)

You will need a good **text editor** as well. There are many to choose from. Personally I use Emacs and Sublime Text. For our purposes here we don't need much sophistication so it comes down to personal preference.

Here is a list of some text editors:

- [Emacs](https://www.gnu.org/software/emacs/)
- [Vim](http://www.vim.org/download.php)
- [Sublime Text](https://www.sublimetext.com)
- [Atom](https://atom.io)
- [BBEdit](http://www.barebones.com/products/bbedit/index.html)
- [Notepad++](https://notepad-plus-plus.org)
- [Visual Studio Code](https://code.visualstudio.com)
- [Gedit](https://wiki.gnome.org/Apps/Gedit)

There are some GUI-based LaTeX editors as well, if you're into that sort of thing (I'm not): 

- [TeXmaker](http://www.xm1math.net/texmaker/)
- [TeXstudio](http://www.texstudio.org)
- [TeXworks](https://www.tug.org/texworks/)

There are also online LaTeX editors/compilers/environments. The advantage is that you don't have to install LaTeX locally on your own machine, and you don't have to worry about installing packages and updating outdated packages (they are all in the cloud). The disdvantage is that you can't do anything if you're not connected to the internet.

- [ShareLaTeX](https://www.sharelatex.com)
- [Overleaf](https://www.overleaf.com)

There are also many, many Markdown-specific editors. This means they are meant for editing Markdown in particular, and they come with various kinds of built-in smarts for pretty-formatting Markdown.

Here are some:

- [iA Writer](https://ia.net/writer/)
- [Marked](http://marked2app.com)
- [MacDown](https://macdown.uranusjr.com)
- [Bear](http://www.bear-writer.com)
- [Ulysses](https://www.ulyssesapp.com)
- [Typora](https://typora.io)
- [Mou](http://25.io/mou/)

If you're using Sublime Text (as I am) there is a nice Markdown plugin called [MarkdownEditing](https://github.com/SublimeText-Markdown/MarkdownEditing).

# Markdown

Let's start with Markdown, rather than LaTeX, since Markdown is less intimidating.

Markdown is a specification for "marking up" plain text documents using not-terribly-difficult-or-offensive codes that denote semantic elements. By "semantic elements" I mean things like headings, sub-headings, quotes, and so on. There are also variants of Markdown, such as Git-Markdown, that add various other codes to further extend Markdown's capabilities.

This document that you're reading (`README.md`) is a Markdown document. If you're reading it on GitHub, it's been rendered for you in your web browser by GitHub.

Here are some Markdown references online:

- [Markdown](http://daringfireball.net/projects/markdown/): The original specification by John Gruber
- [Mastering Markdown](https://guides.github.com/features/mastering-markdown/): a brief tutorial by GithHub

Here is a very simple Markdown document:

```
# Chapter 1

It was a bright cold day in April, and the clocks were striking thirteen. Winston Smith, his chin nuzzled into his breast in an effort to escape the vile wind, slipped quickly through the glass doors of Victory Mansions, though not quickly enough to prevent a swirl of gritty dust from entering along with him.
```

We have a heading, denoted using the `#` symbol, called "Chapter 1", followed by a paragraph of plain text. There are lots of other elements we can denote using Markdown, including things like lists, images, quotes, code listings, and so on. See the documentation for examples.

Note that there is no *stylistic* specification within a Markdown document. The codes denote semantic elements not stylistic elements. This is part of the philosophy of separating content from style. The idea is that one can take a semantically coded plain text Markdown document, and convert it into another format, such as HTML, or pdf, or a host of other formats, and along the way, specify a particular *style*---that is, a sort of translation of what each semantic element should look like.

If you've coded in HTML and used CSS files, this is the same idea.

The program we are going to use to perform this conversion is **Pandoc**.

# Pandoc

Pandoc is a program that can convert not just from Markdown to a host of other formats, but can convert from multiple formats to multiple formats. The [list of formats](http://pandoc.org) pandoc knows about is long.

Here are some resources for working with pandoc:

- [Getting started with pandoc](http://pandoc.org/getting-started.html)
- [Pandoc Demos](http://pandoc.org/demos.html)
- [Pandoc FAQs](http://pandoc.org/faqs.html)
- [Pandoc Manual](http://pandoc.org/MANUAL.html)
- [Pandoc crossref](https://github.com/lierdakil/pandoc-crossref) for
  numbering figures, equations, tables and cross-references to them
- [Pandoc citeproc](https://github.com/jgm/pandoc-citeproc) for
  citations & bibliographies
- [Citation Style Language (CSL) citation styles](https://github.com/citation-style-language/styles)

Let's take the sample Markdown document above (the opening paragraph of George Orwell's "Nineteen Eighty Four") and convert it, using pandoc, to another format.

First save the document in a plain text file, let's call it `1984.md`. Now let's convert it into HTML format using pandoc:

```
pandoc 1984.md -o 1984.html
```

The file we get looks like this:

```
<h1 id="chapter-1">Chapter 1</h1>
<p>It was a bright cold day in April, and the clocks were striking thirteen. Winston Smith, his chin nuzzled into his breast in an effort to escape the vile wind, slipped quickly through the glass doors of Victory Mansions, though not quickly enough to prevent a swirl of gritty dust from entering along with him.</p>
```

What you can see is that pandoc has basically translated the Markdown semantic codes into the corresponding HTML codes. In fact if you double-click on the `1984.html` file, and open it in a web browser, it will render the html file for you in the browser:

![1984.html](images/1984.png)

This sample document isn't very interesting, at least it doesn't make use of very many Markdown features. Let's have a look at another example that's closer to what we might be doing as academic writers:

```
# Introduction

Experimental studies of human motor learning often make use of robotic devices to manipulate the mechanics of human limb motion. The idea is to change the relationship between muscle forces and limb motion by using the robot to apply motion-dependent forces to the limb. The muscle forces that usually result in a given motion of the limb (e.g. reaching with the hand in a straight line between two targets) now result in a different motion, because of the added forces imposed by the robot. Through *motor learning*, the nervous system learns to generate new muscle forces to counteract the forces imposed by the robot.

In one such study,
```


# LaTeX

- [LaTeX Font Catalogue](http://www.tug.dk/FontCatalogue/)

# Markdown vs LaTeX

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









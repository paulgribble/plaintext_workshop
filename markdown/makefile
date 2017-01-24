
OPTIONS =  --latex-engine=xelatex \
	  -F pandoc-crossref \
	  -F pandoc-citeproc

ms.pdf:	ms.md
	pandoc ms.md -o ms.pdf $(OPTIONS)

ms_custom.pdf:	ms.md custom.latex
	pandoc ms.md -o ms_custom.pdf $(OPTIONS) --template custom.latex

all:	ms.pdf ms_custom.pdf

clean:
	rm -fr ms.pdf ms_custom.pdf


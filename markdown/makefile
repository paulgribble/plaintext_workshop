
OPTIONS =  --latex-engine=xelatex \
	  -F pandoc-crossref \
	  -F pandoc-citeproc \
	  --template mylatex.template

ms.pdf:	ms.md
	pandoc ms.md -o ms.pdf $(OPTIONS)

clean:
	rm -fr ms.pdf


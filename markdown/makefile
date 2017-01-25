
OPTIONS =  --latex-engine=xelatex \
	  -F pandoc-crossref \
	  -F pandoc-citeproc

ms.pdf:	ms.md
	pandoc ms.md -o ms.pdf $(OPTIONS)

clean:
	rm -fr ms.pdf


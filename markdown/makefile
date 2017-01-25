
OPTIONS =  --latex-engine=xelatex \
	  -F pandoc-crossref \
	  -F pandoc-citeproc

FIGURES = figures/robot.png \
	figures/experiment.png \
	figures/FC1.png \
	figures/FC2.png

ms:	ms.md formatting.yaml formatting.tex $(FIGURES)
	pandoc ms.md -o ms.pdf formatting.yaml -H formatting.tex $(OPTIONS)

ms_docx:	ms.md $(FIGURES) formatting.yaml
	pandoc ms.md -o ms.docx formatting.yaml $(OPTIONS)	

ms_plain:	ms.md $(FIGURES)
	pandoc ms.md -o ms_plain.pdf $(OPTIONS)

all:	ms ms_docx ms_plain

clean:
	rm -fr ms.pdf ms_plain.pdf ms.docx


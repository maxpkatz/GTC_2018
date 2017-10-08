ALL: abstract.pdf

PNGS := $(wildcard *.png)
PDFS := $(filter-out abstract.pdf,$(wildcard *.pdf))

abstract.pdf: abstract.tex refs.bib $(PNGS) $(PDFS)
	pdflatex abstract
	bibtex abstract
	pdflatex abstract
	pdflatex abstract
	pdflatex abstract


clean:
	rm -f abstract.aux abstract.log abstract.bbl abstract.blg abstract.pdf abstract.brf abstract.out abstractNotes.bib


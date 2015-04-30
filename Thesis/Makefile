
CHAPTERS=thesis_*.tex
FILES=$(CHAPTERS) thesis.tex

thesis.pdf: $(FILES)
	pdflatex thesis.tex
	bibtex thesis.aux
	pdflatex thesis.tex
	pdflatex thesis.tex

thesisclean: $(FILES) thesis.pdf
	rm -f *~ *.aux *.log *.lot *.lof *.toc *.bbl *.blg *.out

clean:
	rm -f *~ *.aux thesis.pdf *.out *.log *.lot *.lof *.toc *.bbl *.blg *.out

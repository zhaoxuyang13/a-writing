TEX_FILES := $(shell find . -name '*.tex')

all: slides.pdf

slides.pdf: $(TEX_FILES)
	TEXINPUTS=${TEXINPUTS}:./sty pdflatex slides

clean:
	-rm *.fdb_latexmk *.fls *.synctex.gz *.pdf *.aux *.log *.bbl *.blg *.out *.nav *.snm *.toc 2>/dev/null || true

.PHONY: clean all

### Makefile ends here

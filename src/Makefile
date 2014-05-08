OUTDIR := out
SOURCES := $(shell ls *.tex)
OUT := $(patsubst ,,$(SOURCES:.tex=.pdf))

main: ${OUT}

%.pdf: %.tex
	latexmk -pdf --output-directory=${OUTDIR} -auxdir=${OUTDIR} $<

clean:
	$(RM) -r out/*

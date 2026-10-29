# Build the CV and copy it to where the website links to it.
# Usage (from this folder): make

OUT = ../assets/pdfs/CV_JoseCristi.pdf

all:
	latexmk -pdf -outdir=build -interaction=nonstopmode -halt-on-error main.tex
	cp build/main.pdf $(OUT)

clean:
	latexmk -C -outdir=build main.tex
	rm -rf build

.PHONY: all clean

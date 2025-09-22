PDF_ENGINE = --pdf-engine=xelatex 
OPTIONS = --number-sections
BIB_OPTIONS = --citeproc

all: report.docx report.pdf

report.docx: report.md
	pandoc report.md -o report.docx $(OPTIONS) $(BIB_OPTIONS)

report.pdf: report.md
	pandoc report.md -o report.pdf $(PDF_ENGINE) $(OPTIONS) $(BIB_OPTIONS)

clean:
	rm -f report.docx report.pdf

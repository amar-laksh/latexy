TEX = pandoc
src = template.tex details.yml
FLAGS = --pdf-engine=xelatex

Amar_Lakshya.pdf : $(src)
	$(TEX) $(filter-out $<,$^ ) -o $@ --template=$< $(FLAGS)

.PHONY: clean
clean :
	rm *.aux *.log *.pdf *.spl *.gz *.fls *.fdb_latexmk *.bbl *.blg

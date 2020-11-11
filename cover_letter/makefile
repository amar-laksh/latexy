TEX = pandoc
src = template.tex details.yml
cyber_src = template.tex details_cyber.yml
FLAGS = --pdf-engine=xelatex

Amar_Lakshya_Cover_Letter.pdf : $(src)
	$(TEX) $(filter-out $<,$^ ) -o $@ --template=$< $(FLAGS)


cyber : $(cyber_src)
	$(TEX) $(filter-out $<,$^ ) -o Amar_Lakshya_Cover_Letter.pdf --template=$< $(FLAGS)

.PHONY: clean
clean :
	rm *.aux *.log *.pdf *.spl *.gz *.fls *.fdb_latexmk *.bbl *.blg

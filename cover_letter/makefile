TEX = pandoc
src = template.tex details.yml
FLAGS = --pdf-engine=xelatex

Amar_Lakshya_cover_letter.pdf : $(src)
	$(TEX) $(filter-out $<,$^ ) -o $@ --template=$< $(FLAGS)

.PHONY: clean
clean :
	rm Amar_lakshya.pdf

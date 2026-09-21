TARGET = resumen

all: $(TARGET).pdf

$(TARGET).pdf: $(TARGET).tex
	latexmk -pdf -interaction=nonstopmode $(TARGET).tex

clean:
	latexmk -c
	rm -f *.aux *.log *.toc *.fls *.fdb_latexmk *.out

clean-all: clean
	rm -f $(TARGET).pdf

.PHONY: all clean clean-all

# name of the paper, without extension
TEXFILE = paper

# make PDF
$(TEXFILE).pdf: $(TEXFILE).tex
	latexmk -pdf -quiet $(TEXFILE)
	
# remove auxiliary files	
clean: 
	rm -f $(TEXFILE).pdf
	rm -f $(TEXFILE).log
	rm -f $(TEXFILE).out
	rm -f $(TEXFILE).fls
	rm -f $(TEXFILE).aux
	rm -f $(TEXFILE).fdb*

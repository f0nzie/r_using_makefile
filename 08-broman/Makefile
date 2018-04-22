# http://kbroman.org/minimal_make/

# put the figure in Figs
Figs/fig1.pdf: R/fig1.R
	cd R; \
	R CMD BATCH fig1.R
	
# remove files	
clean :
	rm -f Figs/fig1.pdf
	rm -f R/fig1.Rout
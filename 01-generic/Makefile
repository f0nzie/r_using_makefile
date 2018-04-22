# this Makefile will work for any notebook by using patterns
%.html : %.Rmd
	Rscript -e 'rmarkdown::render("$<")'

# The all rule is the first rule in the Makefile, so it is the default rule 
# that is run when you type make

# list the the output files
all : generic.html iris.html
	@echo All files are now up to date
	
clean : 
	rm -f generic.nb.html iris.nb.html

# build the files that were given
%.html : %.Rmd
	Rscript -e 'rmarkdown::render("$<")'
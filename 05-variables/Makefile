# a variable with a list the the output files
HTML := generic.html iris.html


all : $(HTML)
	echo All files are now up to date
	
clean : 
	rm -f *.nb.html

# build the files that were given
%.html : %.Rmd
	Rscript -e 'rmarkdown::render("$<")'
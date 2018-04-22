# we start by processing only one file
# this will build the md out of the Rmd
# Run it with "make", or
# "make simple.html"
simple.html : clean simple.Rmd
	Rscript -e 'rmarkdown::render("simple.Rmd")'
	
# remove the files created during the build	
clean :
	rm -f simple.nb.html
	rm -rf simple_files

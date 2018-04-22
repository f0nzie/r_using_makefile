# this Makefile will work for any notebook by using patterns

# clean and call "rmds"
all : clean rmds

# files we want
rmds : generic.html iris.html

# build html files (targets) from Rmd (dependencies)
%.html : %.Rmd
	Rscript -e 'rmarkdown::render("$<")'


clean :
	rm -f *.html
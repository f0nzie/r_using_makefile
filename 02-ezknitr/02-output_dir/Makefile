# this Makefile will work for any notebook by using patterns

# clean and call "rmds"
all : rmds

# files we want
rmds : generic.md iris.md

# build html files (targets) from Rmd (dependencies)
%.md : %.Rmd
	# Rscript -e 'rmarkdown::render("$<")'
	R --slave -e	"ezknitr::ezknit('$<', \
					fig_dir = 'figures', \
					out_dir = 'output' \
					)"


clean :
	rm -f output/*.html
	rm -f output/*.md
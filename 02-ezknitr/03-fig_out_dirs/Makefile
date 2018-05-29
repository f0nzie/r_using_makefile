# this Makefile will work for any notebook by using patterns

# clean and call "rmds"
all : rmds

# files we want
rmds : generic.md iris.md

# build html files (targets) from Rmd (dependencies)
# a folder for figures under output
%.md : %.Rmd
	R --slave -e	"ezknitr::ezknit('$<', \
					fig_dir = './figures/$*/', \
					out_dir = 'output' \
					)"


clean :
	rm -f output/*.html
	rm -f output/*.md
	rm -rf output/generic
	rm -rf output/figures
	rm -rf output/iris
	rm -rf generic
	rm -rf iris
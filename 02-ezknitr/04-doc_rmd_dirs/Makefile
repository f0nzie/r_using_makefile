
# clean and call "rmds"
all : mds

mds : generic.md iris.md


# build html files (targets) from Rmd (dependencies)
# a folder for figures under output
%.md : doc/RMD/%.Rmd
	R --slave -e	"ezknitr::ezknit('$<', \
					fig_dir = './figures/$*/', \
					out_dir = '$(@D)')"


clean :
	rm -f output/*.html
	rm -f output/*.md
	rm -rf output/generic
	rm -rf output/figures
	rm -rf output/iris
	rm -rf generic
	rm -rf iris
	rm -f *.html
	rm -f *.md
# the template files
templates := $(shell find ../ -depth 1 -type f -name "*.tex")

# the tex files in this directory (and any below)
tex := $(shell find . -type f -name "*.tex")

# the resources (js, php, eps, etc.)
source := $(shell find ./resources -type f)

# build notes.pdf whenever any of the above have changed
# make sure to use a tab (not spaces) for the commands below
notes.pdf: $(templates) $(tex) $(source)
	# build using xelatex
	xelatex --halt-on-error --shell-escape notes.tex

	# open preview in the background
	open -g notes.pdf

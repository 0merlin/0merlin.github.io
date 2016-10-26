MD_FILES := $(wildcard *.md)
HTML_FILES := $(MD_FILES:.md=.html)
INFO_MD_FILES := $(wildcard info/*.md)
INFO_HTML_FILES := $(INFO_MD_FILES:.md=.html)
TUTORIALS_MD_FILES := $(wildcard tutorial/*.md)
TUTORIALS_HTML_FILES := $(TUTORIALS_MD_FILES:.md=.html)
APPS_MD_FILES := $(wildcard apps/*.md)
APPS_HTML_FILES := $(APPS_MD_FILES:.md=.html)
ARGS = -s --toc -f markdown --highlight-style zenburn
TEMPLATE = --template templates/template.html
STRIP = sed -e 's/^[ \t]*//' | sed '/^$$/d'

all: output $(HTML_FILES) $(INFO_HTML_FILES) $(TUTORIALS_HTML_FILES) $(APPS_HTML_FILES)

output:
	mkdir -p ../info ../tutorial ../apps

%.html: %.md
	pandoc $(ARGS) $(TEMPLATE) $< > ../$@

*/%.html: %.md
	pandoc $(ARGS) $(TEMPLATE) $< > ../$@

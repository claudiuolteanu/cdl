TEXFILES = header.tex kr1.tex kr2.tex kr3.tex gnu.tex j1.tex dox.tex dox2.tex dox3.tex sfat1.tex sfat2.tex functii.tex bugs.tex bugs_nice.tex
HIGHLIGHT_OPTS = -L -f -t 8 -c highlight.sty

all: $(TEXFILES)

header.tex: header.c
	highlight $(HIGHLIGHT_OPTS) -i $< -o $@

bugs.tex: bugs.c
	highlight $(HIGHLIGHT_OPTS) -i $< -o $@ --font-size=footnotesize -l

bugs_nice.tex: bugs_nice.c
	highlight $(HIGHLIGHT_OPTS) -i $< -o $@ --font-size=scriptsize -l

functii.tex: functii.c
	highlight $(HIGHLIGHT_OPTS) -i $< -o $@

sfat1.tex: sfat1.c
	highlight $(HIGHLIGHT_OPTS) -i $< -o $@ --font-size=small

sfat2.tex: sfat2.c
	highlight $(HIGHLIGHT_OPTS) -i $< -o $@ --font-size=small

kr1.tex: kr1.c
	highlight $(HIGHLIGHT_OPTS) -i $< -o $@ --font-size=small

kr2.tex: kr2.c
	highlight $(HIGHLIGHT_OPTS) -i $< -o $@ --font-size=small

kr3.tex: kr3.c
	highlight $(HIGHLIGHT_OPTS) -i $< -o $@ --font-size=small

gnu.tex: gnu.c
	highlight $(HIGHLIGHT_OPTS) -i $< -o $@ --font-size=footnotesize -l

j1.tex: j1.java
	highlight $(HIGHLIGHT_OPTS) -i $< -o $@ --font-size=footnotesize -l

dox.tex: dox.cpp
	highlight $(HIGHLIGHT_OPTS) -i $< -o $@ --font-size=footnotesize -l

dox2.tex: dox2.cpp
	highlight $(HIGHLIGHT_OPTS) -i $< -o $@ --font-size=footnotesize -l

dox3.tex: dox3.cpp
	highlight $(HIGHLIGHT_OPTS) -i $< -o $@ --font-size=footnotesize -l

.PHONY: clean
clean:
	rm -f $(TEXFILES) highlight.sty

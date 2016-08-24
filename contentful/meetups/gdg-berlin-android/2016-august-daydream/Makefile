RSTS = $(wildcard *.rst)
HTMLS = $(patsubst %.rst,%-html,$(RSTS))


all : $(HTMLS)

%-html: %.rst
	hovercraft $^ $@

debug : $(RSTS)
	watch -n 2 hovercraft $^

%-html: %.rst
	hovercraft -t ../../../../talk-template $^ $@

clean:
	rm -rf $(HTMLS)
	
slides: all
	decktape -s 1920x1080 "${PWD}/*-html/index.html" "${PWD}/slides.pdf"


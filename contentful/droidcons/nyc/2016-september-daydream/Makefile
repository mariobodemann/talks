RSTS = $(wildcard *.rst)
HTMLS = $(patsubst %.rst,%-html,$(RSTS))


all : $(HTMLS)

debug : $(RSTS)
	watch -n 5 make

%-html: %.rst
	hovercraft -t ../../../../talk-template $^ $@

clean:
	rm -rf $(HTMLS)
	
slides: all
	cp *-html/daydream.css *-html/daydream.css.bk
	cat *-html/daydream-slides.css >> *-html/daydream.css
	decktape -s 1920x1080 "${PWD}/*-html/index.html" "${PWD}/slides.pdf"
	mv *-html/daydream.css.bk *-html/daydream.css

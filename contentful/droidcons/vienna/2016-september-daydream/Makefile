RSTS = $(wildcard *.rst)
HTMLS = $(patsubst %.rst,%-html,$(RSTS))


all : $(HTMLS)

%-html: %.rst
	hovercraft $^ $@

debug : $(RSTS)
	watch -n 5 make

%-html: %.rst
	hovercraft -t ../../../../talk-template $^ $@

clean:
	rm -rf $(HTMLS)
	
slides: all
	cp daydream.css daydream.css.bk
	cat daydream-slides.css >> daydream.css
	decktape -s 1920x1080 "${PWD}/*-html/index.html" "${PWD}/slides.pdf"
	mv daydream.css.bk daydream.css

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
	cat daydream-slides.css >> daydream-html/daydream.css
	decktape -s 1920x1080 "${PWD}/daydream-html/index.html" "${PWD}/slides.pdf"

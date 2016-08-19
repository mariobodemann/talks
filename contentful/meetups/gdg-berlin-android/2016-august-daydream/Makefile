RSTS = $(wildcard *.rst)
HTMLS = $(patsubst %.rst,%-html,$(RSTS))


all : $(HTMLS)

%-html: %.rst
	hovercraft $^ $@

debug : $(RSTS)
	watch -n 2 hovercraft $^

%-html: %.rst
	hovercraft $^ $@

clean:
	rm -rf $(HTMLS)
	
slides: 
	deck2pdf --profile=impressjs *-html/index.html slides.pdf


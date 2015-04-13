RSTS = $(wildcard *.rst)
HTMLS = $(patsubst %.rst,%-html,$(RSTS))


all : $(HTMLS)

%-html: %.rst
	hovercraft $^ $@

clean:
	rm -rf $(HTMLS)
	

# you need pdflatex ..
#

pdflatex=pdflatex
flyerlist=$(wildcard flyer_*tex)


pdfflyer :
	@echo 'starts pdflatex for all flyer_ files ...'
	@for file in $(flyerlist); do \
		$(pdflatex) $$file > make.log; \
		echo $$file "done."; \
	done

clean :
	rm -f $(wildcard *.aux)	$(wildcard *.log) $(wildcard *.toc)


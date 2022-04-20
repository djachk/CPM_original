SHELL = /bin/sh

tar:
	make clean
	cd lib ; make clean
	cd examples ; make clean
	cd examples ; rm -rf Frames
	d=`basename \`pwd\`` ;\
	cd ..; rm -f $$d.tar* ;\
	tar cvf $$d.tar $$d 

manual:
	latex manual ; latex manual
	pdflatex manual

clean:
	rm -f manual.aux manual.toc manual.dvi manual.log

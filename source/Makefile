all: 
	#clean
	$(MAKE) spanish
	$(MAKE) english
	#pdftoppm cv-en.pdf cv -png -rx 300 -ry 300
	
spanish: 
	#clean
	pdflatex main.tex
	mv cv-es.pdf
	#$(MAKE) clean

english: 
	#clean
	pdflatex "\def\inenglish{1} \input{main.tex}"
	mv cv-en.pdf
	#$(MAKE) clean

clean:
	rm -rf *.aux *.log *.out

cleanclean: clean
	rm -rf *.pdf
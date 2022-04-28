clean:
	rm -f $$(ls *.* | grep -v '\.pdf\|\.tex\|\.md\|\.bib\|\.png')
	rm -rf auto

squeaky:
	make clean
	rm -f *.pdf

paper:
	make clean
	pdflatex paper_chequeDishonour.tex
	pdflatex paper_chequeDishonour.tex
	pdflatex paper_chequeDishonour.tex
	makeglossaries paper_chequeDishonour
	pdflatex paper_chequeDishonour.tex
	pdflatex paper_chequeDishonour.tex
	biber paper_chequeDishonour
	pdflatex paper_chequeDishonour.tex
	pdflatex paper_chequeDishonour.tex
	pdflatex paper_chequeDishonour.tex
	make clean

brief:
	make clean
	pdflatex policyBrief.tex
	pdflatex policyBrief.tex
	pdflatex policyBrief.tex
	makeglossaries policyBrief
	pdflatex policyBrief.tex
	pdflatex policyBrief.tex
	biber policyBrief
	pdflatex policyBrief.tex
	pdflatex policyBrief.tex
	pdflatex policyBrief.tex
	make clean

slides:
	make clean
	pdflatex sl_NIAct.tex
	pdflatex sl_NIAct.tex
	pdflatex sl_NIAct.tex
	biber sl_NIAct
	pdflatex sl_NIAct.tex
	pdflatex sl_NIAct.tex
	pdflatex sl_NIAct.tex
	make clean

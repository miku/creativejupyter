Example.pdf: Example.ipynb
	jupyter nbconvert --to=pdf --template=./revtex.tplx Example.ipynb

.PHONY: clean
clean:
	rm -rf Example_files/
	rm -rf Example.slides.html
	rm -rf Example.pdf
	rm -rf Example.tex


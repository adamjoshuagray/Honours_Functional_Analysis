READ = evince
NAME = Assignment
COMP = pdflatex


$(NAME).pdf: $(NAME).tex unswmaths.cls
	$(COMP) $^
	
read: $(NAME).pdf
	$(READ) $^ &

clean:
	rm -f *.aux *.log *~
	

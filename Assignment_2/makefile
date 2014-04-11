READ = evince
NAME = Assignment
COMP = pdflatex
CLASS = unswmaths.cls

$(NAME).pdf: $(NAME).tex $(CLASS)
	$(COMP) $^

read: $(NAME).pdf
	$(READ) $^ &

clean:
	rm -f *.aux *.log *~ *.save $(NAME).pdf *.bak

spell:
	ispell $(NAME).tex

class_update:
	cd ..; \
	git submodule update --init --recursive; \
	cd -; \
	cp -r ../UNSW_Latex/artwork artwork; \
	cp -r ../UNSW_Latex/unswmaths.cls unswmaths.cls	


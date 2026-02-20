all: estados.png gestion.png liquidacion.png subasta.png

%.png: %.uml
	plantuml $<

clean:
	rm -f *.png

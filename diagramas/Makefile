all: estados.png negocios.png liquidacion.png subasta.png

%.png: %.uml
	plantuml $<

clean:
	rm -f *.png

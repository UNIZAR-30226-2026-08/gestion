PLANTUML_JAR := $(firstword $(wildcard plantuml*.jar))

ifneq ($(PLANTUML_JAR),)
    PLANTUML_CMD := java -jar $(PLANTUML_JAR)
else
    PLANTUML_CMD := plantuml
endif

SRCS := $(wildcard *.uml)
OBJS := $(SRCS:.uml=.png)

all: $(OBJS)

%.png: %.uml
	$(PLANTUML_CMD) --format latex $<

clean:
	rm -f *.png *.tex

.PHONY: all clean

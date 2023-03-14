# el target all permite ejecutar multiples targets

all: one two three f1.o f2.o

one:
	touch one
two:
	touch two
three:
	touch three
clean:
	rm one two three

##multiples targets, cada comando se ejecuta en cada target
## la variable automatica $@ hace referencia al target en ejecucion

f1.o f2.o:
	echo $@

#las variables automaticas son variables que devuelven informacion contextual como los target o prerequisites

hey: one two
	echo $@ #imprime el target
	echo $? #imprime los prerequisites mas nuevos que el target
	echo $^ #imprime todos los prerequisites
	touch hey
one:
	touch one
two:
	touch two
clean:
	rm hey one two

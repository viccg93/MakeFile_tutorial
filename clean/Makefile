#clean puede ser usado como un target, por que no es una palabra reservada
#clean debe ser usada como target y no como filename
#generalmente se usa para limpiar la salida de otros targets
#si un target no existe como filename siempre se ejecutara

#aunque some_file existe despues de la primera ejecucion
#la dependencia con other_file, hace que siempre se ejecute
some_file: other_file
	echo "esta regla siempre corre y es la segunda"
	touch some_file
other_file:
	echo "esta regla siempre corre y es la primera"
clean:
	rm some_file

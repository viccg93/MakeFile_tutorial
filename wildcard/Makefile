#* y % son wildcard, pero funcionan de distinta manera
# * busca en el filesystem nombres que coincidan, siempre se debe usar con la funcion wildcard
# $(wildcard *.c)
# * no deb ser usado directamente en variables, ya que en ese caso se pasa la cadena y no el result de la exp

all: print one two three four

print: $(wildcard *.c)
	ls -la $?

right_assignation := $(wildcard *.o)
wrong_assignation := *.o

#falla porque pasa la cadena *.o y no la evaluacion
one: $(wrong_assignation)

#funciona, pero se queda como cadena '*.o' si no hay matches
two: *.o

#funciona y no devuelve hace nada si no hay matches, por lo que es el comportamiento deseado
three: $(right_assignation)

#igual que three, pero sin variable

four: $(wildcard *)


#el wildcard % es muy util, pero es algo confuso ya que cuenta con 2 modos
#matching mode, donde hace match con uno o mas caracteres de una cadena y a esos caracteres
#se les conoce como stem
#y replacing mode, donde toma los caracteres del stem y los remplaza por otra cadena

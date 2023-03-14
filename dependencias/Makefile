
#esta regla se ha agregado como extra, ejecuta el programa
saludoRun: saludo
	./saludo
#esta regla se llama primero(en orden de aparicion), pero solo se ejecuta si existe saludo.o
#en caso contrario llama al target saludo.o
saludo: saludo.o
	cc saludo.o -o saludo
#este target es dependecia de saludo y genere el archivo .o desde el
#codigo fuente saludo.c, por lo que depende de saludo.c,
#si no existe ejecuta el target saludo.c
saludo.o: saludo.c
	cc -c saludo.c -o saludo.o
#este target es el ultimo en ser llamado, pero el primero en ejecutarse
#cuando no existe el archivo saludo.c, no se pueden ejecutar saludo y saludo.o
#ya que ambos dependen de saludo.c
saludo.c:
	echo "#include<stdio.h>" > saludo.c
	echo "int main(){printf(\"Hola mundo\");}" >> saludo.c

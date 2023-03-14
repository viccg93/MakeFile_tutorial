#las variables solo pueden almacenar cadenas y se asignan con :=, aunque = es valido
archivos := file1 file2
some_file: $(archivos)
	echo "Variable archivos: " $(archivos)
	touch some_file
#genera archivo file1
file1:
	touch file1
#genera archivo file2
file2:
	touch file2
#elimina todos los archivos
clean:
	rm -r file1 file2 some_file

#las comillas (single o double) no tienen importancia para make, pero si para bash
#las referencias se deben hacer con $(var) o ${var}, $var funciona pero es considerado mala practica

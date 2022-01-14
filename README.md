# ejercicio_1104.sh

Escriba un script que, para un archivo CSV y un número de columna determinados, imprima:

**el nombre de la columna correspondiente**

Primero se necesita extraer el nombre de la columna, por ejemplo si se toma en cuenta la columna 7, se usa:

$ cut -d ',' -f 7 Buzzard2015_data.csv | head -n 1

Se obtiene: 

biomass

**el número de valores distintos en la columna**

En segundo lugar, para obtener el número de valores distintos podemos ordenar los resultados (eliminando *head*) y usar *uniq*

cut -d ',' -f 7 Buzzard2015_data.csv | tail -n +2 | sort | uniq | wc -l       

Se obtiene:

285


**el valor mínimo**

Para obtener el valor min e utilizó el siguiente código *sort -n* 

**el valor máximo**

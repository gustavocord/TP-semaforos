# Trabajo practico de Sistemas Operativos y redes - Hilos y semaforos
Alumno: Gustavo Cordoba

-En la cocina de Hell’s Burgers compiten tres equipos de cocineros. ¿Quién será el primero en entregar la hamburguesa ? La dificultad de la competencia es que la cocina no cuenta con el equipamiento individual para cada equipo, sino que algunos de ellos son compartidos. Se tienen que ordenar para cocinar los medallones ya que solo tienen una plancha para todos los equipos y esta cocina un medallón a la vez, existe solo un horno que cocina dos panes a la vez y un solo salero.-

## implementaciones

* los equipos (hilos) comienzan en el mismo momento y realizando las tareas de manera recurrente
* Los equipos no pueden utilizar los recursos compartidos al mismo tiempo (horno, salero, plancha)
* El orden de la receta es lla misma para todos los equipos
* El archivo receta.txt contiene la receta y cada linea es una accion
* El archivo resultado.txt contiene el resultado y un log de lo que sucedio en la competencia como quien gano y la accion de cada equipo en tiempo real


## Procedimiento 
 Inicialmente se definierom  los mutex y los semaforos compartidas junto con una variable que indicara el puesto de cada equipo al finalizar la ejecucion .
 Hilos y Semaforos : Para cada hilo se implementaron 8 semaforos individuales para las acciones que requieren compartir equipamiento .
 Ademas se utilizaron 3 mutex  para las acciones que requieren compartir equipamiento  

## Dificultades
_ El trabajo requirio mucha investigacion en si y se dificulto bastante ya que no es un lenguaje en el que este acostumbrado a programar dado esto me llevo mas tiempo del que estimaba . Uno de los obstaculos fue leer el archivo de texto y luego escribir el resultado de la competencia en otro archivo pero esto pude resolver gracias a la investigacion que hacia en internet y consultando con mis compañeros.



### Ejecución :man_technologist:	

```
Compilar:   gcc Hamburguesa.c -o ejecutable -lpthread
Ejecutar:   ./ejecutable
```


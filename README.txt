﻿@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@
@  Comentarios Iteración 2/ Changelog --         @
@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@

El proyecto ha sido completamente rediseñado.

1- El partido incluye los equipos, una lista de resultados y la lista de contenedores de apuesta.
2- Como se deduce de lo anterior, se ha empleado un contenedor de apuesta, que contendrá todas las apuestas de cierta modalidad, y que tendrá un atributo booleano para saber si se ha pagado el contenedor o no.
3- Se ha optado por retransmitir sucesivamente la excepción de cuentas de un método al superior que le invoca, en el método que lo requiere, y por ello hemos añadido un catch de la excepción en el main.
4- Puesto que se ha añadido la comprobación para que tengan que pasar 2 horas desde el cierre de apuestas del partido para poder fijar el resultado, SERÁ NECESARIO descomentar la línea indicada del método setResultadoPartido() para que la salida indicada en el .java de prueba sea la del proyecto.
5- Las constantes (en este caso, sólo una) se incluyen en un archivo config.properties en la carpeta src, aunque sería más adecuado ubicarlo en una carpeta separada (resources), se ha ubicado aquí para evitar perder el archivo. Se utiliza un try/catch para la IO Exception (excepción en la entrada/salida) y si no se encuentra el archivo, se imprime el rastro que ha dejado la excepción mediante printStacktrace().

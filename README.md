# ADVENT_OF_CODE_2025
//DAY 1 - PROBLEMA 2 
Igual que en la primera parte del día 1, elegimos este problema para más tarde comprobar nuestra mejora una vez finalizado el evento.
Debido a que la segunda parte del día es una modificación del primero, las técnicas usadas son las mismas.
Para abordar el problema, en vez de crear condiciones dentro de condiciones para todas las funciones que usamos en la primera parte, decidimos "comprimir" las funciones dedicadas a lo que ocurría cuando la posición bajaba de 0 o superaba el 99 y transformarlas en condiciones dentro de las funciones dedicadas a girar a la izquierda o a la derecha. Una vez hecho esto, solo hizo falta cambiar las condiciones del contador, que ahora aumentará cada vez que la posición se vaya de rango y se tenga que ajustar. 
La única otra alternativa que planteamos fue añadir al código original en vez de quitar y transformar funciones, pero nos dimos cuenta de que no era nada eficiente y había una manera mucho más rápida y limpia de obtener la solución.
Con este ejercicio hemos aprendido que lo que puede parecer un ligero cambio puede alterar por completo la lógica detrás de tu código, obligándote a darle otra vuelta y tener que cambiar la estructura anterior. 

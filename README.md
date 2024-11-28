# Tp-Estructura-de-datos
Juego Dragon Ball

Implementación de una cola de prioridades para gestionar combates:

Objetivo: Crear una cola de prioridades donde los personajes con mayor nivel de poder tengan prioridad en los enfrentamientos. Esto es útil para organizar torneos donde los personajes más fuertes combaten primero o se enfrentan en rondas avanzadas.

Conceptos clave: 
1.	Cola de Prioridades:

o	Es una estructura de datos donde cada elemento tiene una prioridad asociada.

o	Los elementos con mayor prioridad se procesan antes que los de menor prioridad.

o	En este caso, la prioridad será el nivel de poder del personaje.

2.	Heap Binaria:

o	Se utiliza para implementar eficientemente una cola de prioridades.

o	Un Max-Heap es un árbol binario donde el valor de cada nodo es mayor o igual al de sus hijos. El nodo raíz contiene el valor máximo (en este caso, el personaje más fuerte).

Explicación de la estructura:

•	Importar heapq: Python proporciona el módulo heapq para gestionar heaps.

•	Negar la prioridad: Dado que heapq implementa un Min-Heap por defecto (prioriza valores menores), negamos el nivel de poder para simular un Max-Heap.

•	Inserción: Se usa heapq. heappush para insertar un personaje con su nivel de poder negado.
•	Extracción: heapq. heappop elimina y devuelve el personaje con mayor prioridad.

Puntos clave: 

•	Inserción en O(log n): La operación de insertar en un heap binario es eficiente, incluso con un gran número de personajes.

•	Extracción en O(log n): Obtener el personaje más fuerte (prioridad máxima) también es eficiente.

•	Orden de Enfrentamientos: La estructura garantiza que los personajes más fuertes combatan primero.

Aplicación en torneos: 

•	Rondas de Combate: Se puede usar la cola de prioridades para organizar rondas donde los personajes más fuertes se enfrentan primero o avanzan más rápidamente.

•	 Simulación de Batallas: Después de cada combate, el ganador podría volver a insertarse con un nivel de poder ajustado (por ejemplo, aumentado por experiencia de combate).


Conclusion:
Luego de finalizar todas las partes  del proyecto y crear un juego basado en el universo de Dragon Ball, llegamos a la conclusión de que, para desarrollar un sistema eficaz y funcional, es importante elegir las estructuras de datos adecuadas para cada segmento del juego. Estas estructuras nos ayudan en la organización de la información y la optimización de las operaciones que requerimos. Para organizar el juego, utilizamos clases para ilustrar a los personajes y sus habilidades de forma más precisa y organizada. Esto simplificó la elaboración de combates y la evolución de los personajes, haciendo el código más estructurado y sencillo. Además, aplicamos árboles binarios para organizar a los personajes de acuerdo a su grado de poder. Esto nos facilito la ejecución de búsquedas e inserciones rápidas, lo que nos ayuda para detectar a los jugadores más poderosos de manera mas rapida. Además, empleamos grafos para recrear los viajes entre planetas, lo que incorporó una dimensión adicional de exploración al juego. Respecto a los enfrentamientos, empleamos una cola de prioridad para garantizar que los personajes con mayor fuerza intervengan primero, lo que convierte las peleas en más estratégicas. En cambio, utilizamos el ordenamiento topológico para desbloquear las capacidades de los personajes en la secuencia adecuada, siguiendo un camino lógico que replica el progreso del entrenamiento. Cada herramienta que usamos tuvo un objetivo, no solo mejorar el desempeño, sino también aportar a una experiencia de juego más fluida para cada jugador.  Este trabajo practico evidencia que las estructuras de datos son esenciales para convertir conceptos complejos en un juego práctico, estratégico y leal a la esencia de la saga Dragon Ball.

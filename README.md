# Producto-Unidad-3
# 1.	PLANTEAMIENTO DEL PROBLEMA
La electrónica digital ha marcado un gran avance en la tecnología durante los últimos 80 años. Es una rama de la electrónica que nos permite realizar circuitos lógicos a partir de las necesidades que se presenten en cualquier situación. Permitiéndonos aplicar dicho concepto para resolver o sustentar necesidades más avanzadas como el resolver operaciones aritméticas, multiplexar diferentes salidas o decodificar una serie de valores binarios (Lógica combinacional) y acoplarlo con unidades básicas de memoria, mediante su diseño haciendo el uso de diagramas y tablas de estado, convirtiéndolo así en circuitos lógicos secuenciales, que pueden ser de alta relevancia en la fundamentación acerca del funcionamiento de microprocesadores. 
En nuestro caso, justamente, realizaremos el diseño de circuitos lógicos utilizando los diagramas y tablas de estado para representar cada problema que se nos sea presentado. El propósito de este producto de unidad es analizar el funcionamiento de los circuitos lógicos combinacionales y secuenciales, haciendo énfasis en las aplicaciones que pueden tener en general y a su vez que puedan ser implementados (de ser necesario) a circuitos lógicos, en nuestro caso, a la operatividad de una máquina expendedora de bebidas y a un sistema de riego automático.
# 2.	OBJETIVOS
## 2.1.	OBJETIVO GENERAL
Diseñar diagramas de estado a partir de sus respectivas tablas y viceversa complementando su aplicación en una máquina expendedora de bebidas y en un sistema de riego automático, mediante el respectivo análisis de cada proceso que se lleve a cabo junto con su funcionalidad, con el fin de implementarlo en un circuito lógico. 

## 2.2.	OBJETIVOS ESPECÍFICOS
-	Investigar la funcionalidad y la composición de un circuito lógico secuencial, haciendo énfasis principalmente en las diferentes máquinas de estado que pueden aplicarse en el diseño de un circuito a partir de una problemática o necesidad, de tal manera que funcione de manera automática.
-	Buscar artículos relacionados a la problemática de resolver o diseñar diferentes circuitos, mediante el uso de diagramas y tablas de estado y comparar cuál es su relación con el proyecto a realizar en este producto de unidad.
-	Desarrollar el proceso en el que se realicen los grafos de estado junto con sus tablas de verdad, cuya fundamentación, en cuestión, esté relacionada con las diferentes máquinas de estado existentes.
# 3. ESTADO DEL ARTE
## Diseño del sistema de diagnóstico de fallas del paquete de baterías de litio basado en una máquina de estado de dos niveles.
En este documento se analiza el diseño de un sistema útil, que se utiliza para monitorear el estado del paquete de baterías de litio y diagnosticar su falla. Este sistema se implementó mediante la adopción creativa de una máquina de estado de dos niveles. Los fallos que puede producir el paquete de baterías de litio de potencia se utilizaron para definir el estado de la máquina de estados finitos. La máquina de estado de dos etapas se utilizó para registrar y reportar todo tipo de información de fallas, mientras que la máquina de estado de una etapa se utilizó para determinar la salida final del sistema. Este sistema se comunicaba con la PC a través de CAN y proporcionaba mucha información importante para el sistema de gestión de la batería. Los experimentos muestran que este sistema puede juzgar el tipo de falla y el nivel de falla de manera eficiente y precisa y también puede tomar medidas de protección a tiempo.

## Clasificación de regiones estáticas utilizando una máquina de estado finito jerárquica
En este artículo se nos presenta sobre la capacidad de la mayoría de los enfoques existentes para clasificar regiones estáticas, como objetos abandonados y retirados en imágenes, se ve afectada por la iluminación y el volumen de tráfico debido a varios valores de umbral predefinidos. Para reducir estos efectos, proponemos un método de clasificación de regiones estáticas preciso utilizando una máquina jerárquica de estados finitos que consta de tres capas. Cada FSM está definido por una máquina de estado de Mealy, donde una máquina de vectores de soporte (SVM) determina la transición de estado según el estado actual y las características de entrada. Debido a que el método propuesto utiliza clasificadores de SVM entrenados de manera óptima, no requiere valores de umbral y garantiza una mejor precisión de clasificación bajo cambios ambientales severos. 

## Implementación de transiciones de estados de animación en escenas interactivas basadas en una máquina gráfica de estados finitos
Este artículo habla sobre el uso de funciones gráficas para probar la máquina de estados finitos que conecta clips de movimiento y finalmente implementar la animación interactiva de personajes. Estos enfoques no solo facilitan la investigación de la reutilización de datos de animación y el autocontrol del movimiento de los personajes, sino que también llevan a cabo herramientas de transferencia gráfica de estados de caracteres que pueden probar e implementar la máquina de estados finitos de la animación interactiva.

# 4. MARCO TEÓRICO
## Máquina de estados
Un ‘estado’ es la condición de una cosa en un tiempo determinado. Algunos que pueden realizar tareas y que utilizan estados como su núcleo son máquinas de estado. También son conocidas como máquinas de estado finitas, lo que significa que sabemos todos los posibles estados de ella. La clave para la máquina de estado es el concepto del tiempo y la historia. El estado de la máquina es evaluada periódicamente. Cada vez que es evaluada, un nuevo estado es elegido (el que podría ser el mismo estado nuevamente) y el resultado es presentado.

## Una máquina de estado genérica:

 ![1](https://user-images.githubusercontent.com/66962449/93040932-d57efb80-f610-11ea-88b5-569ee8458422.jpg)
 
Un diagrama de una máquina de estado genérica. El elemento de memoria  contiene el nuevo estado conocido como el estado variable. Cuando la máquina de estado cuenta con los servicios, el estado variable es actualizado con el valor de la próxima etapa. Acá lanueva etapa es una función de ambos; el estado actual y algunos inputs. La nube de la lógica es un sistema que decide cual será el próximo estado, o la próxima lógica de estado. 

## Una máquina de estado simple: El contador.

Un clásico ejemplo de una máquina de estado es un contador. Por ejemplo, un ‘for loop’ o un circuito integrado lógico de 74×4040 trabajan como una máquina de estado. Cada vez que la máquina cambia de estado, ya sea por la línea del reloj o por el comportamiento de bucle, el estado de la memoria cambia a un nuevo estado igualando el estado anterior más uno. El set finito de estados que puede tener es la cantidad de números que puede contar.
 
 ![2](https://user-images.githubusercontent.com/66962449/93040937-d9128280-f610-11ea-945b-d2b37d6fbcbf.jpg)
 
Un contador básico expresado como máquina de estado
Partes de la máquina de estado del contador:
•	El estado actual es el valor que ha sido contado.
•	El resultado es el estado actual.
•	La próxima etapa lógica es lo que sea el estado actual + 1.
•	No hay entradas. En un diagrama más avanzado, una entrada o una función de reseteo del contador será establecido como entrada.
La máquina de estado avanza a cualquier ritmo que sea atendida.

## Máquinas de Estado Moore y Mealy

Los profesores de lógica digital aman preguntar en las pruebas sobre Moore vs. Mealy y es por eso que tenemos que mencionarlo. La distinción entre ellas muchas veces no hace sentido, mientras escribas en una maquina de estado en C; es más como una: distinción de “como hacer un hardware lógico”. Para nosotros la lección de Moore y Mealy es que existió gente que pensó sobre este tipo de cosas e inventó formas de notarlo. Mientras ellos se centraban en el hardware lógico, nosotros nos centraremos en el software c.

## Máquina de estado Moore

Edward Moore escribió un ensayo en 1956 (Gedanken-experiments on Sequential Machines) y por lo tanto el estilo de la máquina lleva su nombre.  El dice que la salida depende solo del estado, y el próximo estado es dependiente del estado actual (o salida), y la entrada.
 
 ![3](https://user-images.githubusercontent.com/66962449/93040948-e0d22700-f610-11ea-9ec4-5ed751903c01.jpg)
 
Nuestro diagrama previo
Puedes notar que no importa cuál será el estado de la entrada, la salida solo depende el estado actual contenido dentro del elemento de la memoria.

## Máquina de estado Mealy

George Mealy escribió un ensayo un año antes que Moore, titulado “A Method for Synthesizing Sequential Circuits”,  en el cual entra en profundidad acerca de crear máquinas de estado desde funciones matemáticas, y describe esas salidas de máquinas de estado en términos de sus entradas.
Para diagramar la máquina Mealy, la salida está hecha para depender de ambos: el estado actual y la entrada. Aquí la nube de la lógica de la próxima etapa contiene la lógica de salida también:
 
 ![4](https://user-images.githubusercontent.com/66962449/93040951-e4fe4480-f610-11ea-8ea8-0b41284be070.jpg)
 
Una forma de dibujar la máquina Mealy
También puede ser dibujado separando la nube en la lógica del próximo estado o lógica de salida.
 
 ![5](https://user-images.githubusercontent.com/66962449/93040967-f21b3380-f610-11ea-802c-a3ca1b2db717.jpg)
 
Otra forma de dibujar una máquina Mealy

## Diagramas de Estado Abstractos

Hasta ahora, hemos visto que las máquinas de estado tienen una memoria que almacena el estado actual, que debe provenir de algún estado, y que irá al siguiente estado. Aunque nuestro diagrama actual no muestra como se mueve a través de estados, el propósito debiese ser dibujar un mapa de movimiento entre los estados para que podamos escribir un código que emule nuestro diseño. Esto se llama diagrama de estado.
Este es un ejemplo de cómo se pueden diagramar los estados de una máquina de estado, usando ideas de Moore y Mealy.
 
 ![6](https://user-images.githubusercontent.com/66962449/93041005-0101e600-f611-11ea-995d-692ddc49cf95.jpg)
 
Un diagrama de estado abstracto
Partes del diagrama:
•	El círculo es el estado
•	El nombre coloquial del estado esta dado en la mitad superior del circulo
•	La salida del estado está dada en la mitad inferior del círculo. A veces esto es explicito, como “X=1,” y el estado se comporta como Moore, aunque a veces puede ser “SALIDA = ENTRADA” donde durante ese estado, hace la salida igual a lo que haya sido la entrada. En este sentido, la máquina es muy Mealy. Normalmente se engloban los dos para escribir máquinas de estado C porque realmente no importa la construcción C de la máquina.
•	La flecha es el recorrido de la transición de estado.
•	Las Xs, arriba de la línea, son las condiciones para que esa transición de estado ocurra. Si se dan las condiciones, ese será el recorrido de transición.
•	Las Ys, bajo la línea, son cosas que pasan durante la transición. Este concepto se desvía estrictamente del mundo lógico digital de Moore y Mealy y se origina de la naturaleza de ejecución consecutiva de C. Mientras utilizamos un programa, es fácil chequear las condiciones de transición y realizar algunas acciones de una sola vez mientras cambian los estados, entonces se deben poner las acciones bajo las condiciones.
Siempre ten en mente que estas son representaciones abstractas de códigos y son una herramienta para crear niveles más altos de operación. Agrega cuantos detalles necesites en el diagrama.
Considera un estado básico que se pueda mover hacia un nuevo estado.
 
 ![7](https://user-images.githubusercontent.com/66962449/93041037-124af280-f611-11ea-9e8e-57c6eca70ac6.jpg)
 
Estado simple con un set de transiciones de estado incompleto
¿Qué pasa si no se cumplen las condiciones de salida? El diagrama está incompleto y no se han  definido todas las posibles acciones del estado. Usualmente no sabríamos la solución completa del programa hasta que estén hechos los diagramas, y los vayamos completando. Con este diagrama, podemos asumir que si las condiciones no son concretadas, el estado volverá a sí mismo.
 
 ![8](https://user-images.githubusercontent.com/66962449/93041050-1f67e180-f611-11ea-9079-6988d2cbdf65.jpg)
 
Estado especificado completamente
Acá, se definen todas las posibles transiciones de estado.
Diagrama de estado del contador
Revisa el comportamiento del contador como se dibuja con un diagrama de estado.
 
 ![9](https://user-images.githubusercontent.com/66962449/93041247-b16fea00-f611-11ea-844f-41e2c200732d.jpg)
 
## Diagrama de estado de un contador simple
Acá todos los estados posibles son representados con un círculo único. La acción del estado es agregar uno. Para determinar el próximo estado, es fácil ver que sólo tenemos una opción, que es regresar al estado en que estábamos.

# 5. DIAGRAMAS
## 5.1. DIAGRAMAS DE ESTADO


# Bibliografia:
## [1]  Yang Sheng, Chen Xikun, Sun Dong y Liu Qinhuang, «Sci-Hub IEEEXplore» 28 de agosto de 2014
https://sci-hub.tw/https://ieeexplore.ieee.org/document/6885368
## [2] J. Kim y D. Kim , «Sci-Hub IEEEXplore»   29 de enero de 2015
https://sci-hub.tw/https://ieeexplore.ieee.org/document/7025478 
## [3] S. Wu, «Sci-Hub IEEEXplore»    20 de septiembre de 2012
https://sci-hub.tw/https://ieeexplore.ieee.org/document/6305768 

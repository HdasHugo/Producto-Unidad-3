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
![Diagrama 1 1](https://user-images.githubusercontent.com/68835261/93069737-a2a22b00-f643-11ea-8b5e-730e7e6dc2fb.JPG)

![Diagrama 1 2](https://user-images.githubusercontent.com/68835261/93069740-a3d35800-f643-11ea-9181-71be2ca47510.JPG)

![Máquina expendedora de bebidas](https://user-images.githubusercontent.com/68835261/93069802-b2217400-f643-11ea-929e-ea8bbd324622.JPG)

![Circuito de riego automático](https://user-images.githubusercontent.com/68835261/93069811-b483ce00-f643-11ea-9918-8bece3a6687b.JPG)

# 6. EXPLICACIÓN DEL CÓDIGO FUENTE
### 1.	Dibuje el diagrama de estados para la máquina de estado finito cuya tabla de estados es la siguiente. Partiendo del estado s0, calcula la salida para la cadena de entrada 1000110.
![Tabla 1 1](https://user-images.githubusercontent.com/68835261/93070025-fa409680-f643-11ea-85b6-3e8a18ee6b11.JPG)

![Figura 1 1](https://user-images.githubusercontent.com/68835261/93069903-d0876f80-f643-11ea-9b59-ef8ceaf5e2db.JPG)

### 2.	Dibuje el diagrama de estados para la máquina de estado finito cuya tabla de estados es la siguiente. Partiendo del estado inicial s0, calcula la salida para la cadena de entrada abbccc
![Tabla 1 2](https://user-images.githubusercontent.com/68835261/93070035-fdd41d80-f643-11ea-9006-2dbeb73e50cd.JPG)

![Figura 1 2](https://user-images.githubusercontent.com/68835261/93069914-d3826000-f643-11ea-9dd0-e8d3109e18b3.JPG)

### 3.	Halle la tabla de estados para la máquina de estado finito cuyo diagrama de estados es:
![Figura 1 3](https://user-images.githubusercontent.com/68835261/93069919-d67d5080-f643-11ea-98b8-6928c7d0957a.JPG)

![Tabla 1 3](https://user-images.githubusercontent.com/68835261/93070043-00cf0e00-f644-11ea-86a4-e473cb53e43a.JPG)

### 4.	Construya una máquina de estado finito que modele una máquina expendedora de bebidas que acepta monedas de 5, 10 y 20 centavos. La máquina acepta monedas hasta que se introducen 25 centavos y devuelve cualquier cantidad que supere los 25 céntimos. Entonces, el cliente puede pulsar los botones y elegir una bebida de cola (C), cerveza (Z) o agua (A). 

![Figura 1 4](https://user-images.githubusercontent.com/68835261/93069933-dc733180-f643-11ea-8624-b517ec37d21a.JPG)

Para la elaboración del diagrama de estados para la máquina expendedora de bebidas hemos necesitado de un total de 6 estados, denominados S0, S1, S2, S3, S4 y S5. Donde:

S0 --> 0 ctvs (máquina expendedora de bebidas activa).

S1 --> 5 ctvs.

S2 --> 10 ctvs.

S3 --> 15 ctvs.

S4 --> 20 ctvs.

S5 --> 25 ctvs (Entrega del producto).

Como podemos observar en la figura 1.4 nos encontramos con diferentes combinaciones en lo que respecta al ingreso de las diferentes monedas, es decir, podemos introducir 5 monedas de 5 ctvs. O también se podrían introducir dos monedas de 10 ctvs y una moneda de 5 ctvs. En ambos casos se sumaría un total de 25 ctvs. Y, por ende, se obtendría la bebida que el usuario desee. Sin embargo, también existe la posibilidad de sobrepasar los 25 ctvs, ya que, por ejemplo, se podrían introducir tres monedas de 10 ctvs. O una moneda de 20 ctvs y una de 10 ctvs. En ambos casos, obtendríamos la bebida que se escoja, pero adicional a ello la máquina expendedora también nos devolverá el cambio respectivo. Entonces independientemente de la combinación en la que se introduzcan las monedas, el sistema funcionará correctamente.

Ahora bien, las entradas que hemos utilizado en este diagrama de estados son las combinaciones binarias 00, 01, 10 y 11, las cuales corresponden a las monedas a introducir de 0, 5, 10 y 20 ctvs respectivamente. Y cuyas flechas de transición se han representado por los colores marrón, negro, naranja y azul, respectivamente, con fines de mejor entendimiento. Por otro lado, las flechas de transición de color verde hacen referencia a que el valor acumulado de monedas sobrepasa los 25 ctvs. Por lo que se obtendrá cambio.

Cabe recalcar que, solamente en el estado S5 se entrega la bebida escogida. Y una vez culminada esta acción, se retornará nuevamente al estado S0, para repetir el proceso si el usuario desea otra bebida o si otro usuario acude a la máquina expendedora.
Para entender de mejor manera el funcionamiento de dicha máquina, postulamos un ejemplo para los siguientes casos:

### - Inexistencia de cambio
No existirá cambio cuando la cantidad de dinero no supere los 25 ctvs. Por ejemplo:
Si se introducen 5 monedas de 5 ctvs, tenemos las siguientes transiciones: 

- S0 --> S1: Ingreso de la primera moneda. (Cantidad acumulada: 5 ctvs).

- S1 --> S2: Ingreso de la segunda moneda. (Cantidad acumulada: 10 ctvs).

- S2 --> S3: Ingreso de la tercera moneda. (Cantidad acumulada: 15 ctvs).

- S3 --> S4: Ingreso de la cuarta moneda. (Cantidad acumulada: 20 ctvs).

- S4 --> S5: Ingreso de la quinta moneda y entrega del producto. (Cantidad acumulada: 25 ctvs).

### - Existencia de cambio
Existirá cambio cuando la cantidad de dinero supere los 25 ctvs. Por ejemplo:
Si se introducen dos monedas de 10 ctvs y una de 20 ctvs, tendríamos las siguientes transiciones:

- S0 --> S2: Ingreso de la primera moneda de 10 ctvs. (Cantidad acumulada: 10 ctvs).

- S2 -> S4: Ingreso de la segunda moneda de 10 ctvs. (Cantidad acumulada: 20 ctvs).

- S4 --> S5: Ingreso de la moneda de 20 ctvs. (Cantidad acumulada: 40 ctvs). Entrega de cambio       y entrega del producto.

Finalmente presentamos a continuación la tabla de transiciones que describe todo el proceso explicado con el diagrama de estados realizado.

![Tabla 1 41](https://user-images.githubusercontent.com/68835261/93072473-1134b800-f647-11ea-8456-f35da550a69a.JPG)

### 5.	Construya una máquina de estados finito que modele un circuito de riego automático como el mostrado en la figura. El circuito deberá accionar la bomba en las siguientes condiciones:
### a)	El circuito accionará la bomba solamente cuando la tierra esté seca, pero antes debe comprobar las siguientes condiciones:
i.	Para evitar que la bomba se estropee por funcionar en vacío, nunca se accionará la bomba cuando el depósito de agua esté vacío.
ii.	Si hay restricciones en el riego (época de verano), sólo se podrá regar de noche.
iii.	En el resto del año (si no hay restricciones) se podrá regar de día y de noche (si la tierra está seca).
### b)	Para la implementación del circuito se dispone de las siguientes entradas:
i.	S: Señal que indica si la tierra está seca: Tierra seca: S=1; Tierra húmeda: S=0
ii.	R: Señal que indica si hay restricciones en el riego (es verano): Hay restricciones: R=1. No hay restricciones: R=0.
iii.	D: Señal que indica si es de día o de noche: Día: D=1; Noche: D=0.
iv.	V: Señal que indica si el depósito de agua está vacío: Vacío: V=1; Hay agua: V=0.
### c)	Y la salida B, que accionará la bomba para regar: Bomba funcionando: B=1; Bomba apagada B=0.
![Figura 1 5](https://user-images.githubusercontent.com/68835261/93069945-e137e580-f643-11ea-8c19-bd685edd2f90.JPG)

Para la elaboración del diagrama de estados para un sistema de riego automático hemos utilizado un total de 6 estados, denominados V, R, D, N, S, B, donde:

V --> Depósito de agua lleno o vacío.

R --> Existencia de restricción (Época de verano o no).

D --> Estado que indica si es de día.

N --> Estado que indica si es de noche.

S --> Estado que indica si la tierra está seca o no.

B --> Estado final (Bomba de agua activada).

Como podemos observar en la figura 1.4 nos encontramos con una variable de entrada que puede tomar el valor de 1 o 0 lógico, cuyo valor influenciará en la transición de cada uno de los estados. Como sabemos la bomba se accionará siempre y cuando la tierra esté seca y es por ello que los dos estados que representan a estas condiciones se encuentran al último de nuestro diagrama, sin embargo, se deben cumplir los demás requisitos que nos estipula la problemática del enunciado, y es por ello que el estado V es el inicial, ya que necesitamos que el depósito de agua se encuentre lleno para seguir con el resto del proceso, entonces, si el estado V recibe un valor de 1 lógico, tenemos que el sistema permanecerá en el mismo estado, caso contrario pasaremos al estado R, el cual determinará si existe restricción (es verano) o no. En el caso de no existir restricción, pasaremos al estado D (es de día). Caso contrario pasaremos al estado N.
Una vez que pasamos de R a D y este último reciba un valor de 1, entonces pasaremos al estado S. De no ser así, se entiende que es de noche y pasaremos al estado N, que por consiguiente pasará al estado S.

Por otro lado, si pasamos de R a N y este último recibe un valor de 1, entonces pasaremos al estado S. Caso contrario regresaremos de N a R, de esta manera nos cercioramos que solo se riegue en la noche, ya que nos encontramos en época de verano.

Finalmente, el estado S es el que determinará si se va a activar o no la bomba de agua. Entonces si la tierra está seca pasaremos al estado B, el cual representa que el sistema de riego funciona en ese momento. Caso contrario, tendríamos que la tierra no está seca, por consiguiente, regresaríamos nuevamente el estado R y se repetiría el proceso hasta que la tierra esté seca.
Una vez que se culmine el proceso de riego, el sistema se reiniciará, pasando del estado B al estado inicial V.

Para entender de mejor manera, postulamos los siguientes ejemplos:
### -	Suponiendo que el depósito de agua está lleno, la tierra está seca, no es época de verano y es de día, la transición de estados se vería de la siguiente manera:
- V --> R: Tanque de agua lleno.
- R --> D: No es época de verano.
- D --> S: Es de día.
- S --> B: La tierra está seca. (Se activa la bomba de agua).

### -	Suponiendo que el depósito de agua está lleno, la tierra está seca, no es época de verano y es de noche, la transición de estados se vería de la siguiente manera:
- V --> R: Tanque de agua lleno.
- R --> D: No es época de verano.
- D --> N: No es de día.
- N --> S: Es de noche.
- S --> B: La tierra está seca. (Se activa la bomba de agua).

### -	Suponiendo que el depósito de agua está lleno, la tierra está seca, es época de verano y es de día, la transición de estados se vería de la siguiente manera:
- V --> R: Tanque de agua lleno.
- R --> N: Es época de verano.
- N --> R: No es de noche (Regresa al estado R para verificar si es época de verano o no). 

### -	Suponiendo que el depósito de agua está lleno, la tierra está seca, es época de verano y es de noche, la transición de estados se vería de la siguiente manera:
- V --> R: Tanque de agua lleno.
- R --> N: Es época de verano.
- N --> S: Es de noche.
- S --> B: La tierra está seca. (Se activa la boba de agua).

Finalmente presentamos a continuación la tabla de transiciones que describe todo el proceso explicado con el diagrama de estados realizado. 

![Tabla 1 5](https://user-images.githubusercontent.com/68835261/93070064-075d8580-f644-11ea-91e4-945785692f5f.JPG)
![Tabla 1 6](https://user-images.githubusercontent.com/68835261/93070075-0af10c80-f644-11ea-992a-79cf18997c5b.JPG)

# 7. DESCRIPCIÓ DE PRERREQUISITOS Y CONFIGURACIÓN
En lo que corresponde a la utilización de aplicaciones secundarias para elaborar los diferentes grafos de estado, podemos decir que no se ha necesitado de ninguna que influya directamente sobre su implementación, ya que Creately ofrece una interfaz de desarrollo de diagramas muy extenso y completo. 

Ahora bien, necesitamos saber cuales son los pasos para poder implementar diagramas de estados en Creately. Para lo cual, debemos:

1.	Seleccionar en la sección de formas, todos los elementos o figuras que se utilizarán en el circuito, (En nuestro caso seleccionaremos el círculo). Y arrastrarlo a la hoja de trabajo.

![DP1](https://user-images.githubusercontent.com/68835261/93069953-e432d600-f643-11ea-9569-42575dc9cccb.JPG)

2.	Conectar todas las formas (Estados) mediante un conector.

![DP2](https://user-images.githubusercontent.com/68835261/93069964-e72dc680-f643-11ea-9599-191d08aceb05.JPG)

3.	Una vez que ya se ha realizado la conexión entre los estados procedemos a dar clic en el conector y se nos desplegará un recuadro con opciones, en el cual podemos escoger la dirección del conector representado por una flecha, cambiar de color, colocar texto y cambiar la forma del conector.

![DP3](https://user-images.githubusercontent.com/68835261/93069970-e9902080-f643-11ea-96e4-3d63ec71f17f.JPG)

4.	Finalmente, el diagrama de estados terminado quedaría de la siguiente manera:

![DP4](https://user-images.githubusercontent.com/68835261/93069976-ebf27a80-f643-11ea-9ae7-1ba3ac7c0bc4.JPG)

# 8. APORTACIONES
### Implementación de sistema de riego automático en un circuito lógico
El procedimiento que se llevó a cabo para representar e implementar el sistema de riego automático en un circuito lógico fue el realizar la tabla de verdad con las 4 variables de entrada V, S, D y R (Tabla 1.7), simplificar mediante mapas de Karnaugh y obtener la función lógica resultante (Figura 1.6).
![Tabla 1 7](https://user-images.githubusercontent.com/68835261/93070096-0f1d2a00-f644-11ea-89de-cdee5dd2c7d5.JPG)
![Figura 1 6](https://user-images.githubusercontent.com/68835261/93070113-13e1de00-f644-11ea-89be-1a761336ed9e.JPG)

Por lo tanto, la función lógica implementada nos queda, tal como se observa en la sección derecha de la figura 1.7 
![Figura 1 7](https://user-images.githubusercontent.com/68835261/93070127-16dcce80-f644-11ea-82c4-917590d0329d.JPG)
![Figura 1 8](https://user-images.githubusercontent.com/68835261/93070133-1a705580-f644-11ea-8379-f49c43779e27.JPG)

# 9. CONCLUSIONES
-	Los diagramas de estado, para el primer y segundo ejercicio, se han diseñado, partiendo de la tabla de estados proporcionadas, mientras que en el tercer ejercicio se implementó la tabla de estados partiendo de un diagrama de estados. Toda su realización fue de gran importancia para aplicar el mismo principio en una máquina expendedora de bebidas y en un sistema de riego automático, donde cada uno de sus estados se representaron en base a los requerimientos de cada problema. Si nos damos cuenta, se utilizaron un total de 6 estados en los dos casos, cuyas transiciones, dependieron de la moneda que se inserte en la máquina expendedora y de las diferentes condiciones que se requerían para que la bomba de agua se active en el sistema de riego.

-	Al realizar cada diagrama y tabla de estado podemos deducir que todos están relacionados con una máquina de Mealy, ya que las variables de entradas y salidas se encuentras en las transiciones (conectores) que claramente dependen a su vez del estado en el que se encuentren, en otras palabras, la salida depende de la condición de entrada que debe existir y del estado en el que se encuentre en ese momento.

-	El diseño de cada circuito se la realizó en base a todo lo investigado, lo cual tiene que ver con las funcionalidades que ofrecen los diagramas y tablas de estado para aplicarlos en circuitos lógicos secuenciales. Cabe mencionar que esto es la base de una gran cantidad de aplicaciones en lo que respecta a sistemas digitales, ya que tienen una amplia relevancia e importancia. Sin duda los diagramas de estado, son la base para implementar un sinnúmero de aplicaciones, pues han sido muy importantes en el avance de la electrónica y de la tecnología. Lo más esencial para nosotros es conocer cómo es su funcionamiento (interacción entre estados y variables de entrada) y mediante esta práctica se ha cumplido este objetivo. De hecho, al momento de realizar la investigación con los artículos de los autores investigados, podemos darnos cuenta de la gran cantidad de aplicaciones que tienen y que de cierta manera se relaciona con nuestro proyecto en cuestión.

# 10. RECOMENDACIOINES
-	Se recomienda realizar la investigación única y exclusivamente de los temas a ser tratados durante la ejecución y realización del informe que a su vez sustenten los fundamentos para el diseño e implementación del circuito. 

-	Cerciorarse que la transición entre los diferentes estados del sistema, junto con las entradas sea la correcta para evitar fallos en las salidas.

-	Comparar detalladamente los Datasheet de cada componente que usemos, puesto que, si no lo verificamos, los datos de salida del circuito integrado pueden ser erróneos y esto causará que el funcionamiento del circuito implementado no sea el correcto, incluso pueden ocurrir averías en los mismos, por ello es importante identificar los pines de entrada, salida y de energía, con su respectiva numeración.
# 11. CRONOGRAMA

# 12. BIBLIOGRAFÍA
## [1]  Yang Sheng, Chen Xikun, Sun Dong y Liu Qinhuang, «Sci-Hub IEEEXplore» 28 de agosto de 2014
https://sci-hub.tw/https://ieeexplore.ieee.org/document/6885368
## [2] J. Kim y D. Kim , «Sci-Hub IEEEXplore»   29 de enero de 2015
https://sci-hub.tw/https://ieeexplore.ieee.org/document/7025478 
## [3] S. Wu, «Sci-Hub IEEEXplore»    20 de septiembre de 2012
https://sci-hub.tw/https://ieeexplore.ieee.org/document/6305768 

# 13. ANEXOS
## 13.1. HOJAS TÉCNICAS


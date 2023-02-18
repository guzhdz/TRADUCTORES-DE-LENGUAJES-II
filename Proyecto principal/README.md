# Compilador

Un traductor es un programa que recibe como entrada código escrito en un cierto lenguaje y produce como salida código en otro lenguaje.

https://sciatel.wikispaces.com/TRADUCTORES+DEL+LENGUAJE+DE+PROGRAMACION

Un compilador es un programa informático que traduce un programa que ha sido escrito en un lenguaje de programación a un lenguaje común, usualmente lenguaje de máquina, aunque también puede ser traducido a un código intermedio (bytecode) o a texto. Este proceso de traducción se conoce como compilación.

https://es.wikipedia.org/wiki/Compilador

# Analizador Lexico
Link: https://github.com/guzhdz/TRADUCTORES-DE-LENGUAJES-II/tree/main/Proyecto%20principal%20(Por%20partes)/Analizador%20Lexico

El Análisis Léxico es la primera fase de un compilador, este consiste en un programa que recibe como entrada el código fuente de otro programa (secuencia de caracteres) y produce una salida compuesta de tokens (componentes léxicos) o símbolos. 

# Tarea: Mini generador léxico 
Genera un pequeño analizador léxico, que identifique los siguientes tokens (identificadores y números reales) construidos de la siguiente manera.
identificadores = letra(letra|digito)*
Real = entero.entero+

El codigo se encuentra en los archivos script.js y analizador.js, para ejecutarlos puede simplemente compilar y correr el archivo script.js o usar la extension de live server de VS Code para hacer deploy del index.html y en consola ver el resultado de la ejecucion.

Resultado de la ejecucion:
![Mini analizador img 1](https://user-images.githubusercontent.com/89165084/213944343-8f33242a-b181-4698-93a7-c2b1be2fcc3a.jpg)
![Mini analizador img 2](https://user-images.githubusercontent.com/89165084/213944420-bc4f6c95-de59-4618-8b0c-914a9ce720c0.jpg)


# Tarea: Etapa del proyecto analizador léxico completo.
Genera un analizador léxico utilizando todos los símbolos léxicos en el archivo simbolos_lexicos.pdf.

Resultado de la ejecucion:

![Analizador completo img 1](https://user-images.githubusercontent.com/89165084/213944726-ec851892-1ca3-4041-afac-36f8ae2a7296.jpg)!
![Analizador completo img 2](https://user-images.githubusercontent.com/89165084/213944892-50c32dfd-bedf-4cc9-b39f-dbef5ddffcfc.jpg)!

Se mejoro el aspecto visual, de manera que ahora si se ejecuta en un servidor local o con la extension live server de visual code el archivo index.html, aparecera una interfaz visual que permitira ingresar cualquier texto y lo analizara:

![Lexico visual1](https://user-images.githubusercontent.com/89165084/216058211-45b5e04a-d30b-4e36-8872-c6eb2074101f.jpg)

![Lexico visual2](https://user-images.githubusercontent.com/89165084/216058237-a12973df-fb88-4dd8-a91e-8b2237fc4bcb.jpg)

# Analizador sintactico
Un analizador sintáctico, es un programa informático que analiza una cadena de símbolos según las reglas de una gramática formal. El análisis sintáctico convierte el texto de entrada en otras estructuras (comúnmente árboles), que son más útiles para el posterior análisis y capturan la jerarquía implícita de la entrada. 

Un analizador léxico crea tokens de una secuencia de caracteres de entrada y son estos tokens los que son procesados por el analizador sintáctico para construir la estructura de datos, por ejemplo un árbol de análisis o árboles de sintaxis abstracta. 

El uso más común de los analizadores sintácticos es como parte de la fase de análisis de los compiladores. De modo que tienen que analizar el código fuente del lenguaje, los lenguajes de programación tienden a basarse en gramáticas libres de contexto, debido a que se pueden escribir analizadores rápidos y eficientes para estas.

# Tarea: Mini analizador sintáctico (Excel)
Subir un archivo en excel simulando las gramáticas del ejercicio 1 y 2 del archivo (Practica Analizador Sintactico LR.pdf)

Entrada para el Ejercicio 1
hola+mundo

Entrada para el Ejercicio 2
a+b+c+d+e+f

Link de archivo: https://github.com/guzhdz/TRADUCTORES-DE-LENGUAJES-II/blob/main/Tareas/Tarea%202.%20Mini%20analizador%20sintactico/Mini%20analizador%20sint%C3%A1ctico%20(Excel).pdf

# Tarea: Mini analizador sintáctico (código)
Generar un algoritmo para analizar los Ejercicios 1 y 2 del archivo (PracticaAnalizadorSintactico.pdf)

Se modifico el codigo del analizador lexico para que funcionara junto con un codigo nuevo y hicira la funcion del analizador sintactico. Se agrego una nueva clase (Sintactico) la cual realiza as tareas importantes del mismo, ademas de que se cambio la interfaz para que concordara con el objetivo de este mini analizador sintactico.

Link del proyecto: https://github.com/guzhdz/TRADUCTORES-DE-LENGUAJES-II/tree/main/Tareas/Tarea%202.%20Mini%20analizador%20sintactico/Mini%20analizador%20sintactico%20programa

El proyecto puede ejecutarse en un servidor local o mediante la extension de live server de visual code, ejecutando el index.html.

Foto del codigo:

![image](https://user-images.githubusercontent.com/89165084/216158896-8cb0f7ee-7cd4-4c8a-90ed-876efc65695e.png)

Tablas LR en las que se baso el codigo:

![image](https://user-images.githubusercontent.com/89165084/216159161-9e1cdc1b-b374-48d8-aeab-01dfb023f9de.png)

![image](https://user-images.githubusercontent.com/89165084/216159390-5e52721e-aa6b-4729-9a4d-fd20a71e23b5.png)

Prueba y ejecucion del codigo del Ejercicio 1:

![image](https://user-images.githubusercontent.com/89165084/216159777-45f6c593-721b-4c14-93fb-43335ffb41c9.png)

Prueba y ejecucion del codigo del Ejercicio 2:

![image](https://user-images.githubusercontent.com/89165084/216160956-22bb9bee-eb72-49fd-bfa2-d0586d7a0fb6.png)
![image](https://user-images.githubusercontent.com/89165084/216161014-4494532f-6c4b-41e3-bd81-e439b35aa6ef.png)
![image](https://user-images.githubusercontent.com/89165084/216161151-3f58e151-f901-40c1-aa00-9b7019499237.png)

# Tarea: Gramática del compilador
Utilizando tu analizador léxico y tu algoritmo para trabajar con las tablas lr. Carga e implementa la siguiente gramática.
(Los archivos de la garmatica esten en: )

### 1. Transición de Scratch a C y Conceptos Fundamentales

La lección marca un cambio significativo del lenguaje de programación visual Scratch a C, un lenguaje de programación textual. Se enfatiza que los conceptos aprendidos en Scratch son universalmente aplicables a cualquier lenguaje de programación.

- **Universalidad de Conceptos:** "De hecho, todos los conceptos esenciales de programación presentados en Scratch se utilizarán a medida que aprendas a programar cualquier lenguaje. Las funciones, condicionales, bucles y variables presentes en Scratch son componentes fundamentales de cualquier lenguaje de programación." (3.pdf)
- **Código Fuente y Código Máquina:** Se explica la distinción crucial entre el "código fuente", que son instrucciones legibles por humanos, y el "código máquina" (binario, es decir, unos y ceros), que es lo que las computadoras realmente entienden. (3.pdf)
- **El Compilador:** Para convertir el código fuente a código máquina, se utiliza un "compilador". Para C, se introduce la herramienta make. "Resulta que podemos convertir código fuente a código máquina mediante un programa muy especial llamado compilador." (3.pdf)

### 2. Entorno de Desarrollo: Visual Studio Code (VS Code) para CS50

El curso utiliza Visual Studio Code (VS Code), accesible a través de cs50.dev, como entorno de desarrollo integrado (IDE). Este entorno viene preconfigurado con todo el software necesario para el curso.

- **Ventajas de VS Code:** La principal ventaja es que "ya incluye todo el software necesario para el curso." (3.pdf) Se desaconseja la instalación manual de software para evitar "dolores de cabeza". (2.pdf, 0:05:10-0:05:15)
- **Componentes del IDE:** VS Code se divide en varias regiones:
- **Explorador de Archivos:** A la izquierda, para visualizar y manipular archivos y carpetas. (3.pdf)
- **Editor de Texto:** En la sección central superior derecha, donde se escribe el código. (3.pdf, 2.pdf, 0:06:10-0:06:14)
- **Interfaz de Línea de Comandos (CLI) / Ventana de Terminal:** En la parte inferior, para enviar comandos al sistema. "La programación de resolución de problemas es, en realidad, se trata de que la entrada se convierta en salida." (2.pdf, 0:04:26-0:04:30)

### 3. Comandos de Línea de Comandos (CLI)

Se introducen varios comandos fundamentales para interactuar con el sistema de archivos a través de la terminal:

- cd: Cambiar directorio. (3.pdf)
- cp: Copiar archivos y directorios. (3.pdf)
- ls: Listar archivos en un directorio. (3.pdf)
- mkdir: Crear un directorio. (3.pdf)
- mv: Mover (renombrar) archivos y directorios. (3.pdf)
- rm: Eliminar (borrar) archivos. (3.pdf)
- rmdir: Eliminar (borrar) directorios. (3.pdf)

Estos comandos permiten a los programadores manipular archivos y directorios de manera eficiente, a menudo preferible al uso del ratón para tareas repetitivas. (2.pdf, 0:06:55-0:07:02)

### 4. Creando el Primer Programa en C: "Hello, World"

El proceso de crear, compilar y ejecutar un programa en C se demuestra con el clásico "Hello, World".

- **Pasos:**

1. **Crear el archivo:** code hello.c (2.pdf, 0:09:28-0:09:31)
2. **Escribir el código:** El código debe ser preciso, ya que "cada carácter tiene un propósito". (3.pdf) Un ejemplo básico:
3. #include <stdio.h>
4. int main(void) {
5. printf("hello, world\n");
6. }
7. **Compilar:** make hello. Esto convierte el código fuente (.c) en un archivo ejecutable. Si no hay errores, no se muestra ningún mensaje. (2.pdf, 0:14:15-0:14:22)
8. **Ejecutar:** ./hello. El ./ es necesario para indicar que el programa está en el directorio actual. (2.pdf, 0:18:16-0:18:22)

- **printf y Secuencias de Escape:** printf es la función en C para imprimir texto en la pantalla. La secuencia \n es una "secuencia de escape" que crea un salto de línea. Otras secuencias de escape incluyen \r (retorno de carro), \" (comillas dobles), \' (comillas simples) y \\ (barra invertida). (3.pdf)

### 5. Archivos de Encabezado (Header Files) y Bibliotecas

Las bibliotecas son colecciones de código preescrito que otros han creado y que pueden ser reutilizadas. Para usar funciones de una biblioteca, se debe incluir su archivo de encabezado.

- **#include <stdio.h>:** Permite el uso de funciones como printf, que está contenida en la biblioteca stdio.h (Standard Input/Output). (3.pdf)
- **#include <cs50.h>:** CS50 proporciona su propia biblioteca con funciones útiles para principiantes, como get_string, get_int, get_char, etc., que simplifican la entrada del usuario. (3.pdf)
- **Páginas del Manual (Man Pages):** La documentación para las funciones de C se encuentra en las páginas del manual (o man pages). CS50 ofrece una versión más amigable en manual.cs50.io. (3.pdf)

### 6. Variables y Tipos de Datos

Las variables son "lugares de almacenamiento especiales" para guardar valores. En C, se debe especificar el "tipo" de datos que una variable almacenará.

- **Declaración de Variables:** tipo nombre_variable = valor; Por ejemplo: string answer = get_string("What's your name? "); (3.pdf)
- **Tipos de Datos Comunes en C:**string: Cadena de texto. (3.pdf)
- int: Números enteros. (3.pdf)
- bool: Valores booleanos (true o false). (3.pdf)
- char: Caracteres individuales. (3.pdf) Se usan comillas simples ('y') para caracteres, a diferencia de las comillas dobles ("hola") para cadenas. (2.pdf, 0:18:24-0:18:32)
- float: Números reales con decimales (punto flotante). (3.pdf)
- double: Valores de punto flotante con mayor precisión que float. (3.pdf)
- long: Números enteros con más bits, para valores más grandes que int. (3.pdf)
- **Códigos de Formato (printf):** Para imprimir valores de variables con printf, se usan "códigos de formato" (placeholders):
- %s: para cadenas (string). (3.pdf)
- %i: para enteros (int). (3.pdf)
- %c: para caracteres (char). (3.pdf)
- %f: para flotantes (float). (3.pdf)
- %li: para long enteros. (3.pdf)
- **Truncamiento y Desbordamiento (Overflow):Truncamiento:** La división de enteros en C trunca el resultado (elimina la parte decimal), en lugar de redondear. Por ejemplo, 1 / 3 da 0, y 3 / 2 da 1. (3.pdf, 2.pdf, 0:02:26:45-0:02:27:11)
- **Desbordamiento de Enteros (Integer Overflow):** Los tipos de datos tienen límites de memoria (ej. int con 32 bits puede contar hasta ~4 mil millones). Si un valor excede este límite, el número "desborda" y se convierte en un valor incorrecto (ej. negativo o cero). (3.pdf, 2.pdf, 0:02:19:42-0:02:20:32) Este es un problema fundamental en computación con implicaciones reales (ej. el error del Boeing 787 o Pac-Man).

### 7. Condicionales (If/Else)

Las estructuras condicionales permiten que el programa tome decisiones basadas en si una expresión es verdadera o falsa.

- **Sintaxis Básica:**if (condicion) {
- // código a ejecutar si la condición es verdadera
- } else {
- // código a ejecutar si la condición es falsa
- }
- **else if:** Permite evaluar múltiples condiciones en secuencia.
- **Operadores de Comparación:**<: Menor que
- >: Mayor que
- ==: Igual a (¡dos signos de igual para comparación, uno para asignación!)
- !=: No es igual a
- <=: Menor o igual que
- >=: Mayor o igual que
- **Operadores Lógicos:**||: OR lógico (para verificar si _una_ de varias condiciones es verdadera).
- &&: AND lógico (para verificar si _todas_ las condiciones son verdaderas).

### 8. Bucles (Loops)

Los bucles permiten repetir bloques de código varias veces.

- **while Loop:** Repite un bloque de código "mientras" una condición sea verdadera.
- int i = 3;
- while (i > 0) {
- printf("meow\n");
- i--; // Decrementa i
- }
- **for Loop:** Una forma más concisa de un bucle while cuando se conoce el número de iteraciones.
- for (int i = 0; i < 3; i++) {
- printf("meow\n");
- }
- Incluye inicialización, condición y actualización del contador en una sola línea.
- **do-while Loop:** Ejecuta el bloque de código al menos una vez, y luego continúa repitiendo "mientras" la condición sea verdadera. Útil para obtener entrada de usuario válida.
- int n;
- do {
- n = get_int("Number: ");
- } while (n < 1);
- **break:** Se utiliza dentro de un bucle para salir forzadamente de él antes de que la condición del bucle se vuelva falsa.

### 9. Funciones Definidas por el Usuario

Los programadores pueden crear sus propias funciones para abstraer y reutilizar el código.

- **Sintaxis:**tipo_retorno nombre_funcion(tipo_parametro nombre_parametro) {
- // cuerpo de la función
- return valor; // Opcional, si tipo_retorno no es void
- }
- **void:** Si una función no devuelve ningún valor, su tipo_retorno es void. Si no toma ningún argumento, el tipo_parametro es void. (3.pdf)
- **Prototipos de Función:** En C, si una función se define _después_ de ser llamada (como es convencional para main estar al principio), se debe declarar un "prototipo" de la función al principio del archivo. Esto le dice al compilador que la función existirá más adelante. "Observe cómo meow se llama a la función con la meow() instrucción. Esto es posible porque la meow función se define al final del código y su prototipo se proporciona al principio como void meow(void)." (3.pdf)
- **Parámetros:** Las funciones pueden aceptar "parámetros" (entradas) para hacerlas más flexibles y reutilizables (ej. void meow(int n) para maullar n veces).
- **Valores de Retorno:** Las funciones pueden devolver un valor utilizando la palabra clave return. Esto permite que una función calcule algo y entregue ese resultado a la parte del programa que la llamó (ej. get_positive_int que devuelve un int).

### 10. Calidad del Código: Corrección, Diseño y Estilo

Se presentan tres pilares para evaluar la calidad del código, cruciales en la programación real y en el curso:

- **Corrección:** "¿El código se ejecuta como se espera?". Se puede verificar con check50. (3.pdf)
- **Diseño:** "¿Qué tan bien está diseñado el código?". Se refiere a la eficiencia, claridad y generalización del código. Por ejemplo, evitar la repetición excesiva (principio "no te repitas") o el uso de "números mágicos" (constantes). Se puede evaluar con design50. (3.pdf)
- **Comentarios:** Los comentarios (usando // para una sola línea o /* ... */ para bloques) permiten a los programadores documentar su código en lenguaje humano, lo que es vital para comprender la lógica más adelante o para otros colaboradores. (3.pdf)
- **Constantes:** Usar const para variables cuyo valor no debe cambiar (ej. const int N = 3;) mejora el diseño y previene errores accidentales. (3.pdf)
- **Estilo:** "¿Qué tan estéticamente agradable y consistente es el código?". Se relaciona con el formato y la legibilidad. Se puede evaluar con style50. (3.pdf) Incluye aspectos como la sangría y el espaciado.

### 11. Implicaciones de las Limitaciones de la Computación

Se destacan problemas inherentes a la forma en que las computadoras manejan los números y la memoria, que pueden llevar a errores inesperados:

- **Imprecisión de Punto Flotante:** La representación de números reales con decimales en binario es inherentemente imprecisa debido a la cantidad finita de bits. Esto puede llevar a resultados ligeramente incorrectos en cálculos con decimales. (2.pdf, 0:02:29:54-0:02:31:16)
- **Problemas Históricos Reales:** Se citan ejemplos como el error de desbordamiento de enteros en el Boeing 787 y el "Kill Screen" de Pac-Man en el nivel 256, que ilustran cómo la falta de consideración de los límites de los tipos de datos puede causar fallos críticos. (3.pdf)
- **El Problema del Año 2000 (Y2K) y el Problema del Año 2038:** Se mencionan como ejemplos de problemas causados por la limitación de bits o dígitos en la representación de fechas y horas, lo que puede causar desbordamientos en el futuro. (3.pdf, 2.pdf, 0:02:31:40-0:02:34:02)
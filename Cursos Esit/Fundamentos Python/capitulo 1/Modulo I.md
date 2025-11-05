Lección 1
1. La función print() es una función integrada imprime/envía un mensaje específico a la pantalla/ventana de consola.
2. Las funciones integradas, al contrario de las funciones definidas por el usuario, están siempre disponibles y no tienen que ser importadas. Python 3.7.1 viene con 69 funciones incorporadas. Puedes encontrar su lista completa en orden alfabético en Python Standard Library.
3. Para llamar a una función (invocación de función), debe utilizarse el nombre de la función seguido de un paréntesis. Puedes pasar argumentos a una función colocándolos dentro de los paréntesis. Se deben separar los argumentos con una coma, por ejemplo, print("¡Hola,", "Mundo!"). Una función print() "vacía" imprime una línea vacía a la pantalla.
4. Las cadenas de Python están delimitadas por comillas, por ejemplo, "Soy una cadena" (comillas dobles), o 'Yo soy una cadena, también' (comillas simples).
5. Los programas de computadora son colecciones de instrucciones. Una instrucción es un comando para realizar una tarea específica cuando se ejecuta, por ejemplo, para imprimir un determinado mensaje en la pantalla.
6. En las cadenas de Python la barra diagonal inversa (\) es un carácter especial que anuncia que el siguiente carácter tiene un significado diferente, por ejemplo, \n (el carácter de nuevalínea) comienza una nuevalínea de salida.
7. Los argumentos posicionales son aquellos cuyo significado viene dictado por su posición, por ejemplo, el segundo argumento se emite después del primero, el tercero se emite después del segundo, etc.
8. Los argumentos de palabra clave son aquellos cuyo significado no está dictado por su ubicación, sino por una palabra especial (palabra clave) que se utiliza para identificarlos.
9. Los parámetros end y sep se pueden usar para dar formato la salida de la función print(). El parámetro sep especifica el separador entre los argumentos emitidos. Por ejemplo, print("H", "E", "L", "L", "O", sep="-"), mientras que el parámetro end especifica que imprimir al final de la declaración de impresión.

Lección 2
1. Los literales son notaciones para representar valores fijos en el código. Python tiene varios tipos de literales - es decir, un literal puede ser un número por ejemplo, 123), o una cadena (por ejemplo, "Yo soy un literal.").
2. El sistema binario es un sistema numérico que emplea 2 como su base. Por lo tanto, un número binario está compuesto por 0s y 1s únicamente, por ejemplo, 1010 es 10 en decimal.
   Los sistemas de numeración Octales y Hexadecimales son similares pues emplean 8 y 16 como sus bases respectivamente. El sistema hexadecimal utiliza los números decimales más seis letras adicionales.
3. Los enteros (o simplemente int) son uno de los tipos numéricos que soporta Python. Son números que no tienen una parte fraccionaria, por ejemplo, 256, o -1 (enteros negativos).
4. Los números punto-flotante (o simplemente flotantes) son otro tipo numérico que soporta Python. Son números que contienen (o son capaces de contener) una parte fraccionaria, por ejemplo, 1.27.
5. Para codificar un apóstrofe o una comilla dentro de una cadena se puede utilizar el carácter de escape, por ejemplo, 'I\'m happy.', o abrir y cerrar la cadena utilizando un conjunto de símbolos distintos al símbolo que se desea codificar, por ejemplo, "I'm happy." para codificar un apóstrofe, y 'El dijo "Python", no "typhoon"' para codificar comillas.
6. Los valores booleanos son dos objetos constantes True y False empleados para representar valores de verdad (en contextos numéricos 1 es True, mientras que 0 es False.
   Extra  
   Existe un literal especial más utilizado en Python: el literal None. Este literal es llamado un objeto de NoneType, y puede ser utilizado para representar la ausencia de un valor. Pronto se hablará más acerca de ello.

Lección 3 
1. Una **expresión** es una combinación de valores (o variables, operadores, llamadas a funciones, aprenderás de ello pronto) las cuales son evaluadas y dan como resultado un valor, por ejemplo, 1 + 2.
2. Los **operadores** son símbolos especiales o palabras clave que son capaces de operar en los valores y realizar operaciones matemáticas, por ejemplo, el * multiplica dos valores: x * y.
3. Los operadores aritméticos en Python: + (suma), - (resta), * (multiplicación), / (división clásica: regresa un flotante siempre), % (módulo: divide el operando izquierdo entre el operando derecho y regresa el residuo de la operación, por ejemplo, 5 % 2 = 1), ** (exponenciación: el operando izquierdo se eleva a la potencia del operando derecho, por ejemplo, 2 ** 3 = 2 * 2 * 2 = 8), // (división entera: retorna el número resultado de la división, pero redondeado al número entero inferior más cercano, por ejemplo, 3 // 2.0 = 1.0)
4. Un operador **unario** es un operador con solo un operando, por ejemplo, -1, o +3.
5. Un operador **binario** es un operador con dos operandos, por ejemplo, 4 + 5, o 12 % 5.
6. Algunos operadores actúan antes que otros, a esto se le llama - **jerarquía de prioridades**:
	- El operador ** (exponencial) tiene la prioridad más alta;
	- Posteriormente los operadores unarios + y - (nota: los operadores unarios a la derecha del operador exponencial enlazan con mayor fuerza, por ejemplo 4 ** -1 es igual a 0.25)
	- Después *, /, //, y %,
	- Finalmente, la prioridad más baja: los operadores binarios + y -.
7. Las sub-expresiones dentro de **paréntesis** siempre se calculan primero, por ejemplo,  15 - 1 * ( 5 *( 1 + 2 ) ) = 0.
8. Los operadores de **exponenciación** utilizan **enlazado del lado derecho**, por ejemplo, 2 ** 2 ** 3 = 256.

Lección 4
1. Una variable es una ubicación nombrada reservada para almacenar valores en la memoria. Una variable es creada o inicializada automáticamente cuando se le asigna un valor por primera vez. (2.1.4.1)
2. Cada variable debe de tener un nombre único - un identificador. Un nombre válido debe ser aquel que no contiene espacios, debe comenzar con un guion bajo(_), o una letra, y no puede ser una palabra reservada de Python. El primer carácter puede estar seguido de guiones bajos, letras, y dígitos. Las variables en Python son sensibles a mayúsculas y minúsculas.
3. Python es un lenguaje de tipo dinámico, lo que significa que no se necesita declarar variables en él. Para asignar valores a las variables, se utiliza simplemente el operador de asignación, es decir el signo de igual (=), por ejemplo, var = 1.
4. También es posible utilizar operadores de asignación compuesta (operadores abreviados) para modificar los valores asignados a las variables, por ejemplo: var += 1, o var /= 5 * 2.
5. Se les puede asignar valores nuevos a variables ya existentes utilizando el operador de asignación o un operador abreviado, por ejemplo:
	`var = 2`
	`print(var)
	`var = 3
	`print(var)
	`var += 1
	`print(var)
6. Puedes combinar texto y variables usando el operador + y emplear la función print() para generar cadenas y variables, por ejemplo:
	`var = "007"
	print("Agent " + var)

Lección 5
1. Los comentarios pueden ser utilizados para colocar información adicional en el código. Son omitidos al momento de la ejecución. Dicha información es para los lectores que están manipulando el código. En Python, un comentario es un fragmento de texto que comienza con un #. El comentario se extiende hasta el final de la línea.
2. Si deseas colocar un comentario que abarque varias líneas, es necesario colocar un # al inicio de cada línea. Además, se puede utilizar un comentario para marcar un fragmento de código que no es necesario en el momento y no se desea ejecutar. (observa la última línea de código del siguiente fragmento), por ejemplo:
	`# Este programa imprime
	 `# una introducción en la pantalla.`
	`print("¡Hola!")  #Invocando a la función print()`
	`# print("Soy Python.")`
3. Cuando sea posible, se deben auto comentar los nombres de las variables, por ejemplo, si se están utilizando dos variables para almacenar la altura y longitud de algo, los nombres length y width son una mejor elección que myvar1 y myvar2.
4. Es importante utilizar los comentarios para que los programas sean más fáciles de entender, además de emplear variables legibles y significativas en el código. Sin embargo, es igualmente importante no utilizar nombres de variables que sean confusos, o dejar comentarios que contengan información incorrecta.
5. Los comentarios pueden ser muy útiles cuando tú estás leyendo tu propio código después de un tiempo (es común que los desarrolladores olviden lo que su propio código hace), y cuando otros están leyendo tu código (les puede ayudar a comprender que es lo que hacen tus programas y como es que lo hacen).

Lección 6
1. La función print() **envía datos a la consola**, mientras que la función input() **obtiene datos de la consola**.
2. La función input() viene con un parámetro opcional: **la cadena de mensaje**. Te permite escribir un mensaje antes de que el usuario ingrese algo, por ejemplo:
	`name = input("Ingresa tu nombre: ")
	`print("Hola, " + name + ". ¡Un gusto conocerte!")`
3. Cuando la función input() es llamada o invocada, el flujo del programa se detiene, el símbolo del cursor se mantiene parpadeando (le está indicando al usuario que tome acción ya que la consola está en modo de entrada) hasta que el usuario haya ingresado un dato y/o haya presionado la tecla _Enter_.
		Puedes probar la funcionalidad completa de la función input() localmente en tu máquina. Por razones de optimización, se ha limitado el máximo número de ejecuciones en Edube a solo algunos segundos únicamente. Ve a Sandbox, copia-pega el código que está arriba, ejecuta el programa, y espera unos segundos. Tu programa debe detenerse después de unos segundos. Ahora abre IDLE, y ejecuta el mismo programa ahí -¿Puedes notar alguna diferencia?
		Tip: la característica mencionada anteriormente de la función input() puede ser utilizada para pedirle al usuario que termine o finalice el programa. Observa el siguiente código: 
			`name = input("Ingresa tu nombre: ")`
			`print("Hola, " + name + ". '¡Gusto en conocerte'!")`
			`print("\nPresiona Enter para terminar el programa.")`
			`input()`
			`print("FIN.")`
 4. El resultado de la función input() es una cadena. Se pueden unir cadenas unas con otras a través del operador de concatenación (+). Observa el siguiente código:
	`num_1 = input("Ingresa el primer número: ") # Ingresa 12`
	`num_2 = input("Ingresa el segundo número: ") # Ingresa 21`
	`print(num_1 + num_2) # El programa retorna 1221`
5. También se pueden multiplicar (* - replicación) cadenas, por ejemplo:
	`my_input = input("Ingresa algo: ") # Entrada de ejemplo: hola`
	`print(my_input * 3) # Salida Esperada: holahola`



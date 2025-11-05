**Definición de computadora:** Máquina que procesa datos de entrada, los transforma y genera información de salida. 
	Componentes mínimos: 
		**- Unidad de procesamiento central (CPU).**
		**- Unidad de memoria.**
		**- Periféricos de entrada/salida.**
Las computadoras no solo son equipos tradicionales(PCs, laptops), sino también dispositivos integrados en diversos sistemas (ej.: teléfonos inteligentes, relojes inteligentes y servidores también son técnicamente computadores.).

Breve repaso de la historia.
- **Ábaco:** El primer dispositivo para contar, originario de Mesopotamía alrededor del año 3000 A.C..
- **Pascalina:** COnsiderada la primera máquina para calcular, creada en 1642 por Blaise Pascal. 
- **ENIAC:** La primera computadora electrónica de propósito general, que surgió en 1945. A pesar de su tamaño y complejidad, fue un hito que inspiró a John Von Neumann, quien creó la bases de la computadoras modernas. 

**Introducción a la Arquitectura de Von Neumann**
Antes de 1945, las computadoras eran limitadas y requerían cambios físicos para reprogramarse. En 1945, John Von Neumann propuso un modelo que almacena datos e instrucciones en la misma memoria, permitiendo reprogramación fácil y rápida. Este diseño sigue siendo fundamental hoy.

**Componentes de la Arquitectura de Von Neumann**
La arquitectura incluye tres elementos principales conectados por buses:
- **CPU**: Ejecuta instrucciones y realiza cálculos.
- **Memoria Principal**: Guarda datos e instrucciones en celdas con direcciones únicas.
- **Dispositivos de E/S**: Facilitan la interacción con el usuario (ej. teclado, monitor).
Los buses trasladan datos, direcciones y señales entre componentes.

**Instrucciones**
Las instrucciones son secuencias de bits que indican operaciones, datos y dónde almacenar resultados. Cada computadora tiene un juego de instrucciones específico, como sumar o comparar.

**Unidad de Procesamiento Central (CPU)**
La CPU ejecuta instrucciones mediante:
- **ALU**: Realiza operaciones matemáticas y lógicas.
- **Unidad de Control**: Coordina los componentes.
- **Registros**: Almacenan datos temporales.
Puede procesar 32 o 64 bits por operación, afectando el rendimiento.

**Memoria Principal**
Almacena datos e instrucciones en celdas de tamaño fijo (ej. 32 o 64 bits), accesibles por direcciones únicas. El acceso puede ser por palabras o bytes.

**Dispositivos de Entrada y Salida**
Conectados por buses, permiten interacción externa (ej. teclado para entrada, pantalla para salida). Los controladores gestionan su funcionamiento.

**Evolución de la Arquitectura de Von Neumann**
Mejoras incluyen:
- **Multi-Núcleo**: Varios procesadores en una CPU.
- **Memoria Caché**: Almacena datos frecuentes para acceso rápido.
- **Computación Heterogénea**: Combina CPU y GPU para eficiencia.

**El Futuro de la Arquitectura de Computación**
Nuevas tecnologías emergentes:
- **Computación Cuántica**: Usa qubits para cálculos rápidos.
- **Arquitectura Neuromórfica**: Imita el cerebro para inteligencia artificial.
- **Memoria Persistente**: Almacena datos sin energía.
- **Edge Computing**: Procesa datos localmente.

**Componentes Principales de la CPU**
La CPU se compone de tres elementos fundamentales:

**Unidad Aritmético Lógica (ALU)**
    - Es un circuito digital que realiza operaciones aritméticas (suma, resta, multiplicación, división) y lógicas (OR, AND, NOT, XOR).
    - Trabaja con una cantidad fija de bits, determinada por el tamaño de la palabra del CPU.
    - Puede operar de tres formas según la ubicación de los operandos (datos):
        - **Registro-Registro**: Ambos operandos están en registros de la CPU (acceso rápido).
        - **Registro-Memoria**: Un operando en un registro y otro en la memoria principal.
        - **Memoria-Memoria**: Ambos operandos en la memoria principal.
    - Nota: Generalmente, la ALU trabaja con dos operandos a la vez.
**Unidad de Control (UC)**
    - Lee instrucciones de la memoria principal de forma síncrona con el **reloj de la CPU**.
    - Genera señales de control para ejecutar las instrucciones y las decodifica para coordinar otros componentes.
    - **Reloj de la CPU**: Un oscilador electrónico que genera una señal periódica para sincronizar operaciones.
        - **Frecuencia del reloj**: Medida en Hz, MHz o GHz (ejemplo: 3 GHz = 3 mil millones de ciclos por segundo).
        - **Duración del ciclo**: Inverso de la frecuencia (ejemplo: 0.33 nanosegundos para 3 GHz).
    - Cada operación puede requerir uno o más **ciclos de reloj**.
 **Registros**
    - Memorias pequeñas y rápidas que almacenan datos e instrucciones temporales. Se dividen en tres tipos:
        - **Registros de propósito general**: Para cualquier dato o instrucción, útiles para programadores.
        - **Registros de propósito específico**: Reservados para información clave de la CPU, como:
            - **Contador de programa (PC)**: Dirección de la siguiente instrucción a ejecutar.
            - **Registro de estado (SR)**: Almacena el estado de la última operación de la ALU (flags).
            - **Puntero de pila (SP)**: Dirección de la cima de la pila en memoria.
        - **Registros transparentes**: Usados solo por la CPU, no accesibles por programadores:
            - **Registro de instrucción (IR)**: Instrucción actual en decodificación.
            - **Registro de direcciones (AR)**: Dirección de memoria a acceder.
            - **Registro de datos (DR)**: Datos a leer o escribir en memoria.
Flujo de Procesamiento de Información
El procesamiento de instrucciones sigue un ciclo de cinco etapas, que generalmente se completa en un ciclo de reloj:
 **Captura (Fetch)**
    - La UC obtiene la siguiente instrucción de la memoria usando el PC y la carga en el IR.
 **Decodificación (Decode)**
    - La UC analiza la instrucción en el IR para identificar la operación y los datos requeridos.
 **Obtención de operandos (Fetch Operands)**
    - Si la instrucción necesita operandos, se obtienen de registros o memoria.
**Ejecución (Execution)**
    - La ALU realiza la operación con los operandos y almacena los resultados temporalmente en registros.
**Escritura de resultados (Write Back)**
    - Los resultados se escriben en registros o memoria, y se actualizan el PC y el SR.
Este ciclo se repite hasta completar el programa, asegurando un procesamiento ordenado y eficiente.
## Principios de Comunicación
**Título del Módulo:** Principios de Comunicación
**Objetivos del módulo:** Explicar la importancia de los estándares y protocolos en las comunicaciones de red. 


| Título del Tema                    | Objetivo del Tema                                   |
| ---------------------------------- | --------------------------------------------------- |
| Protocolo de <br>comunicación      | Describir los protocolos de comunicación de red.    |
| Estándares de <br>comunicación     | Describir los estándares de comunicación de la red. |
| Modelos de <br>comunicación de red | Comparar los modelos OSI y TCP/IP.                  |
### Protocolo de comunicación
Los protocolos son necesarios para que las computadoras se comuniquen correctamente a través de la red. Estos incluyen el formato del mensaje, el tamaño del mensaje, el tiempo, la codificación, la encapsulación y los patrones del mensaje. 
* **Formato del mensaje** Cuando se envía un mensaje, debe usar un formato o estructura específica.
* **Tamaño del mensaje** Las reglas que rigen el tamaño de las piezas comunicadas a través de la red son muy estrictas. También pueden ser diferentes, de acuerdo con el canal utilizado. 
* **Sincronización** La sincronización determina la velocidad a la que se transmiten los bits a través de la red. También afecta cuándo un host individual puede enviar datos y la cantidad total de datos que se pueden enviar en una transmisión dada. 
* **Codificación** El host de envío convierte primero los mensajes enviados a través de la red en bits. Cada bit se codifica en un patrón de sonidos, ondas de luz o impulsos electrónicos, según el medio de red a través del cual se transmitan los bits. 
* **Encapsulación** Cada mensaje transmitido en una red debe incluir un encabezado que contenga información de direccionamiento que identifique los hosts de origen y destino. La encapsulación es el proceso de agregar esta información a los elementos de datos que conforman el mensaje. 
* **Patrón de mensaje** Algunos mensajes requieren una confirmación antes de que se pueda enviar el siguiente mensaje. Este tipo de patrón de solicitud y respuesta es un aspecto común de muchos protocolos de red. Sin embargo, hay otros tipos de mensajes que pueden simplemente transmitirse a través de la red, sin preocuparse de si llegan a su destino. 
### Estándares de comunicación
Las topologías nos permiten ver la red mediante la representación de dispositivos finales y dispositivos intermediarios. ¿Cómo ve una red un dispositivo? Piense en un dispositivo en una burbuja, Lo único que ve un dispositivo es su propia información de direccionamiento. ¿Cómo sabe el dispositivo que está en la misma red que otro dispositivo? La respuesta son los protocolos de red. La mayoría de las comunicaciones de red se divide en unidades de datos o paquetes más pequeños.
Un estándar es un conjunto de reglas que determina cómo se realiza algo. Los estándares de red e Internet aseguran que todos los dispositivos que se conectan a la red implementen el mismo conjunto de reglas o protocolos del mismo modo. Usando estándares, es posibles que diferentes tipos de dispositivos se envíen información entre sí a través de Internet.
Un estándar de Internet es el resultado final de un ciclo completo de discusión, resolución de problemas y pruebas. Estos diferentes estándares son desarrollados, publicados y mantenidos por una variedad de organizaciones. Cuando se propone un nueva estándar, cada etapa del desarrollo y del proceso de aprobación es registrada en un documento numerado de Solicitud de Comentarios (RFC, Reques for Comments) para seguir la evolución del estándar. Las RFC para los estándar de Internet son publicadas y administradas por el Grupo de Trabajo de Ingeniería de Internet (IETF)
### Modelos de comunicación de Red
Los protocolos son reglas que rigen las comunicaciones. La comunicación correcta entre hosts requiere la interacción entre una serie de protocolos. Los protocolos incluyen HTTP, TCP, IP y Ethernet. Estos protocolos se implementan en el software y el hardware que están instalados en cada host y dispositivos de red. 
La interacción entro los diferentes protocolos en un dispositivo se puede ilustrar como una pila de protocolos. En un pila se ilustran los protocolos como una jerarquía en capas, donde cada protocolo de nivel superior depende de los servicios de los protocolos que aparecen en los niveles inferiores. La separación de funciones permite que cada capa de la pila funcione independientemente de las otras capas.
El conjunto de protocolos TCP/IP que se utilizan para las comunicaciones por Internet sigue la estructura de este modelo
+ **Aplicación** Representa datos para usuario, además de codificación y control de diálogo.
+ **Transporte** Admite la comunicación entre varios dispositivos a través de diversas redes.
+ **Internet** Determina la mejor ruta a través de la red.
+ **Acceso a la red** Los dispositivos de hardware y los medios que componen la red.
Un modelo de referencia describe las funciones que se deben completar en una capa en particular, peo no especifica exactamente cómo se debe lograr una función. El objetivo principal de un modelo de referencia es ayudar a comprender mejor las funciones y los procesos necesarios para las comunicaciones de red.
El modelo de referencia entre redes más conocido fue creado por el proyecto OSI en la ISO internacional. Se usa para diseño de redes de datos, especificaciones de funcionamiento y resolución de problemas. Este modelo se conoce comúnmente como el modelo OSI
### Descripción de la capa del modelo OSI
* **7 - Aplicación** La capa de aplicación contiene protocolos que su utilizan para las comunicaciones de proceso a proceso.
* **6 - Presentación** La capa de presentación proporciona una representación común de los datos transferidos entre los servicios de la capa de aplicación.
* **5 - Sesión** La capa de sesión proporciona servicios a la capa de presentación para organizar su diálogo y gestionar el intercambio de datos.
* **4 - Transporte** La capa de transporte define los servicios para segmentar, transferir y volver a ensamblar los datos para las comunicaciones individuales entre los dispositivos finales.
* **3 - Red** La capa de red proporciona servicios para intercambiar datos individuales a través de la red entre dispositivos finales identificados. 
* **2 - Enlace de datos** Los protocolos de la capa de enlace de datos describen métodos para intercambiar tramas de datos entre dispositivos a través de un medio común.
* **1 - Físico** Los protocolos de la capa física describen los medios mecánicos, eléctricos, funcionales y de procedimiento para activar, mantener y desactivar conexiones físicas para la transmisión de bits y desde un dispositivo de red. 
## Medios de Red
**Título del módulo:** Medios de red
**Objetivo del módulo:** Describir los medios de red comunes

| Título del tema           | Objetivo del Tema                             |
| ------------------------- | --------------------------------------------- |
| Tipos de Medios de<br>Red | Describir los tipos comunes de cables de red. |
### Tipos de medios de red 
La comunicación se transmite a través de una red en los medios. El medio proporciona el canal por el cual viaja el mensaje desde el origen hasta el destino. 
Las redes modernas utilizan principalmente tres tipos de medios para interconectar dispositivos: 
+ **Hilos metálicos dentro de cables:** Los datos se codifican en impulsos eléctricos.
+ **Fibra de vidrio o plástico (cables de fibra óptica):** Los datos se codifican como pulsos de luz.
+ **Transmisión inalámbricas:** Los datos so codifican a través de la modulación de frecuencias especificas de ondas electromagnéticas. 
Los cuatros criterios principales para elegir los medios son los siguientes: 
* ¿Cuál es la distancia máxima en la que el medio puede transportar una señal exitosamente?
* ¿Cuál es el entorno en el que se instalarán los medios?
* ¿Cuál es la cantidad de datos y a qué velocidad se deben transmitir?
* ¿Cuál es el costo de la instalación de los medios?
Los tres cables de red más comunes son el cable coaxial, el cable de par trenzado y el cable de fibra óptica. La tecnología Ethernet generalmente usa cables de par trenzado para interconectar dispositivos. El cable coaxial es como es como los cables de cobre que utilizan la compañías de TV. También se utilizan para conectar los diversos componentes que forman los sistemas de comunicación satelitales. El cable de fibra óptica puede ser de vidrio o de plástico con un diámetro similar al de un cabello humano y puede transmitir información digital a velocidades muy rápidas a través de grandes distancias. Dado que usan luz en lugar de electricidad, la interferencia eléctrica no afecta la señal. 
## La Capa de Acceso
Título de módulo: Capa de Acceso
Objetivo del módulo: Explicar cómo se produce la comunicación en las redes Ethernet.

| Título del tema                         | Objetivos del tema                                                    |
| --------------------------------------- | --------------------------------------------------------------------- |
| Encapsulación y la<br>Trama de Ethernet | Explicar el proceso de encapsulación y la trama de Ethernet.          |
| La Capa de Acceso                       | Explicar cómo mejorar la comunicación de la red en la capa de acceso. |
### Encapsulación y la Trama de Ethernet
El proceso que consiste en colocar un mensaje dentro de otro formato de mensaje se denomina encapsulamiento. Cuando el destinatario revierte este proceso y quita la carta del sobre se produce la desencapsulación del mensaje. De la misma manera en la que una carta se encapsula en un sobre para la entrega, los mensajes de las computadoras también deben encapsularse. Un mensaje que se envía a través de una red de computadoras sigue reglas de formato específicas para que pueda ser entregado y procesado. 
Los estándares del protocolo Ethernet definen muchos aspectos de la comunicación de red, incluido el formato, el tamaño, la temporización y la codificación de las tramas. EL formato para las tramas de Ethernet especifica la ubicación de las direcciones MAC de origen y de destino, e información adicional, incluido el preámbulo para la secuencia y la temporización, el delimitador de inicio de trama, la longitud y el tipo de trama, y la secuencia de verificación de tramas para detectar errores de transmisión. 
### La Capa de Acceso
La capa de acceso es la parte de la red que permite a las personas obtener acceso a otros hosts y a archivos e impresoras compartidos. La capa de acceso proporciona la primera línea de dispositivos de red que conectan hosts a la red Ethernet cableada. dentro de una red Ethernet, cada hosts puede conectarse directamente a un dispositivo de red de capa de acceso mediante un cable Ethernet. Los concentradores Ethernet tienen varios puertos que se utilizan para conectar hosts a la red. Solo es posible enviar un mensaje a la vez a un  concentrador Ethernet. Dos o más mensajes enviados al mismo tiempo provocarán una colisión. Como el exceso de retransmisiones puede congestionar la red y reducir la velocidad del tráfico de red, ahora los concentradores se consideran obsoletos y fueron reemplazados por conmutadores Ethernet.  
Un switch Ethernet es un dispositivo que se utiliza en la capa 2. Cuando un host envía un mensaje a otro host conectado a la misma red conmutada, el conmutador acepta y decodifica las trama para leer la parte de la dirección MAC del mensaje. Una tabla switch, llamada tabla de direcciones MAC, contiene una lista de todos los puertos activos y las direcciones MAC del host que se adjunta a ellos. Cuando se envía un mensaje entre hosts, el conmutador verifica si la dirección MAC de destino está en la tabla. Si está, el conmutador Ethernet también permiten enviar y recibir tramas a través del mismo cable Ethernet simultáneamente. Esto mejora el rendimiento de la red porque elimina las colisiones. 
Para crear la tabla de direcciones MAC, los conmutadores examinan la dirección MAC de origen de cada trama que se envía entre los hosts. Cuando un host envía un mensaje o responde a un mensaje enviado por inundación, el conmutador inmediatamente aprende la dirección MAC de este host y el puerto al que está conectado. La tabla se actualiza de manera dinámica cada vez que el conmutador lee una nueva dirección MAC de origen. 
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
* **1 - Físico** Los protocolos de la capa física describen los medios mecánicos, eléctricos, funcionales y de procedimiento para activar, mantener y desctivar conexiones físicas para la transmisión de bits y desde un dispositivo de red. 
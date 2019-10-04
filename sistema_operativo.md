# Sistema Operativo. 

## Definición. 
Un Sistema Operativo es un programa o conjutno de programas que actúa como intermediario entre el usuario y el hardware del ordenador, gestionando los recursos del sistema y optimizando su uso. Cuando encendemos un ordenador, se carga parte del sistema operativo, y él es que el "despierta" el ordenador, reconociendo sus periféricos y verificando que no exitan errores (a este primer diagnóstico se denomina POST). 
Despues de esto, se encarga de presentar al usuario una forma fácil de manejar y programar el hardware que está por debajo, abstrayendonos de muchas tareas, como por ejemplo, como tenemos que poner los datos en un disco para organizarnos

## Funciones del Sistema Operativo: 
- Control de la ejecución de los programas. Para ello acepta los trabajos, les asigna recursos, y administra la forma en la que se realizan. 
- Administración de periféricos. Coordinando y administrando los dispositivos conectados al ordenador. 
- Gestión de permisos y usuarios. 
- Control de Concurrencia. Establece prioridades cuando varios procesos solicitan acceso a los mismos recursos. 
- Control de errores. Gestiona los errores de hardware y la pérdida de datos. 
- Administración de la memoria. Asigna memoria a los procesos y  gestiona su uso. 
- Control de seguridad. Debe proporcionar seguridad tanto para los usuarios como para el software y la información almacenada en los sistemas. 

En concordancia con estas funciones, es posible analizar la estructura de un sistema operativo en 5 niveles, de los cuales los dos primeros entrarían dentro de la parte del sistema operativo dependiente del hardware y el resto de la parte portable del mismo. 
- Nivel 1 - Gestión del Procesador. En los sistemas operativos multiproceso, este nivel se encarga de compartir la CPU entre los diferentes procesos realizando tareas de sincronización entre procesos, conmutación de la CPU y gestión de interrumpciones. 
- Nivel 2 - Gestión de Memoria. Se distrubuye la memoria entre los procesos y se realizan tareas de asignación y liberación de memoria, así como control de acceso no permitido a zonas de memoria. 
- Nivel 3 - Gestión de Procesos. Este nivel se encarga de la creación y destrucción de procesos, intercambio de mensajes y detección y arranque de los mismos. 
- Nivel 4 - Gestión de Dispositivos. Gestión de las entradas y salidas en función de los dispositivos conectados. 
- Nivel 5 - Gestión de la Información. En este nivel se realizan tareas como simplificar el acceso a los recursos, apertura y cierre de ficheros, lectura y escritura de ficheros, ...

## Elementos constitutivos. 

El núcleo. / Manejo de procesos

Administrador de memoria. 

Sistema de Entrada/Salida

Administrador de archivos. 

Proporcionar interfaz al usuario


## Clasificaciones. 

Existen varias formas de clasificar los sitemas operativos, atendiendo a varios criterios: 
Si atendemos al número de usuarios, tenemos sistema monousuario y sistemas multiusuario en función en fucnión de si permiten trabajar a más de un usuario a la vez. Si atendemos al número de tareas, tenemos sistemas monotarea, y sisteams multitarea, y por último, si atendemos al número de procesadores que tiene la máquina donde se ejecuta el sistema operativo, tenemos sistemas monoproceso ( un solo procesador, aunque se puede simular multitarea) y sistemas multiproceso. En estos últimos tenemos sistemas simétricos, donde si tenemmos 3 procesadores y 3 procesos, cada procesador se encargará de un proceso, y sistemas asimétricos donde podemos por ejemplo cargar un proceso pesado sobre un procesador y todos los demás procesos repartirlos en los otros dos, o otros esquemas. 

Si atendemos a la forma en la que ofrecen los servicios, tenemos tres tipos de sistemas operativos: 
### Sistemas centralizados. 
Existe un gran ordenador central que lleva a cabo toda la capacidad de proceso y luego múltiples terminales tontos que se conectan a él, y que son los que utilizan los usuarios. Fué un sistema bastante utilizado hasta que los microordenadores fueron basantante potentes. 

### Sistemas en red. 
En este tipod e sistemas, tenemos dos o más ordenadores conectados o red con ta intención de compartir ciertos recursos. Casa elemento tiene su propio sistema operativo, sus propios archivos locales, etc. 

### Sistemas distribuídos. 
Tenemos un conjuntod e procesadores, cada uno con su memoria, que pueden estar en el mismo equipo o en equipos diferentes. El sistema operativo se encarga de asignar procesos a nodos y todo de forma transparente para el usuario. 
Sprite, Solaris-MC, Mach, Chorus, Spring, Amoeba, Taos, 




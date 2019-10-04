# Tipos de Datos Abstractos
¿Que es un tipo de datos?

Un tipo abstracto de datos es un tipo definido por el programador que se puede maniputar de un modo similar a los tipos predefinidos por el sistema. De una forma similar a los tipos del sistema tienen conjunto de valores y una serie de operaciones que podemos realizar sobre esos valores. Los usuarios pueden crear variables con los valores que están en el rango definido por ese tipo de datos, y operar con sus métodos. 
El estado de un TDA viene dato por la secuencia de operaciones realizadas sobre él. 

Entre sus características nos encontramos: 
- Encapsulamiento. Se desconoce como está implementado. 
- Protección. Sólo es posible acceder al TAD a través de las operaciones del mismo
- Abstracción. 


# Ficheros 
## Concepto de archivo. 
Un archivo o fichero es un conjunto de información, que tiene una relación lógica entre si y que se encuentra almacenada en un medio de soporte durable. 
Desde el punto de vista de un Sistema Operativo, el archivo es la univdad lógica de organización de los datos en un dispositivo de almacenamiento. 
Todo archivo tiene un nombre, y dentro del dispositivo se encuentran organizados en carpetas. No puede haber dos archivos con el mismo nombre dentro de una misma carpeta. Las carpetas pueden contener un número arbitrario de archivos, y a su vez otras carpetas, creando así estructuras jerárquicas, que pueden llegar a ser muy profundas. 
Al igual que los archivos, las carpetas tienen un nombre, que debería identificar el contenido de la misma. Una excepción a la carpeta con nombre puede ser la carpeta raíz del sistema, que habitualmente no tiene nombre, o éste está fijado.
En muchos sistemas operativos, los nombres del los archivos incorporan una extensión, que es un conjunto pequeño de letras (3 o 4) despues de un punto, que le indican al sistema y al usuario que tipo de información se almacena en ese archivo, y por lo tanto con que programa lo podemos abrir. Por ejemplo, un fichero de texto podría tener como extensión .txt, si tenemos un archivo de word tendríamos .docx, .jpg ciertos ficheros de imágen, .... A veces, los Sistemas Operativos esconden esta extensión, y la forma de reconocer el archivo es mediante el icono asociado, el cual a menudo se pode en función de la extensión. 

En un primer sistema de clasificación, podríamos diferenciar entre ficheros de texto, y ficheros binarios. Los ficheros de texto contienen líneas de texto en codificación ASCII, y se pueden abrir con un un simple editor de texto presente en cualquier sistema operativo y en cuaquier arquitectura. Es un tipo de archivo más común de lo que parece a priori, puesto que muchos tipos de ficheros (segun extensión com vimos antes), en realidad son ficheros de texto con una forma de escribir los datos que estructure la infomración, es el caso de los documentos .html de las páginas web, en general de muchos sistemas para intercambiar información como xml, json, yaml, ...
Los archivos binarios por otro lado, almacenan bit's, de los que a priori no sabríamos  interpretar salvo que utilicemos el programa adecuado. Podemos encontrar ejemplos como los .jpg, .png o .gif de imágen, los .mpg de vídeo, los .doc de word o los mismos ficheros ejecutables. 

## Organización.
Continuando con lo anterior, podemos considerar que un fichero internamente se estructura lógicamente en registros, es decir, que un fichero está compuesto de registros, pudiendo ser estos de tamaño fijo o de tamaño variable. Un fichero de texto bajo este paradigma puede ser un fichero de registros donde cada registro es una línea, que tiene tamaño variable, puesto que quien indica cuando finaliza la línea es un caracter especial de salto de línea. 
Por otro lado, los dispositivos de almacenamiento se orgamizan de otra formas. Por ejemplo, los discos se organizan en bloques, siendo un bloque la unidad mínima que un disco es capaz de leer o escribir. 
Con todo esto, cuando nosotros tenemos un registro de un fichero, éste tiene 2 direcciones. Por un lado la dirección lógica del registro, que indica la posición relativa de ese registro dentro del fichero, y por otro la dirección física, que es la dirección dentro del dispositivo donde está almacenado. El Sistema Operativo tiene que ser capaz de hacer traducciones entre estas dos direcciones, para poder acceder a los datos. 
La organmización de un fichero, define **la relación estre la dirección lógica y la dirección física**. 
Nos encontramos con las siguienres formas de organización: 

- Organización secuencial: Los registros se graban uno detras de otro, sin dejar huecos. La correspondencia entre direcciones es total. Con ella se aprovecha al máximo el soporte, el acceso secuencial es muy rápido. Sin embargo las operaciones de inserción de registros pueden ser difíciles o directamente imposibles. 
- Organización secuencial encadenada: Es una variante de la anterior, y necesita de dispositivos direccionables. En ella, cada registro almacena un puntero a la dirección del siguiente registro según su órden lógico. Las inserciones se graban al final del fichero, y los borrados son posibles, pero permanecen en el disco (habbría que compactar). 
- Organizacón indexada: Solo para dispositivos direccionables. Cada registro se identifica unívocamente mediante una clave formada un un campo o combinación de campos. Se mantiene un índice y los datos. Es posible la inserción modificiación, etc. No se puede modificar el campo clave. 
- Organización secuencial indexada: Los ficheros constan de 3 áreas, un área primaria donde se encuentren los registros ordenados secuencialmente por valor de la clave, un área de índices con las direcciones y un área de desbordamiento utilizado para añadir nuevos registros cuando no pueden ser colocados en el área primaria. El área primaria y el área de índices están ordenados por clave. Solo se puede insertar al final del área de desbordamiento y en esa zona está desordanada pero la gestión del desbordamiento es compleja y hace necesaria una reorganización periódica de los ficheros. 
- Orgamización secuencial indexada encadenada. Es una variante de la anterior. Utiliza puntero e índices a la vez. Las adiciones se realizan en el área de desbordamiento ya que no se pueden añadir en el área primaria. Requieren organización, sino con el tiempo el área de desbordamiento es tan grande que se comporta como secuencial
- Organización directa: Cada registro se almacena en una dirección que depende del valor de su clave. La relación entre clave y dirección la establece el programador y el acceso se hace indicando la dirección relativa dentro del fichero. El sistema operativo no nos avisa de posibles errores en el cálculo de la dirección. El direccionamiento puede ser: 
    - Directo. la dirección es la propia clave. pero desperdicia muchísimo espacio
    - Aleatorio. En este caso, la dirección se calcula mediante una función matematica. Esa función debe dispersar los datos de forma aleatoria y uniforme, intentando minimizar las colisiones


















En los soportes, los tenemos de dos tipos, de acceso aleatorio, que son los más utilizados y de acceso secuencial, que se usaban sobre todo para copias de seguridad
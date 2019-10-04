# Programación Orientada a Objetos

## Guión

- Que es la programación orietnada a objetos
- Paradigma
- Objeto, clase, atributo, método. 
- Propiedades: encapsulación, abstracción, herencia, polimorfismo. 


# Programación Orientada a Objetos ?

La programación orientada a objetos en un paradigma de programación que surge a partir de la programación estructurada, pero que aporta una nueva forma de enfrentarse a un problema a la hora de programar una solución software. 

La programación estructurada se enfrenta a la complejidad de un problema descomponiendolo en problemas más pequeños, y estos problemas más pequeños en otros todavía más pequeños hasta que tengamos acciones simples y fáciles de programas. Aún así, pronto se dan cuenta de algunas limitaciones y se programa intentando tener propiedaes deseables como cada vez más abstracción o la encapsulación (veremos más adelante). 

La programación orientada a objetos ofrece un punto de vista diferente. La POO trata de entender el problema, y modelar el mundo real en estructuras más refinadas llamadas objetos. 

Un objeto es la representación en un programa de un concepto y contiene toda la lógica necesaria para abstraerlo. Los objetos tienen dos partes importante, tienen un estado y tienen un comportamiento. El estado viene dado por los valores de unos atributos (cada objeto tiene valores concretos), y el comportamiento viene dado por el conjunto de operaciones que sabe realizar. Veámoslo con un ejemplo. 

Queremos modelar una academia que imparte cursos de formación. En la academia tenemos dos entes importantes que queremos modelar, por un lado los alumnos y por otro los profesores. De los alumnos nos interesará conocer una serie de atributos, provenientes del mundo real, y que son los que deseamos procesar en nuestro software, por ejemplo, el nombre del alumno, dni, su fecha de nacimiento, datos de contacto, los cursos que ha realizado, .... En cuando a las accioens que puede realizar, seguramente serían cosas como matricularse en un nuevo curso, abandonar una actividad, ...
Si hablamos de los objetos para los profesores, los atributos pueden ser diferentes nombre, dni, salario, materias, ...

Un concepto imporante es diferenciar entre clase y objeto. Hasta ahora hemos hablado de objetos, pero el objeto es un elemento concreto. Por ejemplo, el alumnos Luis, nacido 15/03/1995 matriculado en ingles. Pero antes de poder crear objetos tenemos que definir la platnilla que dice que atributos tienen los objetos de esta plantilla, y que acciones sabe realizar. A esta plantilla la llamamos clase. De esta forma, tenemos la clase Alumno, que define como son los objetos que pertenecen a esa clase. Los objetos son instancias, o casos concretos de una clase. 

El estado ya hemos dicho que es el conjunto de atributnos, y el comportamiento es el conjunto métodos que están programados (tienen mucha similitud con las funciones). 

Una propiedad muy deseable en la programación en la encapsulación. La encapsulación en uno de los  motivos principales por los que se desarrollan los tipos abstractos de datos, que ya aparecen en la programación estructurada. La encapsulación significa que los objetos (en este caso) deberían proteger sus atributos y su implementación interna y ofrecer una serie de métodos para relacionarse con otros objetos. Es muy deseable que un objeto pueda comunicarse con otro, pero que no sepa nada de como están implementadas las funconalidades internas, porque de este modo, los objetos pueden cambiar la forma de funcionar internamente, y los demás objetos ni se darán cuenta. En definitiva, la encapsulación es el ocultamiento del estado. 

Si volvemos a pensar en el ejemplo de antes, Profesores y Alumnos tenían características comunes, y otras diferentes. Esto es algo muy común en programación. Nos encontramos con entidades que se parecen mucho, pero que tienen ciertas sutilezas diferentes. En una programación más tradicional, las partes comunes las tenemos que repetir, lo cual hace las clases más pesadas, difíciles de programas etc. 
El mecanismo de herencia es algo que aprota la POO y que permite que podamos definir una clase, partiendo de otra ya existente. La clase nueva "hereda" todo el comportamiento de la ya existente, y puede añadir las características que son diferentes. 

Por último, otra caracteristica típica de la programación oritenda a objetos se llama polimorfismo. Es la propiedad de enviar mensajes sintácticamente iguales a objetos de tipos distintos
# Acesibilidad, diseño universal y usabilidad. 

## Accesibilidad
La accesibilidad, aplicada al mundo de la tecnología, hace referencia al acceso universal a un contenido electrónico, típicamente, una página web, independientemente del tipo de hardware, software, infraestructura de red, idioma ,localización geográfica o capacidad de los usuarios. 

Para poner en práctica la accesibilidad hay que tener presenta las Pautas de Accesibilidad al Contenido Web (WCAG) así como aplicar los Roles ARIA que se usan para hacer contenido accesible para las personas con diversidad funcional. 

## Usabilidad
La usablidad hace referencia a la facilidad de uso con que las personas pueden usar una herramienta en particual, en concreto podemos pensar también en una web. En hacer que el contenido sea fácil de utilizar. 
Tenemos un problema de usabilidad cuando: 
- Hay problemas para completar una tarea. 
- Se saca al usuario del camino
- Algo produce confusión en los usuarios. 
- Se producen errores. 
- Los cuandos no ven algo que deberían haber visto. 
- Los usuarios piensas que han finalizado una tarea y no es así 
- NO se entiende la navegación web. 
- Se tienen dar muchísimos clics para llegar al objetivo. 
- La página tarda mucho en cargarse. 

Beneficios de la usabilidad: 
- Se reduce el aprendizaje y el esfuerzo
- Disminuyen los costes de asistencia al usuario. 
- Optimización de los costes de diseño, rediseño y mantenimiento.
- Aumenta la tasa de conversión. 
- Para la usuarios es más fácil navegar. 
- Mejora el prestigio de la web y la imagen de marca. 
- Aumenta la velocidad de carga. 

Existen 5 reglas principales para la usabilidad web: 
- Rápido. Las páginas deben cargarse en una media de 4 segundos.
- Simple. Mantener una navegación simple. No forzar a aprender diversos caminos o esquemas de navegación. 
- Investigable. Los motores de búsqueda buscan texto real, no prestan atención a animaciones o gráficos
- Para la mayoría. El código debe ser compatible con todos los navegadores. Utilizar HTML estándar. 
- Mantener actualizado

En la actualidad hay que destacar que por ejemplo en web, gran parte de los usuarios nos visitarán desde dispositivos móviles. Es muy importante considerar la usabilidad cuando nos visitan con estos dispositivos. 

## Diseño universal. 
Es un concepto relativamente reciente y tiene que ver con el diseño de productos y entornos que resulten de fácil acceso para el mayor número de personas posible, sin necesidad de adaptarlos o rediseñarlos de forma especial. Es un término más global que engloba la accesibilidad

## Pautas de Accesibilidad para el Contenido Web (WCAG)
Las pautas de accesibilidad para el contenido web son un conjunto de reglas, cuyo cumplimiento hace que nuestro sitio sea más accesible para las personas con diversidad funcional. Para que una página sea compatible con la normativa WCAG 2.1, se deben satisfacer todos los requisitos de conformidad: 
- Existen tres niveles de conformidad. Se debe cumplir con todos los requisitos de al menos un nivel. 
    - Nivel A: Requisitos básicos para que algunos usuarios puedan utilizar los contenidos web. 
    - Nivel AA: Mejor accesibilidad y eliminación de algunas barreras de acceso al contenido. 
    - Nivel AAA: Mejoras 
- Páginas completas. No se alcanza si partes de las páginas no cumplen. 
- Procesos completos. 
- Uso exclusivo. 
- Sin interferencias. 

Las pautas se pueden agrupar en cuatro principios
## Pautas: 
- Perceptible. 
- Operable. 
- Comprensible
- Robusto

![Pautas WCAG](accesibilidad_img/pautas.png "Pautas WCAG")

De forma resumida: 
1. Perceptible: 
    - Se proporcionan ayudas textuales a todo contenido no textual de modo que se puedan convertir a otros formatos que las personas necesiten. 
    - Se proporcionan alternativas para medios dependientes del tiempo (videos, sonidos, enlaces. )
    - Existe contenido que puede presentarse de diferente forma sin perder información o estructura
    - Se facilita a los usuarios ver y oír el contenido, incluyendo separación entre el primer plano y el fondo. 
2. Manejable: 
    - Se proporciona acceso a toda funcionalidad mediante el teclado. 
    - Se proporciona tiempo suficiente para leer y usar el contenido. 
    - No se diseña el conteido de forma que pueda provocar ataques, espasmos o convulsiones. 
    - Se proporcionan medios para ayudar a los usuarios a navegar, encontrar contenido y determinar donde se encuentran. 
3. Comprensible: 
    - Los contenidos textuales resultan fáciles de leer y comprender. 
    - Las páginas web aparecen y operan de forma predecible. 
    - Se ayuda a los usuarios a corregir los errores. 
4. Robusto: 
    - Se maximiza la compatiblidad con las aplicaciones de usuario actuales y futuras, incluyendo las ayudas técnicas. 


## Navegación accesible con roles WAI-ARIA
Se trata de hacerles la vida más fácil a usuarios que usan un lector de pantalla. Se trata de estructurar la navegación  a través del sitio web. 
Para orientarse a través de un sitio web, los usuarios que usan lector de pantallas van pulsando diferentes teclas para navegar por la web: ir saltando por encabezados, listas, ojear imágenes, etc. 

Ej, Para ojear los encabezados pueden ir pulsando la letra h. 

¿ Como saltar entre los diferntes bloques de contenido ?
Es decir, de la cabecera a la zonad e navegación, al contenido principal, al cuadro de búsqueda, al pié de página, etc. Las WCAG 2.0 establecieron la especificación WAI-ARIA que consistte en establecer unos roles que sirven para crear contenidos web accesibles. 

Añadir roles es muy sencillo, bastará con añadir a la etiqueta contenedora el atricuto role="[loquesea]"

Ejemplo: 
```html
    <div role="main"> ... </div>
```

Los landmark roles son:
- Banner: zona del título. Solo 1 por página
- Complementary: zona complementaria. por ejemplo artículos relacionados
- Contentinfo: zona de información sobre el documento. 
- Form
- Main. 
- Navigation
- Search
- Application (eliminado de los Landmark Roles en ARIA 1.1, que pasa a ser un rol de estructura)
- Region (añadido en los Landmark Roles en ARIA 1.1)

### Etiquetas Aria-label
Con ello ponemos una etiqueta dentro del elemento con un atributo

## Bibliografía
Web: https://www.mcarmendealba.com/accesibilidad-y-usabilidad-diferencias/
Web: https://olgacarreras.blogspot.com/
Web: http://accesibilidadweb.dlsi.ua.es/?menu=pautas-accesibilidad-contenido-web
Web: http://itakora.com
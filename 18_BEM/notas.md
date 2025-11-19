# BEM en CSS (Block Element modifier)

BEM, es una metodología que nos permite crear código CSS más organizado, flexible, modular y reutilizable, para lograr un código más limpio.
Todo esto gracias a su nomenclatura para nombrar las clases en nuestro HTML

## Ventajas de BEM

* Facilita trabajar con CSS3
* Evita los problemas con la cascada
* Evita los problemas con la especificidad
* Hace reutilizable nuestro código
* nos ahorra en pensar nombres al usar clases en CSS
* Fácil y rápido de entender
* Nos facilita el trabajo en equipo

BEM es una metodología que nos provee una manera de nombrar clases en HTML, empezando con bloques, siguiendo con elementos y terminando con modificadores.

## Block (Bloque)
Un bloque representa una entidad independiente. Eso significa que existe por sí misma y no necesita de otro elemento para existir, esto puede ser un formulario, un contenedor, un menú, un footer, un contenedor de galería, lo que sea que exista por si mismo.
**Ejemplo: navbar**

## Element (elemento)
Después, sigamos con element o elemento, un elemento representa a los elementos, valga la redundancia, dentro de un bloque. Con esto podemos decir que depende directamente de un bloque.
A diferencia de los bloques que no dependen de nadie, los elementos dependen del bloque, por ende, están dentro del bloque.
Estos pueden ser inputs dentro de un form, enlaces dentro de un navbar o imágenes dentro de un contenedor que es un contenedor gallery.

### Nombrar un elemento
Para definir a un elemento con la nomenclatura BEM, primero llevará el nombre del bloque padre, seguido de dos guiones bajos y el nombre del elemento.
**Ejemplo: navbar__link**

## Modifier (Modificador)
Un modificador representa una alteración a un bloque o a un elemento, un ejemplo es suponer que todos los enlaces tendrán un color negro, pero solamente uno tendrá un color rojo, en ese caso entraría un modificador para indicar que ese elemento tendrá otros estilos.
El modificador lleva el mismo nombre de la clase, pero se le agrega dos guiones medios seguido del nombre del modificador
**Ejemplo: navbar__item navbar__item--red**

### Definir un modificador

Para definir un modificador primero debe estar definida la clase del bloque o el elemento para posteriormente copiarla y pegarla, agregando dos guiones medios y el nombre de la modificación que deseas que tenga el elemento.
Ejemplo: `".container .container-steelblue"`
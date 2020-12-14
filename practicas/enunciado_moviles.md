# Práctica evaluable 4: Aplicaciones web en dispositivos móviles

El objetivo de esta práctica es adaptar la web de la práctica anterior a dispositivos móviles. Dependiendo de cómo hayas realizado la implementación podrás aprovechar más o menos directamente el código ya escrito. En general deberían valerte los mismos componentes aunque tendrás que reorganizarlos en pantalla y modificar su HTML y CSS.

Se propone usar [Ionic](https://ionicframework.com/) como framework de desarrollo, ya que permite usar componentes Vue, Angular o React pero si lo preferís podéis usar cualquier otro framework para móviles, como [onsen UI](https://onsen.io/) o [Quasar](https://quasar.dev/) o  usar simplemente componentes especialmente adaptados para móviles como [Bootstrap Vue](https://bootstrap-vue.org/). Cualquier otro del mismo estilo también os vale

> Antes de elegir un *framework* cualquiera echadle un vistazo a la popularidad de su repositorio de Github, la documentación disponible, la antigüedad de la última *release*, etc. Hay *frameworks* que ya no están mantenidos o bien que tienen poca documentación disponible, o solo en idiomas distintos del español o el inglés. 

## Requisitos mínimos

La implementación correcta de estos requisitos es necesaria para poder aprobar la práctica. Con estos requisitos podéis optar hasta un 6 si comentáis adecuadamente el código fuente, indicando la funcionalidad de las variables, de cada clase (si las usáis), de cada método/función (descripción de lo que hace, parámetros, valor de retorno,...).

**Los requisitos mínimos, desde el punto de vista meramente funcional, son los mismos que en la práctica anterior**, es decir:

- Login/logout
- Listado de datos con eliminación de items (similar al botón "x" de la lista de la compra)
- Creación de items

> Pongo "items" como término genérico porque cada uno estáis haciendo una aplicación distinta, en vuestro caso concreto serán "productos" o "usuarios" o "películas" o lo que proceda.

La diferencia es que **tenéis que organizar las funcionalidades de manera distinta en pantalla para adaptaros al móvil**:

- Cada funcionalidad debe aparecer en una pantalla distinta: login, listado, creación.
- En la medida de lo posible debéis usar controles y componentes de UI especialmente adaptados a móviles: por ejemplo no mostréis el listado con viñetas, como en HTML "de escritorio" sino con un componente "tabla" o "lista" del *framework*, en el que típicamente cada item ocupa todo el ancho de la pantalla (por ejemplo un [ion-list](https://ionicframework.com/docs/api/list) en Ionic o un [list](https://quasar.dev/vue-components/list-and-list-items) en Quasar). Intentad adaptar también los controles de formularios, botones, barras de menús, etc.

## Requisitos adicionales

Además de los 6 puntos de los requisitos mínimos, elegir de entre los siguientes:

- **Hasta 1 punto**: cachear la interfaz de la app con _service workers_, como se vio en clase de teoría la semana del 1 de diciembre. Podéis consultar [este tutorial de Google Web Fundamentals](https://developers.google.com/web/fundamentals/architecture/app-shell?hl=es) o alguno similar en la web buscando "PWA app shell".
- **Hasta 1 punto**: usar Firebase o alguna plataforma similar para implementar notificaciones *push*
- **Hasta 1 punto**: usar los APIs JS de captura de imágenes/video/audio para subir imágenes o videos al servidor. Podéis subirlos al servidor propio o a Firebase o alguna plataforma similar
- **Hasta 3 puntos**: usando el servidor mBaaS [Parse](https://github.com/parse-community/parse-server) implementar una lista de la compra como la que hicisteis en la práctica 2 con el *backend* en Parse. (No es necesario que lo hagáis todo, solo hasta donde queráis llegar) **Esto sería otra *app*, no está relacionado con la app que habéis desarrollado en las prácticas 1 y 3** (disculpad pero a estas alturas es complicado proponer funcionalidades alternativas a la práctica "grande" ya que cada uno habéis hecho cosas muy distintas).
    - Hasta 1 punto por instalar y configurar parse si se hace en un servidor local (se podría hacer en docker o en una empresa que lo ofrezca preconfigurado, pero esto no se podría valorar con 1 punto)
    - Hasta 1 punto por implementar el *backend* de la lista de la compra 
    - Hasta 1 punto por añadirle multiusuario: que cada usuario solo vea sus items, se puedan registrar usuarios en la aplicación y hacer login en ella

## Entrega

El plazo de entrega concluye el viernes **15 de enero de 2021** a las 23:59 horas. La entrega se realizará como es habitual a través de Moodle. Entregad una carpeta comprimida con el proyecto de esta práctica y el del servidor (modificado para usar CORS) en dos subcarpetas, ya que ambos son necesarios para ejecutar la aplicación. 

Entregad también un LEEME.txt donde expliquéis brevemente las partes optativas que habéis hecho y cualquier detalle que consideréis necesario.
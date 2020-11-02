# Práctica evaluable 3: Frameworks Javascript

El objetivo de esta práctica es desarrollar una web que sirva de cliente al API de la práctica 1, pero a diferencia de la práctica anterior, **en la implementación se debe usar un *framework* Javascript. Nosotros en clase hemos visto brevemente Vue pero si lo preferís podéis usar otros como React, Angular o algún otro similar**.

> Aclaración: librerías como jQuery no son *frameworks* de este estilo ya que simplemente vienen a facilitar ciertas tareas como el AJAX o la manipulación del DOM.


## Organización del código 

 - Usad una estructura de proyecto similar a la práctica anterior, con una carpeta `client` y una `server`
 - Necesitaréis modificar el servidor **para que use CORS**, como hicimos en el servidor de la lista de la compra
 - En el proyecto cliente tenéis 3 opciones:
   
     1. No usar ninguna herramienta adicional en el cliente, como hemos hecho esta semana en la práctica guiada
     2. Usar *parcel*, como hicimos la semana pasada. En la documentación se explica [cómo usarlo en conjunto con Vue](https://parceljs.org/vue.html), y también con otros frameworks (tendríais 0.25 puntos adicionales por hacerlo así)
     3. Usar `vue-cli` y *single file components* (tendríais 0.5 puntos adicionales por hacerlo así). En otros frameworks hay herramientas equivalentes (por ejemplo en React está `create-react-app`)

## Requisitos mínimos

La implementación correcta de estos requisitos es necesaria para poder aprobar la práctica. Con estos requisitos podéis optar hasta un 6 si comentáis adecuadamente el código fuente, indicando la funcionalidad de las variables, de cada clase (si las usáis), de cada método/función (descripción de lo que hace, parámetros, valor de retorno,...).

Debéis desarrollar una web en la que como mínimo se pueda hacer:

- Login/logout
- Listado de datos con eliminación de items (similar al botón "x" de la lista de la compra)
- Creación de items

> Pongo "items" como término genérico porque cada uno estáis haciendo una aplicación distinta, en vuestro caso concreto serán "productos" o "usuarios" o "películas" o lo que proceda.

## Requisitos adicionales

Además de los 6 puntos de los requisitos mínimos, elegir de entre los siguientes:

- hasta *0.5 puntos* si usáis la estructura de proyecto que genera la herramienta `vue-CLI` y *single file components* (podéis mirar su uso más detallado en la documentación):
    + [Instalación](https://cli.vuejs.org/guide/installation.html) de `vue-cli`
    + [Crear un proyecto](https://cli.vuejs.org/guide/creating-a-project.html)
    + [*Single file components*](https://es.vuejs.org/v2/guide/single-file-components.html)
- hasta *1 punto* si usáis algún *framework* de componentes visuales para Vue como [vuetify](https://vuetifyjs.com/en/) o [bootstrap-vue](https://bootstrap-vue.js.org)
- hasta *0.5 puntos*: implementar una funcionalidad de "ver detalles", al clicar en un item o en un botón asociado a cada item, se muestra más información sobre el item (sin cambiar de página)
- hasta *1 punto*: implementar el listado de otro recurso incluyendo también "ver detalles" y "eliminar".
- hasta *1 punto*: edición de datos: cada elemento del listado debería tener un botón o enlace "editar" para cambiar su contenido. Al pulsarlo aparecerá un formulario para escribir los nuevos datos. Dónde y cómo aparezca (y desaparezca al acabar la edición) queda a vuestra elección.
- hasta *1.5 puntos*: usar una librería para gestionar el estado de vuestra aplicación de manera centralizada (se explicará con más detalle qué es la gestión de estado el 17 de noviembre). En Vue se usaría [Vuex](https://vuex.vuejs.org), en otros *frameworks* hay equivalentes.
- hasta *1.5 puntos*: usar un *router* para gestionar la navegación por la *app*. En el caso de Vue se usaría [Vue Router](https://router.vuejs.org)


## Entrega

El plazo de entrega concluye el lunes **14 de diciembre de 2020** a las 23:59 horas. La entrega se realizará como es habitual a través de Moodle. Entregad una carpeta comprimida con el proyecto de esta práctica y el del servidor (modificado para usar CORS) en dos subcarpetas, ya que ambos son necesarios para ejecutar la aplicación. 

Entregad también un LEEME.txt donde expliquéis brevemente las partes optativas que habéis hecho y cualquier detalle que consideréis necesario.
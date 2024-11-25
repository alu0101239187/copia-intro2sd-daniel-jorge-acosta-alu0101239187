---
title: "Informe Jekyll Search"
categories:
  - Posts
tags:
  - Posts
  - Jekyll Search
---

El objetivo de esta práctica es añadir un buscador simple al sitio web generado usando Jekyll en la prática anterior. Este permitirá la búsqueda en todas las páginas del sitio y el uso de expresiones regulares.

## Resumen de "Lifecycle Types and Their Rationales"

El resumen del capítulo 2 del libro "Developing Information Systems: Practical Guidance for IT Professionals" se puede encontrar en forma de post con el título "Lifecycle Types and Their Rationales".

## Página de búsqueda

En el fichero `_pages/search.md` se puede encontrar la definición de la página. Esta es muy sencilla y consta únicamente de un campo de texto en el que se introduce la búsqueda y una lista en la que irán apareciendo los resultados.

Para realizar la búsqueda se utiliza un objeto `JekyllSearch`, definido en el fichero `assets/src/search.js`. Su constructor recibe un objeto que contiene la fuente de datos para la búsqueda, el campo de búsqueda, la lista en la que se mostrarán los resultados y la URL del sitio web. El método `init` se encarga principalmente de iniciar el listener encargado de ejecutar la búsqueda cada vez que se introduce un nuevo carácter y el encargado de evitar que se envíe el formulario al pulsar _Enter_. El método `findResults` es el encargado de encontrar los resultados que coinciden con el texto introducido, aceptando incluso expresiones regulares. Tras la ejecución de este, `displayResults` se encarga de generar la lista con todos los resultados.

La búsqueda se lleva a cabo en el fichero `assets/src/search.json`, que es una plantilla Liquid capaz de generar un JSON formado por el contenido de todas las páginas del sitio web.

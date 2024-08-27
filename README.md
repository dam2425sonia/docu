# Normas para realizar las entregas

Una vez realizada la tarea o tareas correspondientes se seguirán unas pautas para realizar las entregas, ver el archivo correspondiente.


# Como escribir un README.md correctamente, lenguaje Markdown

El formato markdown (md) se ha convertido en un estándar para editar y mostrar contenido de forma segura en la web:

Es simple.
Es potente, tiene un formato básico que permite crear documentación y/o artículos.
Permite mezclar HTML.
Es accesible.
Visual Studio Code ofrece un soporte muy bueno a este formato, tanto built-in como a nivel de ecosistema de plugins.

Si no conoces Markdown, puedes chequear esta guía

Manos a la obra
Si usamos VS Code tenemos la opción de ir escribiendo nuestro markdown y poder a la vez como queda esto en una ventana de previsualización.

Vamos a crear nuestro primer fichero md:

Creamos un archivo nuevo File >> New File, aquí tenemos dos opciones:

VSCode nos permite indicarle que el formato del nuevo fichero es markdown.
También podemos darle extensión md y ya lo reconoce automáticamente.
Vamos a introducir un texto de ejemplo:

# Hola markdown

Este es un texto de prueba
La ventana del editor no está mal, se ve algo marcado con colores, pero lo suyo es tener un visor para poder chequear el resultado final, para ello Visual Studio Code nos ofrece una ventana de previsualización ¿Cómo podemos activarla? Pulsando en el icono de lupa que hay en la derecha de la aplicación (otras formas de hacerlo: botón derecho y elegir del menú de contexto Open Preview to the side)

Bloques de código
Este visor de Markdown soporta bloques de código, sólo tenemos que indicarlo con los tres backticks y decirle de que lenguaje estamos hablando, podemos añadir lo siguiente:

Para introducir estos bloques de código, dependiendo del editor de Markdown que estemos utilizando, usará tres comillas invertidas (```) o tres tildes ( ~~~) en las líneas antes y después del bloque de código.

```tsx
export const component = () => <h1>Hola Mundo</h1>
```
Si por ejemplo queremos que se nos muestre un json formateado, podríamos hacerlo de la siguiente manera

```json
{
  "name": "Antonio",
  "company": "Tregue",
  "Country": "España"
}
```
Renderizado quedaría:

{
  "name": "Antonio",
  "company": "Tregue",
  "Country": "España"
}
Etiquetas HTML
El estándar de Markdown está muy bien, pero hay sitios en los que nos hace falta un poquito más, ¿Qué podemos hacer en estos casos? Tenemos la opción de mezclar HTML y Markdown.

Por ejemplo: Queremos mostrar la imagen de un logo, podemos hacer algo así como

![aqui va el logo](https://workingful-pro-lemoncode.s3.eu-west-3.amazonaws.com/lemoncode-tv/cursos/lesson/vscode-markdown-basico/logo.png)
Peero, queremos que sólo ocupa 180 píxeles de ancho, para ello reemplazamos la línea que hemos creado antes por html:

- ![aqui va el logo](./content/logo.png)
+ <img src="./content/logo.png" width="180px" />
supongamos que tenemos una imagen con un logo y queremos que ocupe un ancho en concreto, en Markdown podemos añadir imágenes, pero no podemos indicarle el ancho, para ello podemos usar directamente html:

<img src="./content/logo.png" width="90px" />
Si lo renderizamos lo veríamos de la siguiente forma:

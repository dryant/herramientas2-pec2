# README Y WEB EN DESARROLLO

# Web Club de Tenis

Web de un club de tenis (ficticio) comarcal en la que se anuncian los próximos partidos de la liga, actividades tales como extraescolares para niños, participantes de la liga, etc...

Esta web se ha creado para la práctica 2 de la asignatura **Herramientas HTML y CSS II** del Máster de desarrollo de aplicaciones y sitios web de la [**UOC**](https://estudis.uoc.edu/ca/masters-universitaris/aplicacions-multimedia/presentacio).

Los requisitos de la práctica eran los siguientes:

-   Usar el Boilerplate propio del Máster el cual se puede encontrar en [Boilerplate UOC](https://github.com/uoc-advanced-html-css/uoc-boilerplate)
-   Instalar dependencias externas con NPM tales como Fotnawesome, Bootstrap, y otras que se consideren oportunas
-   Usar el preprocesador SASS
-   Usar Bootstrap 5
-   Usar Flex
-   Usar CSS Grid con @supports para navegadores que no soportan CSS Grid
-   Uso de pseudoclases funcionales
-   Uso de container queries y capas de cascada
-   Diseño responsive
-   Aplicación de de metodologías y guías de estilo, adecuación a estándares y calidad del código en general
-   Instalación y configuración de StyleLint
-   Publicación en Github y deployment en Netlify

**Requisitos de la documentación**

-   Documentar todo el proceso de desarrollo
-   Justificación del uso de las pseudoclases funcionales y las capas de cascada.
-   Explicación de las container queries utilizadas
-   Justificación de las decisiones tomadas en el desarrollo, dependencias instaladas y personalización, problemas resueltos.
-   Justificación de la elección de la metodología y/o guía de estilo y descripción de la aplicación de los criterios elegidos

## ¿Qué es un Boilerplate?

Un Boilerplate es un conjunto de código preescrito que se utiliza como base en múltiples lugares.

En el desarrollo web, un "boilerplate" puede incluir la estructura HTML básica, archivos de estilo CSS y scripts JavaScript comunes.

**UOC Boilerplate** es una plantilla de inicio para la asignatura de **Herramientas HTML y CSS II** del [Máster de desarrollo de aplicaciones y sitios web](https://estudis.uoc.edu/ca/masters-universitaris/desenvolupament-llocs-aplicacions-web/presentacio) de la [Universitat Oberta de Catalunya](https://www.uoc.edu). Su objetivo es proporcionar un paquete básico y moderno para el desarrollo web frontend basado en Parcel e incluye un compilador de Sass, un transpilador de ES6, minificadores, un transformador de imágenes y herramientas de desarrollo.

Esta es la versión 3.x de UOC Boilerplate, disponible desde el segundo semestre del 2020.

## Requisitos

[Node.js](http://nodejs.org/) >= 14.15.x

## Como ver la web (Getting started)

Clonar este repositorio con `git clone`, o descarga el archivo .zip usando el botón verde que se encuentra arriba a la derecha.

Una vez en tu ordenador, abre el terminal y dirígete a a la carpeta del proyecto. Ejecuta `npm install` y despues `npm run dev` y se abrirá la web en el navegador.

## Características

-   Se usa el **module bundler** Parcel en su versión 2.
-   Incluye scripts de NPM para un desarrollo rápido y construcción de proyecto. scripts for fast development and production build (see Commands below).

### Estilos CSS

-   Se usa [Sass/SCSS](https://sass-lang.com) para la compilación de CSS.
-   Se Minifica y optimizan los archivos de css con [`cssnano`](https://github.com/cssnano/cssnano) (`@parcel/optimizer-cssnano`).
-   Se incluye PostCSS. Características de [PostCSS](https://postcss.org/):
    -   Transpilación de CSS moderno con [`postcss-preset-env`](https://preset-env.cssdb.org/features).
    -   Se añaden automáticamente prefijo de CC para las propiedades no soportadas con [`autoprefixer`](https://autoprefixer.github.io/).

### HTML

-   Se Minifica y optimizan los archivos de HTML al compilar la versión de producción con [`htmlnano`](https://github.com/posthtml/htmlnano) (`@parcel/optimizer-htmlnano`).
-   Se incluye [PostHTML](https://github.com/posthtml/posthtml) con sus características:
    -   Inclusión de archivos parciales con <include> [`posthtml-include`](https://github.com/posthtml/posthtml-include).

### Scripts

-   Permite transpilación automática de JavaScript moderno (ES201x/ES8/ES7/ES6…) a ES5 así como minificación en la compliación de la versión para producción, con [Babel](https://babeljs.io/).

### Imágenes

-   Conversión de imágnenes con [`@parcel/transformer-image`](https://parceljs.org/recipes/image/) (basado en [`sharp`](https://sharp.pixelplumbing.com/)).

### Desarrollo

-   Servidor de prueba con refresco automático con cada guardado de cambios en archivos.
-   Reporte de errores fácil de entender.

## Como usar el Boilerplate

El contenido de la web tiene que ir en la carpeta `src`. No cambiar la estructura ni los archivos de dicha carpeta a no ser que se quiera cambiar la configuración o que sepas lo que estás haciendo.

Para compilar una versión funcional de la web optimizada ejecutar `npm run build`. Una vez ejecutado el comando la web y todos sus archivos estarán ubicados en la carpeta `dist`

### Commandos

| Command         | Description                                                                                                                                                                                                                                                                                                                                                         |
| --------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `npm run dev`   | Runs a local web server for development and opens the browser to display it. Automatically compiles styles and scripts whenever a file in `src/` is changed, and live reloads the browser. This is what _must be run_ on the development stage.                                                                                                                     |
| `npm run build` | Compiles and minifies and optimizes the files in the assets folder. The generated compiled and optimized files are located in the `dist/` folder. This is what _must be run_ before publishing the project. This is also the build command to be run by external deployment services such as Netlify. The publishable files are then located in the `dist/` folder. |
| `npm run clean` | Deletes the current `/dist` folder and cache folders.                                                                                                                                                                                                                                                                                                               |
| `npm run test`  | Displays a success message if everything is working as expected.                                                                                                                                                                                                                                                                                                    |

## Créditos y mas información

Todos los créditos de este Boilerplate y sus funciones (incluyendo la traducción/adaptación de este README) pertenecen a [Jordi Tarrida](https://github.com/jorditarrida)

Todos los archivos HTML y CSS de la web han sido creados por [Pedro Blanch](https://github.com/dryant)

Aunque se ha tenido especial cuidado en la elección de imágenes libres de derechos, si alguna imagen infringe algún derecho, por favor comunícamelo y la retiro inmediatamente.

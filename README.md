# PROYECTO DE MAQUETACIÓN DE UN BLOG CON VITE Y SASS
## Configuración inicial paso a paso

- Creamos una carpeta llamada _practica-bootcamp-01_ y la abrimos con Visual Studio Code
- Creamos desde la consola de VSCode el archivo **package.json** para poder instalar dependencias
````bash
> npm init -y
````
- Instalamos **Vite** como tooling
````bash
> npm install vite
````
- Instalamos **SASS** para modulizar nuestro CSS
````bash
> npm install -D sass
````
- Creamos las carpetas _src_ y _public_
- Creamos los archivos _index.html_, _index.js_ y _src/main.scss_
````bash
> touch index.html index.js src/main.scss
````
- En _index.html_ agregamos la estructura de un documento html y un contenido de prueba
````html
<h1>Hola Bootcamp</h1>
````
- En _index.html_ enlazamos el _index.js_ como de tipo _module_
````html
<script src="./index.js" type="module"></script>
````
- En _index.js_ importamos nuestro archivo de sass
````js
import './src/main.scss';
````
- En _main.scss_ agregamos unos estilos de prueba
````css
body {
  background-color: lightsalmon;
}
````
- Agregar los **comandos de vite** en el package.json
````json
"scripts": {
    "test": "echo \"Error: no test specified\" && exit 1",
    "dev": "vite",
    "build": "vite build",
    "preview": "vite preview"
  }
````
- Levantamos el server
````bash
npm run dev
````
- Ingresamos a la url que genera vite http://127.0.0.1:5173/

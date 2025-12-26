# React + TypeScript + Vite

This template provides a minimal setup to get React working in Vite with HMR and some ESLint rules.

Temas puntuales
En esta sección aprenderemos mucho sobre cómo funciona React, puntualmente veremos:
o  Custom Hooks - Hooks personalizados
o  DevTools de React
o  useRef - Hook propio de React
o  Generar versión de producción
o  Separación de responsabilidades
Esta es una sección muy importante porque marca el antes y el después de cómo trabajar en React, ya que los custom hooks son lo que usaremos de aquí en adelante para evitar aglomerar los componentes con demasiada lógica.



Proyecto React buscar gifs
1.- comprobar version de node
    node --version
    v       20.19.4
2.- npm create vite
    o  Project name:
    |  03_gifs-app
    o  Select a framework:
    |  React
    o  Select a variant:
    |  TypeScript + SWC

    cd 03_gifs-app
    npm install
    npm run dev
3.- abrir el proyecto en vscode y eliminar :
        o  carpeta assets
        o  App.css
        o  App.tsx
    eliminar contenido de
        o  index.css
    quitar dependencias rotas de 
        o  main.tsx
4.- tareas
    o  agrego este css https://gist.github.com/Klerith/78df674c84d833d28d5c06359b04fc75
       al index.css
    o  instalo la font de https://fonts.google.com/specimen/Montserrat+Alternates
       1.- Get font
       2.- Get embed code 
           seleccionas las letras
             Light 300
             Regular 400
             Bold 700
        3.- copio el codigo generado de 
               Embed code in the <head> of your html
               y lo pego en el index.html
            copio el codigo generado de 
               Montserrat Alternates: CSS classes
               y lo pego en el index.css
5.- para consumir peticiones API instalamos AXIOS
    o  npm install axios

E J E R C I C I O     T E R M I N A D O
El ejercicio termino en el paso anterior SEGUIMOS CON 
LA PARTE II que se grabara como [03_gifs-app_v2]
- inicia la version v.2
6.- Instalamos developer tools
    https://react.dev/learn/react-developer-tools
7.- vamos a crear el archivo de RELEASE que se subira para que se use en la WEB
    c:\npm run build
       corregir los errores
    a.- esta pagina permite montar el aplicativo que creamos de forma local y probarlo como localhost
            https://www.npmjs.com/package/http-server
        para instalarlo de forma local y probarlo como localhost
           1.- abre el cdm como administrador
           2.- y con la nstalacion Globally via npm
               c:\npm install --global http-server
           3.- me voy a la carpeta [dist] donde esta mi proyecto 
               C:\Projects\Git\React\03_gifs-app_v2>cd dist
           4.- me voy a la carpeta [dist] de mi proyecto y ejecuto
               C:\Projects\Git\React\03_gifs-app_v2\dist>http-server -o
    b.- esta pagina permite montar el aplicativo que creamos en la WEB
            https://www.netlify.com/
           1.- creo una cuenta
           2.- agrego la carpeta [dist] a la plataforma
           3.- pongo nombre del proyecto
           4.- Release listo
        

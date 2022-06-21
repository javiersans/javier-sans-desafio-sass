clase 13 SASS
---------
descargar
https://nodejs.org/es/

crear carpeta nueva

abrirla con visual

abrir la consola ctrlñ

tipear comando:
npm install nodemon node-sass

despues tipear npm init (a continuacion, la metralla de enter)

despues enter hasta que te dice is this OK? (yes)            hay q volver a dar enter

a la izquierda, clic en package.json 

UBICAR  la linea 11 y agregarle una coma al final. Después, agregar estas dos líneas de codigo debajo de "test" y a la misma altura que la 11:

"build-css": "node-sass --include-path scss scss/main.scss css/style.css",
"watch-css": "nodemon -e scss -x \"npm run build-css\""

ahora creamos las 2 carpetas (arriba de todo, a la misma altura que node.modules): 

una es la scss y dentro creamos el archivo main.scss
la otra es la clasica de css con el archivo style.css dentro

este es el paso a paso que nos pasó johana
-------
1. Abrir la consola en esta carpeta con ctrl+ñ. npm install nodemon node-sassb. 
esperar y después: tipear npm init

2. Abrir el archivo package.json y editarlo. A continuación de && exit 1" colocar una coma (,) presionar enter y pegar el siguiente texto:"build-css": "node-sass --include-path scss scss/main.scss css/style.css","watch-css": "nodemon -e scss -x \"npm run build-css\""

3. Crear las carpetas con sus respectivos archivos: 
scss/main.scss 
css/style.css
------------------------

ahora hay que volver a la consola

primero tipear npm run build-css
enter y esperar

despues tipear npm run watch-css
enter y esperar  

hacer el archivo readme.txt

IMPORTANTE: si cierro visual, al reabrirlo (desde la carpeta, con abrir con visual, DEBO volver a escribir en la consola: 
npm run watch-css

------
readme.txt

//COMO EMPEZAR A COMPILAR SASS//

1. Abrir la consola en esta carpeta con ctrl+ña. npm install nodemon node-sassb. npm init

2. Abrir el archivo package.json y editarloa. A continuación de && exit 1" colocar una , presionar enter y pegar el siguiente texto:"build-css": "node-sass --include-path scss scss/main.scss css/style.css","watch-css": "nodemon -e scss -x \"npm run build-css\""

3. Crear las carpetas con sus respectivos archivosa. scss/main.scssb. css/style.css

4. En la consola correr el comandoa. npm run build-css //Por unica vezb. npm run watch-css

5. Cada vez que se quiera seguir compilando en SASSa. abrir la consola con ctrl+ñb. npm run watch-css

//FIN



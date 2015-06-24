title: aLb-nodejs
tags:
---
https://github.com/coolaj86/iojs-install-script#apple-os-x


instalar nvm
instalar iojs
correr con permisos de superusuario para generar los modulos (npm install)

Node directory
/usr/local/bin/node

io.js es un fork de nodeJS que está en proceso de unirse de nuevo a node conformando un sólo proyecto de nuevo.

se le pueden enviar variables de entorno cuando se corre el server de node

por ejemplo en el codigo tienes algo como 
process.env.PORT 

y el comando para correr el proyecto pasandole una variable de entorno puerto seria

PORT=8080 node server.js


los callbacks son funciones que se ejecutan cuando un metodo asyncrono termina de ejecutarse

una funcion asyncrona no bloquea las entradas y salidas

Los Event emiter son cunado usamos la funcion .on y le damos una funcion

const permite definir variables constantes que no pueden cambiar.
let hace que la variable solo sea declarada dentro del scope
var no respeta el bloque de la funcion

el primer argumento de una funcion siempre va a ser el error

Stream son mecanismos para leer binarios de manera inteligente, mientras va cargando el buffer va entregando los datos en el response, es una lectura mucho mas rapida y mas fluida.

` backtide
sirver para concatenar strings con el simbolo ${}
ejemplo:
`Server running in port ${port}`

module.export sive para exportar una funcion para que sea usada por un modulo superior
module.export = onRequest

En npm ahora se pueden encontrar tambien librerias para el lado del cliente como JQuery, Backbone etc.

npm install dependencia --save
npm install dependencia --save-dev

previene el funcionamiento default
e.preventDefault()

scripts en el package.json puede servir para poner alias a comandos comunmente usados

"start": "node server.js"
"build-js": "browserify client/app.js -o public/app.js"
"postinstall": "npm

npm start
npm run script
para esto se puede usar grunt


jsonbody tiene un limite el cual se va aumentar
3MB = 3 * 1024 * 1024

con module export tambien se pueden exportar objetos
module.exports = {
  convertVideo: require('./video')
}

al requerir el modulo siempre te regresa el index.js por eso es un estandar

require('../helper') regresa el index.js dentro de la carptea helper

####reemplazar callbacks con promises

los callbacks siempre van al final
async.series(array, callback)
  async.series([
    decodeImages,
    createVideo,
    encodeVideo,
    cleanup
  ], convertFinished)
  
 async.eachSeries
  	realiza las funciones en asyncrono y mantiene el orden
 async.each 
 	realiza las funciones en asyncrono pero no mantiene el orden
    
open $TEMPDIR para abri el directorio temporal en la MAC

os.tmpdir() en node para obtener la ruta

childProcess es un modulo que permite ejecutar comandos del sistema, ejecutar algun script etc.

const spawn = require('child_process').spawn

se exporta el metodo spawn de child_process

spawn - Ejectua el comando y entraga los streams de salida de error y del comando
exec - Ejecuta el comando y hace buffer de la salida y envia todo el buffer
fork - WTH

para instalar binarios hay que copiar al /usr/local/bin/

echo $? para saber si el ultimo comando se ejecuto bien o mal, regresa el codigo de ejecucion (en MAC y Linux)

en javascript 0 es falso
if (!code) //it  means if true

hay socketio del lado del servidor y del lado del cliente
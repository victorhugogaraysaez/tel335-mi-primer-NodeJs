# tel335-mi-primer-NodeJs Visto el 08/04/2024

Por favor cuando vayan a hacer su segundo commit haganlo modificando app.js de la siguiente forma

var http = require('http');

var server = http.createServer();

function mensaje(petic, resp) {

    resp.writeHead(200, {'content-type': 'text/plain'});
    
    resp.write('Hola, Mundo');
    
    resp.end();
    
}   //va sin punto y coma al final, y no se ejecuta pagina sola, hay que escribir en el navegador http://127.0.0.1:3000

server.on('request', mensaje);

server.listen(3000, function() {

    console.log('La aplicación está funcionando en el puerto 3000, hay que escribir en el navegador http://127.0.0.1:3000')
    
});

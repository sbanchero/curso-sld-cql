# Materiales

## Software
  * Vamos a trabajar con una página web de ejemplo que la podemos servir desde nuestras máquinas utilizando Python.

      python -m SimpleHTTPServer
      Serving HTTP on 0.0.0.0 port 8000 ...

    La idea es que lo puedan reproducir uds.

  * Para acceder a nuestro directorio web desde el navegador vamos a [http://localhost:8000](http://localhost:8000)

  * Para probar nuestras geometrías vamos a usar [esta](http://jsfiddle.net/WG8YP/4/) estupenda herramienta.

## Datos
Utilizaremos datos publicados por el Gobierno de la Ciudad de Buenos Aires que pueden ser encontrados [http://data.buenosaires.gob.ar](aquí)

Las coberturas son:

  * Áreas Hospitalarias
  * Puntos de acceso WI-FI público
  * Calles de la Ciudad de Buenos Aires

También utilizaremos una cobertura de división departamental de Argentina de IGN


## CQL_FILTER y Filter 

En gran parte del curso, vamos a probar filtros utilizando CQL_FILTER contra un servicio WMS, pero también vamos a usar (si llegamos) a ver algo de Filter.
EN el primer caso los Queries/Filtros los enviamos via GET al servicio WMS mientras que en el caso de usar Filter irán por POST. Para este caso vamos a utilizar 
la herramienta Poster. 
  * [Chrome](https://chrome.google.com/webstore/detail/chrome-poster/cdjfedloinmbppobahmonnjigpmlajcd)
  * [Firefox](https://addons.mozilla.org/en-us/firefox/addon/poster/)

## Referencias
[Datos de Buenos Aires](http://data.buenosaires.gob.ar)
[POST/GET](http://www.w3schools.com/tags/ref_httpmethods.asp)


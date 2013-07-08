# Introducción al lenguaje CQL

Las capas sobre las que se realizarán los filtros son:

* Wifi (POINT)
  * NOMBRE
  * SITIO: Teatros, Otros Establecimientos, Museos, Hospitales y CESACs, Espacios Públicos, Centros de Exposiciones, Centros Culturales, Bibliotecas
  * COMUNA: [1 a 15]
  * LAT
  * LONG
  * DIRECCION
  * alcance [27 a 100] mts
  * finstalac (Fecha de instalación de la antena aaaa-mm-dd)

* Áreas hospitalarias (POLYGON)
  * GIDAH 
  * NOMBRE
  * area_km2
  * habitantes

## Sintaxis de las consultas, definición de predicados

- Operadores relacionales

  = | <> | < | <= | > | >=


### Probar algunos filtros básicos

1. Aplicar filtros sobre la capa **wifi** 
  * antenas de la comuna 4
  * antenas de las comunas 1 a 6
  * antenas ubicadas solo en **Teatros**
  * antenas con alcance menor a 50 mts


2. Aplicar filtros sobre la capa **Áreas hospitalarias** 
  * filtrar el área hospitalaria con GIDAH 1
  * ¿qué ocurrio al aplicar el filtro anterior?
  * filtrar áreas mayores o iguales a 11 km2
  * filtrar áreas donde la cantidad de habitantes por km2 sea < 10000. Utilice paréntesis para escribir la expresión.

### Uniendo algunos predicados
  Operadores booleanos NOT AND OR
  
1. Aplicar filtros sobre la capa **wifi** 
  * antenas de la comuna 5 y alcance mayor a 30 mts
  * antenas en **Museos** de la Comuna 1
  * antenas ubicadas en **Teatros** o **Bibliotecas**


2. Aplicar filtros sobre la capa **Áreas hospitalarias** 
  * filtrar el área hospitalaria con GIDAH 1
  * ¿qué ocurrio al aplicar el filtro anterior?
  * filtrar áreas mayores o iguales a 11 km2
  * filtrar áreas donde la cantidad de habitantes por km2 sea < 10000. Utilice paréntesis para escribir la expresión.










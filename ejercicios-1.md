# Introducción al lenguaje CQL

Las capas sobre las que se realizarán los filtros son:

* Wifi (POINT)
  * gid
  * nombre
  * sitio: Teatros, Otros Establecimientos, Museos, Hospitales y CESACs, Espacios Públicos, Centros de Exposiciones, Centros Culturales, Bibliotecas
  * comuna: [1 a 15]
  * direccion
  * alcance [27 a 100] mts
  * f_instalac (Fecha de instalación de la antena aaaa-mm-dd)

* Avenidas (LINESTRING)
  * nombre
  * nombre_anterior
  * longitud

* Áreas hospitalarias (POLYGON)
  * gidah 
  * nombre
  * area_km2
  * habitantes

## Sintaxis de las consultas, definición de predicados

- Operadores relacionales

  _= | <> | < | <= | > | >=_


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
  * filtrar el área hospitalaria con GIDAH mayor a 3 y menor que 6
  * filtrar áreas mayores o iguales a 11 km2 y cantidad de habitantes mayores a 220000

  Operador *BETWEEN AND*

1. Aplicar filtros sobre la capa **wifi** 
  * antenas de las comunas 1 a 6
  * antenas con alcance entre 90 y 100

2. Aplicar filtros sobre la capa **Áreas hospitalarias** 
  * filtrar el área hospitalaria con área entre 14 y 20
  * filtrar áreas cantidad de habitantes entre 100000 y 180000

  Operadores *LIKE* / *ILIKE* y los wild-card

1. Aplicar filtros sobre la capa **wifi** 
  * filtrar antenas de que se encuentren en la calle RIVADAVIA
  * pruebe el filtro anterior con *ILIKE*. ¿Qué ocurre si utilizo Rivadavia? 

2. Aplicar filtros sobre la capa **Áreas hospitalarias** 
  * filtrar las áreas hospitalarias que no lleven nombres de doctores. :D
  * filtrar los nombres de hospitales que finalicen con la letra z

3. Aplicar filtros sobre la capa **Avenidas**
  * filtrar las avenidas con nombre "Juan"

  Operador *IN*

1. Aplicar filtros sobre la capa **wifi** 
  * filtrar antenas de que se encuentren en ubicadas en Teatros, Espacios Públicos, Centros Culturales o Bibliotecas

2. Aplicar filtros sobre la capa **Áreas hospitalarias** 
  * filtrar las áreas que NO sean 8, 12 ó 26

### Escribir 5 predicados compuestos con lo visto hasta aquí.
    

### Filtros en datos fecha
  Operadores *BEFORE* y *AFTER*

1. Aplicar filtros sobre la capa **wifi**
  * filtrar las antenas que fueron colocadas antes del 2012-01-25T00:00:00
  * filtrar las antenas que fueron colocadas después del 2012-07-15T00:00:00



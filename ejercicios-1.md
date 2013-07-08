# Introducción al lenguaje CQL

Las capas sobre las que se realizarán los filtros son:

* Wifi (POINT)
  * NOMBRE
  * SITIO: Teatros, Otros Establecimientos, Museos, Hospitales y CESACs, Espacios Públicos, Centros de Exposiciones, Centros Culturales, Bibliotecas
  * COMUNA: [1 a 15]
  * LAT
  * LONG
  * DIRECCION

* Áreas hospitalarias (POLYGON)
  * GIDAH 
  * NOMBRE
  * area km2
  * habitantes

## Sintaxis de las consultas, definición de predicados

- Operadores relacionales

  = | <> | < | <= | > | >=


### Probar algunos filtros básicos

1. Aplicar filtros sobre la capa **wifi** 
  * antenas de la comuna 4
  * antenas de las comunas 1 a 6
  * antenas ubicadas solo en **Teatros**
  * 

2. Aplicar filtros sobre la capa **Áreas hospitalarias** 
  * filtrar el área con GIDAH 1
  * 













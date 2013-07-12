# Introducción al lenguaje CQL

## Operadores para evaluar relaciones espaciales

  INTERSECTS ( Expresión , Expresión ) <> DISJOINT ( Expresión , Expresión )

1. Filtrar todas las antenas de WIFI que intersecten con *Poligono 1*
2. Filtrar todas las calles que intersecten con el *Polígono 2*

CONTAINS ( Expresión , Expresión )

1. Filtrar el área hospitalaria que contiene a la Av. Monroe (*Línea 1*)
2. Filtrar el área hospitalaria que contiene al *Polígono 3* 

WITHIN ( Expresión , Expresión )
1. Filtrar las antenas ubicadas dentro del *Polígono 1*
2. Filtrar las avenidas que están dentro del *Polígono 2* 


CROSSES ( Expresión , Expresión )
1. Filtrar las avenidas que cruzan a la Av. Monroe (*Línea 1*)

OVERLAPS ( Expresión , Expresión )
1. Filtrar las áreas hospitalarias que se solapan con el *Polígono 2*

DWITHIN ( Expresión , Expresión , distance , units ) <> BEYOND( Expresión , Expresión , distance , units )
1. Filtrar las avenidas que se encuentren a no más de 1 km del *Punto 1* 
2. Filtrar las antenas que se encuentren más allá de 5 km del *Punto 2*  

__NOTA__: Tener en cuenta el SRS de los datos. Los del TP son EPSG:4326 WGS84 LatLon

BBOX ( Expresión , Number , Number , Number , Number [ , CRS ] )

  * Filtrar los para todas las capas lo que esté en el siguiente BBOX _-58.488,-34.637,-58.382,-34.580_




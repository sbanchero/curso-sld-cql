# Introducción al lenguaje CQL

## Operadores para evaluar relaciones espaciales

  INTERSECTS ( Expresión , Expresión ) <> DISJOINT ( Expresión , Expresión )

1. Filtrar todas las antenas de WIFI que intersecten con Poligono 1
2. Filtrar todas las calles que intersecten con el Polígono 2


CONTAINS ( Expresión , Expresión )

1. 
2. 

WITHIN ( Expresión , Expresión )


TOUCHES ( Expresión , Expresión )


CROSSES ( Expresión , Expresión )


OVERLAPS ( Expresión , Expresión )


EQUALS ( Expresión , Expresión )


RELATE ( Expresión , Expresión , pattern )


DWITHIN ( Expresión , Expresión , distance , units ) <> BEYOND( Expresión , Expresión , distance , units )
  * 
  * 

NOTA: Tener en cuenta el SRS de los datos. Los del TP son EPSG:4326 WGS84 LatLon

BBOX ( Expresión , Number , Number , Number , Number [ , CRS ] )

  * Filtrar los para todas las capas lo que esté en el siguiente BBOX _-58.488,-34.637,-58.382,-34.580_




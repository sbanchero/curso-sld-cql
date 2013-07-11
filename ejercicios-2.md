# Introducción al lenguaje CQL

```sql
POLYGON((-58.4119188098047 -34.5980030767744,
-58.3987230001122 -34.5997603196344,
-58.3812498748144 -34.5990312879712,
-58.3784934074176 -34.6274890277966,
-58.3921594304398 -34.6272636036672,
-58.4159558045975 -34.6313809561029,
-58.4187886495199 -34.6085381813419,
-58.4179133234463 -34.5999016944123,
-58.4172629177523 -34.5978256694136,
-58.4119188098047 -34.5980030767744))
```




## Operadores para evaluar relaciones espaciales

INTERSECTS ( Expresión , Expresión )


DISJOINT ( Expresión , Expresión )


CONTAINS ( Expresión , Expresión )


WITHIN ( Expresión , Expresión )


TOUCHES ( Expresión , Expresión )


CROSSES ( Expresión , Expresión )


OVERLAPS ( Expresión , Expresión )


EQUALS ( Expresión , Expresión )


RELATE ( Expresión , Expresión , pattern )


DWITHIN ( Expresión , Expresión , distance , units )


BEYOND( Expresión , Expresión , distance , units )


BBOX ( Expresión , Number , Number , Number , Number [ , CRS ] )


BBOX ( Expresión , Expresión | Geometry )



# Consultas ECQL entre capas

Para poder realizar estas consultas entre capas es necesario incorporar un módulo a Geoserver llamado QueryLayer [0]

   INTERSECTS(the_geom, collectGeometries(queryCollection('Trails', 'the_geom', 'INCLUDE')));INCLUDE
   INTERSECTS(the_geom, querySingle('wifi', 'the_geom','comuna = 1')).
   INTERSECTS(the_geom, querySingle('areas_hospitalarias', 'the_geom','GIDAH=4'))



[0] [http://ufpr.dl.sourceforge.net/project/geoserver/GeoServer%20Extensions/2.3.3/geoserver-2.3.3-querylayer-plugin.zip](http://ufpr.dl.sourceforge.net/project/geoserver/GeoServer%20Extensions/2.3.3/geoserver-2.3.3-querylayer-plugin.zip)

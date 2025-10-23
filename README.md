# Accidentabilidad de VMPs en Barcelona e incidencia sobre peatones
### A partir de los datos recopilados por la Guàrdia Urbana el año 2022

## Contexto del proyecto  
El Ayuntamiento de París ha decidido dar por finalizada la concesión de uso del espacio público a los operadores de VMPs compartidos a partir del 1 de septiembre de 2023, una decisión tomada tras una consulta popular celebrada en abril en la que cerca del 90% de los participantes votó a favor de esta medida. Sorprendido por esta noticia he querido comprobar la situación en la ciudad de Barcelona. Se trata de un análisis exploratorio simple en el que comprobaré la accidentabilidad de VMPs (sin distinguir entre eléctricos y no eléctricos) y la incidencia de estos accidentes en los peatones.

### Retos
Lorem ipsum tatatá

### Fuentes de datos
La información de la accidentabilidad en la ciudad de Barcelona, según los expedientes de la Guàrdia Urbana, se facilita a través del portal de Open Data en 5 ficheros CSV diferentes. Para este análisis solo se tendrán en cuenta los datos correspondientes al año 2022.

Enlace a los datos: https://opendata-ajuntament.barcelona.cat/data/es/organization/seguretat

Ficheros disponibles:  
* **2022_accidents_gu_bcn.csv** Información genérica de los accidentes reportados.  
* **2022_accidents_persones_gu_bcn.csv** Información de todas las personas implicadas en cada accidente.  
* **2022_accidents_vehicles_gu_bcn.csv** Información de los vehículos implicados en cada accidente.  
* **2022_accidents_causes_gubcn.csv**  
* **2022_accidents_tipus_gu_bcn.csv**  

## Conclusiones principales

* Se observa que la mayor accidentabilidad de VMP's se produce los días laborables entre las 14h y las 18h.  
* Se observa que las zonas con mayor accidentabilidad de VMP's son aquellas más próximas al mar, con menores pendientes.  
* Un 10.74% de los accidentes reportados tienen, por lo menos, un VMP implicado.  
  * Convendría conocer el porcentaje de VMPs en el total vehículos que circulan en la ciudad, para poner este porcentaje en contexto.  
* Prácticamente un 20% de los accidentes con al menos un VMP implicado ha resultado con al menos un peatón lesionado.  
* De los 170 accidentes de VMPS reportados con al menos un peatón lesionado, el 40% (68 en total) han ocurrido en zonas peatonales, mientras que el 64% (109 en total) no son atribuibles al peatón.  
  *  Las cifras son explícitas y dan cuenta de la peligrosidad de los VMPs para los peatones.  

**La imagen global obtenida para el año 2022 en la ciudad de Barcelona demuestra el alto nivel de accidentabilidad de los vehículos VMPs y de su alto impacto en la seguridad viaria de los peatones.**  

## Descripción de los ficheros

**analysis_accs.ipynb**  
Análisis de la accidentabilidad de VMP's en la ciudad de Barcelona. Obtención de los ficheros csv que se exportarán a la herramienta de visualización flourish.

**cleanse_accidents.ipynb**  
Limpieza y adecuación de los ficheros originales para el análisis a realizar.

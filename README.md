# CursodeBigData
Generando mapas con Python
Introducción
En este laboratorio aprenderemos a crear distintos mapas interactivos. Para ello utilizaremos una nueva librería llamada Folium, 
una librería creada con el objetivo de visualizar datos geoespaciales. También destacamos que estas visualizaciones es posible realizarlas con 
plotly, 
pero hay un límite de veces que podemos llamar a la API para datos geoespaciales, a no ser que paguemos. Por otro lado, folium es completamente 
gratuito
y mas potente.

Inmigración a Canadá de 1980 a 2013 - Flujos migratorios internacionales hacia y desde países seleccionados - y
La revisión de 2015 del sitio web de las Naciones Unidas. El conjunto de datos contiene datos anuales sobre los flujos de migrantes internacionales
registrados por 
los países de destino. Los datos presentan tanto las entradas como las salidas según el lugar de nacimiento, ciudadanía o lugar de residencia 
anterior/posterior tanto para extranjeros como para nacionales. P
ara esta lección, nos centraremos en los datos de inmigración canadiense
Introducción a Folium
Folium es una potente libería de Python que permite crear diferentes tipos de mapas utilizando la librería de javascrip Leaflet. Los mapas de
Folium son interactivos lo que les da un valor añadido ya que pueden ser integrados en dashboards.
Mapas con indicadores
En esta sección trabajaremos con el siguiente copnjiunto de datos: Incidentes del Departamento de Policía de San Francisco del año 2016 - 
Police Department Incidents del portal de datos públicos de San Francisco. Incidentes derivados del sistema de informes de incidentes delictivos 
del Departamento de Policía de San Francisco (SFPD). Se actualiza diariamente y muestra los datos de todo el año 2016. La dirección y la ubicación 
se anonimizaron moviéndose a mitad de cuadra o a una intersección.

Descarguemos e importemos los datos sobre los incidentes del departamento de policía usando el método de pandas read_csv().

En esta sección trabajaremos con los datos del departamento de policia de San Francisco, un conjunto de datos con los incidentes de 2016. Police
Department Incidents.
Mapas de Coropletas
Un mapa de Coropletas es un mapa temático en el que las áreas están sombreadas o modeladas en proporción a la medida de la variable estadística
que se muestra en el mapa, como la densidad de población o el ingreso per cápita. El mapa de coropletas proporciona una manera fácil de visualizar
cómo varía una medida en un área geográfica, o muestra el nivel de variabilidad dentro de una región. A continuación se muestra un mapa de 
Coropletas de los EE. UU. que muestra la población por milla cuadrada por estado.

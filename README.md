# CursodeBigData

DIA 3
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



Día 4: Predicción mediante aprendizaje automático

En este día, me enfrenté al desafío de crear un modelo de aprendizaje automático para predecir si la primera etapa de los lanzamientos de cohetes de SpaceX aterrizará o no. SpaceX ha logrado ahorrar una gran cantidad de dinero al reutilizar la primera etapa de sus cohetes Falcon 9, lo que les permite ofrecer lanzamientos a un costo mucho menor que otros proveedores.

Para lograr esto, comencé realizando un análisis exploratorio de los datos disponibles y determiné las etiquetas de formación necesarias para mi modelo. Luego, creé una columna adicional para representar la clase objetivo. Para garantizar un rendimiento óptimo del modelo, estandaricé los datos y dividí el conjunto de datos en datos de entrenamiento y datos de prueba.

A continuación, me propuse encontrar el mejor hiperparámetro para tres algoritmos diferentes: SVM (Support Vector Machine), árboles de clasificación y regresión logística. Utilicé la función GridSearchCV para probar diferentes combinaciones de hiperparámetros y seleccionar los mejores resultados utilizando los datos de validación.

Para el algoritmo de regresión logística, creé un objeto de regresión logística y luego un objeto GridSearchCV llamado logreg_cv. Ajusté este objeto utilizando los parámetros descritos, estableciendo scoring='accuracy' y cv=10. A través de este proceso, pude encontrar los mejores parámetros utilizando el atributo best_params_ y evalué la precisión en los datos de validación utilizando el atributo best_score_.

Una vez que obtuve los mejores parámetros, calculé la precisión en los datos de prueba utilizando el método score sobre los conjuntos de prueba (X_test e Y_test). También utilicé la matriz de confusión para comparar las predicciones (y_pred) con las etiquetas reales (Y_test) y observé que la regresión logística pudo distinguir entre las diferentes clases, aunque se identificó como un problema principal la presencia de falsos positivos.

Además de la regresión logística, también implementé el algoritmo SVM. Creé un objeto Support Vector Machine y luego un objeto GridSearchCV llamado svm_cv, con los mismos parámetros y configuraciones mencionados anteriormente. A través del ajuste de este objeto, encontré los mejores parámetros y calculé la precisión en los datos de prueba utilizando el método score. También representé la matriz de confusión para evaluar el rendimiento del modelo.

Posteriormente, apliqué un clasificador de árbol de decisión, creando un objeto y un objeto GridSearchCV llamado tree_cv. Al igual que antes, ajusté el objeto tree_cv para encontrar los mejores parámetros y calculé la precisión del modelo en los datos de prueba utilizando el método score.

Finalmente, decidí probar el algoritmo de los k vecinos más cercanos (KNN). Creé un objeto de KNN y un objeto GridSearchCV llamado knn_cv. A través del ajuste de este objeto, encontré los mejores parámetros y calculé la precisión en los datos de prueba utilizando el método score.

Para determinar el método que mejor funcionó en este escenario, creé un dataframe con los resultados obtenidos de cada algoritmo y los comparé. Utilicé un gráfico de barras para visualizar las diferencias en el rendimiento de los algoritmos.

En resumen, a través de este día de trabajo como científico de datos, realicé un análisis exploratorio de los datos, encontré las mejores etiquetas de formación, estandaricé los datos, dividí los datos en conjuntos de entrenamiento y prueba, encontré los mejores hiperparámetros para los algoritmos de SVM, árboles de clasificación y regresión logística, evalué el rendimiento de cada algoritmo en los datos de prueba y comparé sus resultados para determinar el método que mejor se comportó en este contexto de predicción de aterrizaje de la primera etapa de los cohetes Falcon 9 de SpaceX.

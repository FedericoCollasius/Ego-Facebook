# Consigna Ego-Facebook

- Con los datos de Facebook, computar la matriz de similaridad con producto interno de la matriz de atributos, proponer un umbral u y construir un grafo conectando los nodos que superan ese umbral.
- Queremos comparar la red de amistades original y la construida a partir de los datos. Proponer alguna forma para compararlas o utilizar alguna de estas opciones. Comparar las redes mediante la correlacion de las matrices de adyacencia estiradas(flatten). Comparar utilizando la correlacion entre las listas de autovalores.
- Realizar el procedimiento anterior para suficientes valores de umbral y buscar el valor optimo que genera la red de atributos mas similar al grafo de amistades.
- Filtrar la matriz de atributos utilizando PCA: Computar la matriz de covarianza, luego los autovectores. Seleccionar k componentes principales y proyectar los datos al nuevo espacio. Repetir el punto anterior para varios valores de k y varios valores de u. Analizar los resultados.

Es obligatorio fundamentar los experimentos planteados, proveer los archivos e informacion necesaria para replicarlos, presentar los resultados de forma conveniente y clara, y analizar los mismos con el nivel de detalle apropiado. 
En caso de ser necesario,es posible tambien generar instancias artificiales con el fin de ejemplificar y mostrar un comportamiento determinado.

# De manera mas coloquial  

- La idea es trabajar con unos datos de grafos de facebook que son públicos.
- Se cuenta con un archivo que indica en cada fila si dos usuarios son amigos entre sí y con un archivo que para cada usuario indica si tiene un atributo o no (no está muy clara la info de qué son esos atributos). 
- Queremos poder construir grafos a partir de esos atributos, por ejemplo si dos personas tienen muchos atributos en común deberían estar conectadas. 
- Luego queremos comparar los grafos reales con los hechos por atributos y ver como podemos optimizar algunos parámetros para que esos gráfos se parezcan. 
- La idea es usar PCA en un momento para procesar los atributos (Python). 

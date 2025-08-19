Visualización de la Matriz de Correlación:

Utiliza sns.heatmap() para crear una visualización de la matriz de correlación de las variables numéricas. Esto es útil para identificar relaciones fuertes entre variables.

Análisis de Relaciones Específicas:

Se visualizan dos relaciones clave:

El tiempo de contrato (tenure) vs. la cancelación.

El gasto total (Charges.Total) vs. la cancelación.

Se usan gráficos como boxplot para variables categóricas y scatterplot para relaciones continuas.

Separación de Datos:

Se divide el conjunto de datos en variables independientes (X) y la variable dependiente (y). Luego, se divide en datos de entrenamiento y prueba (70% entrenamiento, 30% prueba).

Construcción de Modelos Predictivos:

Regresión Logística: Este modelo requiere normalización de las variables, por lo que se aplica StandardScaler para escalarlas antes de entrenar el modelo.

Árbol de Decisión: Este modelo no requiere normalización, por lo que se entrena directamente con los datos.

Evaluación de los Modelos:

Se evalúan ambos modelos usando métricas clave: exactitud, precisión, recall, F1-score, y la matriz de confusión. Luego, se comparan los resultados de los modelos.

Análisis de Variables Relevantes:

Para la regresión logística, se examinan los coeficientes de las variables, que muestran la importancia de cada variable en la predicción de la cancelación.

Para el árbol de decisión, se muestra la importancia de cada variable en el modelo, lo que indica qué características son más relevantes para la predicción.

Notas Adicionales:

Puedes ajustar el tamaño del conjunto de entrenamiento y prueba según el tamaño de tu base de datos.

Si decides agregar más modelos como Random Forest o KNN, puedes seguir el mismo proceso que para los dos modelos anteriores.

Asegúrate de revisar la normalización de las variables antes de aplicar modelos sensibles a la escala (como KNN y regresión logística).

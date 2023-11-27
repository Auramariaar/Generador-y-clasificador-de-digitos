# Generador-y-clasificador-de-digitos
Este proyecto incluye un cuaderno de Jupyter dedicado a crear un clasificador que utiliza el método Naive Bayes. Este clasificador se aplica a la base de datos MNIST, que contiene imágenes de dígitos manuscritos, y examina una estrategia elemental para la generación de nuevos dígitos.

# Resumen

Este cuaderno, Digit_Generation.ipynb, se centra en la carga, preparación y análisis de un conjunto de datos de imágenes de dígitos escritos a mano, utilizando el conjunto de datos MNIST. Además, incluye la implementación de un modelo de clasificación basado en el algoritmo Gaussian Naive Bayes para la identificación de dígitos, así como la evaluación de su rendimiento.
Librerías

El cuaderno utiliza las siguientes bibliotecas de Python:

    numpy: Para operaciones numéricas.
    matplotlib.pyplot: Para la visualización de imágenes y gráficos.
    sklearn: Para la carga del conjunto de datos MNIST, la división de datos y la implementación del modelo Gaussian Naive Bayes.

# Conjunto de datos
Cargar el conjunto de datos MNIST

El cuaderno comienza cargando el conjunto de datos MNIST, que contiene imágenes de dígitos escritos a mano. Puede aparecer el siguiente mensaje de advertencia durante la carga del conjunto de datos:

vbnet

/usr/local/lib/python3.10/dist-packages/sklearn/datasets/_openml.py:968: FutureWarning: The default value of `parser` will change from `'liac-arff'` to `'auto'` in 1.4. You can set `parser='auto'` to silence this warning. Therefore, an `ImportError` will be raised from 1.4 if the dataset is dense and pandas is not installed. Note that the pandas parser may return different data types. See the Notes Section in fetch_openml's API doc for details.
  warn(

# Preparación de datos

El cuaderno procede con la preparación de los datos de la siguiente manera:

    Se fija una semilla (seed_state) para garantizar la reproducibilidad.
    Se crean índices y se convierten las etiquetas a enteros para asegurar la consistencia.
    Se crean índices balanceados para cada dígito (0-9) para obtener un conjunto de datos equilibrado.
    Se dividen los datos en conjuntos de entrenamiento y prueba utilizando la función train_test_split.

# Modelo de clasificación

El cuaderno implementa un modelo de clasificación utilizando el algoritmo Gaussian Naive Bayes. A continuación, se detallan los pasos:

    Se importan las bibliotecas necesarias.
    Se inicializa el modelo Gaussian Naive Bayes.
    Se entrena el modelo con los datos de entrenamiento.
    Se realizan predicciones en el conjunto de prueba.
    Se calcula la precisión del modelo.

La precisión obtenida del modelo Gaussian Naive Bayes en el conjunto de prueba es del 55.36%.

# Informe de rendimiento

El cuaderno también realiza un informe de rendimiento que incluye la matriz de confusión y gráficas de barras de precisión, recall y F1-score para cada dígito. Se analizan las conclusiones basadas en este informe y se destacan áreas de mejora potencial.

# Conclusión

Este cuaderno proporciona una introducción a la carga y preparación de datos, así como a la implementación y evaluación de un modelo de clasificación en el contexto del conjunto de datos MNIST. Ofrece información sobre el rendimiento del modelo y sugiere áreas para futuras mejoras y exploración de datos.


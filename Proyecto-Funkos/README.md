# Clasificador de Funkos con CNN
Este proyecto implementa una Red Neuronal Convolucional (CNN) desde cero para clasificar imágenes de figuras Funko Pop. El objetivo principal es demostrar un flujo de trabajo completo: desde la ingesta de datos hasta la optimización de un modelo para evitar el sobreajuste.

 Tecnologías Utilizadas
Python

TensorFlow / Keras

Matplotlib & Seaborn (Visualización)

Scikit-Learn (Métricas de evaluación)

 Arquitectura y Metodología
Para construir este modelo, se siguió un enfoque técnico estructurado:

Preprocesamiento: Redimensionado de imágenes (150x150) y reescalado de píxeles [0, 1].

Data Augmentation: Uso de capas RandomFlip, RandomRotation y RandomZoom para mejorar la generalización del modelo.

Modelo CNN:

Capas Conv2D con filtros de 32, 64 y 128.

Capas MaxPooling2D para reducción de dimensionalidad.

Dropout (0.3 y 0.5) para combatir el overfitting.

Compilación: Optimizador Adam (learning rate 0.001) y función de pérdida SparseCategoricalCrossentropy.

Callback: Implementación de EarlyStopping para detener el entrenamiento tras 5 épocas sin mejora en la validación.

 Resultados
El modelo alcanzó un 56.25% de Accuracy en el conjunto de Test.
La matriz de confusión reveló que el modelo identifica perfectamente clases complejas como Zoro y Kaido, mientras que presenta confusión en clases con menor representación en el dataset, lo cual confirma la necesidad de un mayor volumen de datos para producción.

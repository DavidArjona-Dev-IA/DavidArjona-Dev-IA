Clasificador de Sentimientos con SVM (Twitter)
Este proyecto implementa un modelo de Máquinas de Vectores de Soporte (SVM) para realizar análisis de sentimiento sobre un conjunto de datos de tweets. El objetivo es clasificar automáticamente el tono emocional (positivo/negativo/neutral) del texto no estructurado.

 Tecnologías Utilizadas
Python

Scikit-Learn (SVM, Métricas de evaluación)

Pandas (Manipulación de datos)

NLTK / SpaCy (Procesamiento de texto/limpieza)

 Pipeline de Procesamiento
Para transformar texto "sucio" en predicciones, se siguió un flujo de trabajo típico de NLP:

Preprocesamiento: Limpieza de tweets (eliminación de menciones, enlaces, hashtags, stop-words y normalización de texto).

Vectorización: Transformación de texto a números utilizando TF-IDF (Term Frequency-Inverse Document Frequency) para capturar la importancia de las palabras.

Modelo: Entrenamiento de un clasificador SVC (Support Vector Classifier) con optimización de hiperparámetros.

Evaluación: Medición de rendimiento mediante Matriz de Confusión, Accuracy y F1-Score.

 Valor del Proyecto
Este sistema demuestra la capacidad de trabajar con datos no estructurados. A diferencia de los LLMs (que son modelos "caja negra" enormes), este proyecto muestra el dominio de modelos de Machine Learning tradicionales, que siguen siendo extremadamente valiosos por su interpretabilidad y eficiencia en tareas específicas de clasificación.

Próximos pasos
Word Embeddings: Implementar vectores densos (Word2Vec o FastText) para mejorar la comprensión semántica.

Pipeline de Producción: Empaquetar el modelo con pickle o joblib para realizar inferencias en tiempo real sobre nuevas publicaciones.

Este proyecto implementa una arquitectura RAG (Retrieval-Augmented Generation) utilizando LlamaIndex. El objetivo es permitir que un modelo de lenguaje (LLM) consulte y extraiga información precisa de una fuente de documentos personalizada, mejorando la veracidad de las respuestas y evitando alucinaciones.

 Tecnologías Utilizadas
Python

LlamaIndex (Framework de indexación y consulta)

LLMs (OpenAI GPT / Llama 3)

Bases de Datos Vectoriales (ChromaDB / Pinecone)

 Flujo de Trabajo (Pipeline)
El sistema sigue un proceso de 4 etapas para responder preguntas sobre documentos:

Ingesta de Datos: Carga y lectura de documentos (PDFs/TXTs).

Indexación: División de textos en chunks y generación de embeddings (representaciones vectoriales).

Recuperación (Retrieval): Búsqueda semántica en la base de datos vectorial para encontrar la información relevante a la consulta del usuario.

Generación: Envío del contexto recuperado al LLM para que redacte una respuesta fundamentada en los datos proporcionados.

 Valor del Proyecto
Este sistema permite crear asistentes inteligentes sobre dominios de conocimiento específicos (como manuales técnicos o bases de conocimiento corporativas) sin necesidad de reentrenar el modelo, siendo una solución altamente escalable y eficiente.

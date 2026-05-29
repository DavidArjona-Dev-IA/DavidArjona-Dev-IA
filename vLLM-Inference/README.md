Despliegue e Inferencia de LLMs con vLLM
Este proyecto explora la implementación de entornos de inferencia de alto rendimiento utilizando vLLM. El objetivo es optimizar el despliegue de Modelos de Lenguaje (LLMs) para maximizar la velocidad de respuesta (throughput) y la eficiencia en el uso de la memoria VRAM de la GPU.

 Tecnologías Utilizadas
Python

vLLM (Engine de inferencia de alta concurrencia)

PyTorch

Hugging Face (Model Hub)

 Metodología y Optimización
Para lograr una inferencia eficiente, se han aplicado los siguientes conceptos clave:

PagedAttention: Implementación de la técnica central de vLLM que permite gestionar de forma eficiente la memoria de la caché KV, eliminando la fragmentación de memoria interna.

Carga de Modelos: Integración de modelos directamente desde el hub de Hugging Face con configuraciones optimizadas para inferencia.

Manejo de Solicitudes: Pruebas de concurrencia para medir cómo el motor maneja múltiples peticiones simultáneas, un aspecto crítico en entornos de producción.

 Valor del Proyecto
vLLM es el estándar actual para servir modelos en producción debido a su capacidad para manejar peticiones de forma mucho más rápida que las implementaciones tradicionales. Este proyecto demuestra la capacidad de configurar y ejecutar un serving de modelos capaz de escalar en entornos reales.

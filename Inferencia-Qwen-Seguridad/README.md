#  Laboratorio de Inferencia y Seguridad de LLMs (Qwen2)

Este proyecto es una exploración profunda sobre el comportamiento de los Modelos de Lenguaje (LLMs). A diferencia de los proyectos de entrenamiento, aquí nos centramos en la **inferencia**, el ajuste de parámetros de generación y las vulnerabilidades de seguridad en el Prompt Engineering.

##  Tecnologías Utilizadas
* **Python**
* **Hugging Face Transformers**
* **PyTorch** (para gestión de tensores y GPU)
* **Técnicas de Seguridad** (Jailbreaking & Prefilling)

##  Experimentación realizada
Este cuaderno documenta tres experimentos críticos para entender cómo "razona" un LLM:
* **Configuración de Parámetros:** Pruebas de impacto real de la `temperature`, `top_p` y `repetition_penalty` sobre la coherencia del texto.
* **Seguridad y Prompt Engineering:** Implementación de un test de estrés (Proyecto Prometeo) para poner a prueba las instrucciones de seguridad del modelo mediante técnicas de *Prefilling*.
* **Análisis de Probabilidades:** Auditoría paso a paso de cómo el motor de inferencia selecciona el siguiente token y por qué ocurren los bucles de repetición.

##  Valor del Proyecto
El proyecto revela que la seguridad en IA es un equilibrio técnico: demuestra cómo parámetros mal configurados pueden llevar a un modelo a "alucinar" o a ignorar sus propias instrucciones de seguridad (vulnerabilidad por *prefilling*).

## 🚀 Próximos pasos
* **Defensa de Modelos:** Investigar métodos de *Guardrails* para evitar ataques de inyección de prompts.
* **Cuantización Avanzada:** Comparar el rendimiento de la inferencia en FP16 frente a versiones cuantizadas (AWQ/INT4).

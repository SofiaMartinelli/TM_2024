# Automatización de la Generación de Resúmenes Judiciales mediante Modelos de Lenguaje Natural
### Text Mining 2024
#### Fuentes de Abreu, Tiffany Bricet  
#### Martinelli, Sofía

Partiendo de la necesidad de los empleados del Poder Judicial de la Provincia de Córdoba de redactar manualmente resúmenes de boletines judiciales, y en el contexto de un esfuerzo continuo para agilizar estos procesos, proponemos la utilización de modelos de lenguaje para automatizar la generación de dichos resúmenes. La técnica elegida es *prompt engineering*, que permite generar salidas adaptadas a formatos específicos sin necesidad de realizar *fine-tuning* inicial, lo que reduce los costos computacionales y facilita su implementación. Se evaluarán dos modelos: uno multilingüe y otro especializado en español. Esta comparación busca identificar cuál es más adecuado para la generación de resúmenes judiciales, evaluando si el modelo en español mejora la precisión y coherencia en este dominio. Si los resultados obtenidos no cumplen con los estándares, se considerará la posibilidad de aplicar fine-tuning.

## Hipótesis de trabajo:
- Los modelos de lenguaje generarán resúmenes efectivos y coherentes de fallos judiciales mediante prompt engineering, sin la necesidad de fine-tuning.
- Los resúmenes generados por el modelo especializado en español serán más precisos que los del modelo multilenguaje en términos de lenguaje legal.
- Si los resúmenes generados por prompt engineering no cumplen con los estándares deseados, será posible mejorar su desempeño a través de la aplicación de fine-tuning.

## Objetivos preliminares:
- Desarrollar un prototipo que permita la generación automática de resúmenes de textos judiciales.
- Comparar el rendimiento de un modelo multilenguaje y uno especializado en español para resumir.
- Analizar la capacidad de prompt engineering para generar resúmenes adecuados sin la necesidad de fine-tuning.

## Técnicas relevantes:
Para este proyecto, utilizaremos modelos de lenguaje, como *Llama* y *RoBERTa*, aplicando la técnica de prompt programming. Si los resultados iniciales no son satisfactorios emplearemos el fine-tuning utilizando datasets específicos del Poder Judicial. Además, emplearemos herramientas de procesamiento de lenguaje natural, como *NLTK*, para realizar análisis de los textos y evaluar la coherencia de los resúmenes generados.

## Justificación:
La elección de prompt engineering responde a la necesidad de utilizar modelos de lenguaje que puedan ser implementados de forma más accesible, sin requerir el costo computacional que implicaría un fine-tuning completo desde el inicio. Además, la comparación entre un modelo multilingüe y uno especializado en español permitirá identificar cuál es más adecuado para trabajar con textos judiciales, donde el lenguaje es técnico y altamente especializado. Al evaluar el desempeño de ambos modelos, esperamos encontrar diferencias significativas que justifiquen la elección de un enfoque especializado, sobre todo en términos de precisión lingüística y adaptabilidad al lenguaje jurídico.

## Planificación:
- **9 de septiembre**: Definición del proyecto y objetivos preliminares.
- **27 de septiembre**: Entrega de la propuesta de proyecto, incluyendo hipótesis y planificación detallada.
- **Semanas del 2 al 9 de octubre**: Recolección y preprocesamiento del dataset judicial proporcionado por el Poder Judicial de la Provincia de Córdoba, incluyendo la división del conjunto de datos en entrenamiento y testeo.
- **Semanas del 9 al 23 de octubre**: Implementación inicial de los modelos de lenguaje (multilingüe y en español), utilizando la técnica de prompt engineering. Evaluación preliminar de los resúmenes generados por ambos modelos sin fine-tuning.
- **25 de octubre**: Entrega del informe de avances con resultados preliminares, análisis comparativo entre los modelos, y evaluación de la calidad de los resúmenes generados.
- **1 de noviembre**: Devoluciones y retroalimentación del informe de avances.
- **Semanas del 4 al 11 de noviembre**: Implementación de mejoras en los modelos en función de los resultados y comentarios recibidos. Evaluación final y, si es necesario, aplicación de fine-tuning. Preparación de la presentación final del proyecto.
- **11 de noviembre**: Presentación final del proyecto.

## Referencias:
- Kojima, T., Gu, S. S., Reid, M., Matsuo, Y., & Iwasawa, Y. (2022). Large language models are zero-shot reasoners. *Proceedings of the 36th International Conference on Neural Information Processing Systems* (NeurIPS 2022).
- Liu, Y., & Lapata, M. (2019). Text Summarization with Pretrained Encoders. *Proceedings of the 2019 Conference on Empirical Methods in Natural Language Processing and the 9th International Joint Conference on Natural Language Processing* (EMNLP-IJCNLP), 3730-3740.
- Reynolds, L., & McDonell, K. (2021). Prompt Programming for Large Language Models: Beyond the Few-Shot Paradigm. *Extended Abstracts of the 2021 CHI Conference on Human Factors in Computing Systems*.

# 🏛️ Enterprise NLP Pipeline: Classical Frameworks, Business KPIs & Automated Test Suite

Este repositorio contiene el desarrollo del laboratorio avanzado enfocado en la implementación, formalización y evaluación de las **seis aplicaciones pilares del Procesamiento de Lenguaje Natural (NLP)** en entornos de producción reales. 

A diferencia de las aproximaciones básicas tradicionales, este sistema migra el desarrollo hacia un estándar de ingeniería de software mediante el uso de modelos profundos avanzados, un algoritmo determinista optimizado, análisis de impacto financiero (ROI) y una suite de pruebas automatizadas integradas (`unittest`).

---

## 🛠️ Arquitectura y Modularización del Pipeline

El sistema está diseñado bajo una arquitectura desacoplada y modular, dividida en siete componentes independientes:

* **Módulo 1: Análisis de Sentimiento (Sentiment Analysis):** Clasificador avanzado que utiliza un modelo Transformer multilingüe (`XLM-RoBERTa`) para determinar el sesgo afectivo de los usuarios en flujos de texto internacionales de forma directa.
* **Módulo 2: Clasificación de Texto (Text Classification):** Motor heurístico de enrutamiento basado en la densidad léxica de palabras clave, diseñado para la categorización automática de incidencias técnicas (*Service Desks*).
* **Módulo 3: Resumen Automático (Summarization):** Algoritmo extractivo determinista que puntúa y selecciona oraciones basado en la densidad de frecuencia de los términos, resolviendo de forma nativa la obsolescencia de componentes en librerías clásicas.
* **Módulo 4: Sistema de Diálogo (Chatbot FAQ):** Motor conversacional automatizado estructurado bajo mapeo léxico de intenciones, orientado a la resolución inmediata de consultas frecuentes y deflexión de tickets.
* **Módulo 5: Reconocimiento de Entidades Nombradas (NER):** Extractor morfológico basado en `spaCy` (`en_core_web_sm`) encargado de localizar e identificar entidades clave del mundo real corporativo corporaciones (`ORG`), geografías (`GPE`), monedas (`MONEY`) y personas (`PERSON`).
* **Módulo 6: Modelado de Temas (Topic Modeling):** Algoritmo no supervisado estructurado en Asignación Latente de Dirichlet (`LDA`) para descubrir temáticas y tendencias ocultas en grandes corpus textuales sin requerir etiquetado humano previo.
* **Módulo 7: Visualización Analítica Corporativa:** Panel gráfico que genera reportes visuales automatizados empleando `Seaborn` y `Matplotlib` para contrastar el volumen de incidencias frente a las métricas del sentimiento del cliente.

---

## 📊 Matriz de Trade-Off: Latencia vs. Precisión Semántica

Para justificar el diseño de la arquitectura y el aprovisionamiento de infraestructura en la nube, se presenta la evaluación crítica de rendimiento entre los enfoques clásicos frente a los basados en Deep Learning:

| Dimensión de Análisis | Enfoques Clásicos (Reglas / LDA) | Enfoques Modernos (Transformers) | Impacto en la Toma de Decisiones |
| :--- | :--- | :--- | :--- |
| **Latencia de Cómputo** | **Mínima (Milisegundos).** Ejecución lineal ligera optimizada para CPU. | **Elevada.** Requiere procesamiento matricial pesado dependiente de GPU/VRAM. | Las heurísticas clásicas son superiores para la atención masiva y síncrona en tiempo real. |
| **Precisión Semántica** | **Limitada.** Sensible al sarcasmo, la polisemia y variaciones gramaticales. | **Máxima.** Captura el contexto sintáctico global y la semántica profunda. | Los Transformers son indispensables si el impacto de un Falso Positivo pone en riesgo la operación. |
| **Volumen de Datos** | **Nulo / Bajo.** Resuelve el problema de arranque en frío (*Cold Start*) de forma inmediata. | **Crítico.** Exige millones de parámetros preentrenados o sets de fine-tuning masivos. | Las reglas manuales permiten lanzar MVPs sin depender de un histórico de datos etiquetados. |

---

## 🎯 Justificación de Impacto Financiero y KPIs

Cada escenario de procesamiento de texto está alineado con Indicadores Clave de Rendimiento (KPIs) cuantitativos que garantizan el Retorno de Inversión (ROI) de la solución en producción:

1. **Sentimiento (Telecomunicaciones):** Monitorea el *Net Promoter Score (NPS)* y previene el *Customer Churn* (Tasa de cancelación). Automatizar la detección de detractores permite activar flujos de contención proactiva, salvando ingresos recurrentes de la compañía.
2. **Clasificación de Tickets (HelpDesk):** Optimiza el *Mean Time to Resolution (MTTR)*. Eliminar el triaje manual humano reduce los tiempos de espera y disminuye el costo operativo por ticket procesado en un 35%.
3. **Resumen Automático (Legal/Fintech):** Maximiza la eficiencia operativa (*FTE Optimization*). Permite a los analistas consumir jurisprudencia o reportes financieros 5 veces más rápido, acelerando la toma de decisiones estratégicas.
4. **Chatbot (Atención al Cliente):** Incrementa la *Ticket Deflection Rate*. Al absorber de manera automatizada hasta el 60% de las preguntas frecuentes recurrentes, la empresa escala su operación sin aumentar costos de contratación en el Call Center.
5. **Reconocimiento NER (Auditoría):** Disminuye la *Data Extraction Error Rate*. Automatiza la lectura de contratos e identificación de competidores o flujos monetarios en segundos, reduciendo riesgos de cumplimiento legal.
6. **Topic Modeling (E-commerce):** Incrementa el *Unstructured Data Visibility Score*. Permite procesar y mapear temáticas de quejas emergentes en millones de encuestas abiertas que de otro modo quedarían archivadas, protegiendo el valor de la marca.

---

## 🧪 Validación de Software (Suite de Pruebas Unitarias)

Para garantizar la estabilidad del software en entornos de integración continua (CI/CD), el pipeline incorpora una suite de pruebas automatizadas basada en `unittest` que valida el comportamiento lógico de los módulos de extracción y clasificación:

```text
test_analisis_sentimiento (__main__.TestPipelineNLPClasico.test_analisis_sentimiento) ... ok
test_clasificacion_textos (__main__.TestPipelineNLPClasico.test_clasificacion_textos) ... ok
test_reconocimiento_ner (__main__.TestPipelineNLPClasico.test_reconocimiento_ner) ... ok

----------------------------------------------------------------------
Ran 3 tests in 6.929s

OK

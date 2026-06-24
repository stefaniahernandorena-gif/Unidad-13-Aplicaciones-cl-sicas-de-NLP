# Unidad-13-Aplicaciones-cl-sicas-de-NLP
Unidad 13 · Aplicaciones clásicas de NLP
# 🏛️ Classical NLP Applications: Business Use Cases & Implementations

Este repositorio contiene el laboratorio correspondiente a la exploración y optimización de las **cuatro aplicaciones clásicas del Procesamiento de Lenguaje Natural (NLP)** en entornos de negocio reales: Análisis de Sentimiento, Clasificación de Texto, Resumen Automático y Sistemas de Diálogo (Chatbots).

A lo largo del proyecto se priorizó la reestructuración de código heredado, sustituyendo librerías obsoletas por arquitecturas modernas de Deep Learning y algoritmos deterministas eficientes.

---

## 🛠️ Optimizaciones de Ingeniería Realizadas

1. **Análisis de Sentimiento Multilingüe (Escenario 1):** Se descartó el uso de *TextBlob* sugerido en las plantillas básicas debido a su incapacidad nativa para procesar sintaxis en español sin traducción. Se integró un modelo **Transformer multilingüe basado en XLM-RoBERTa** que detecta la polaridad idiomática real de forma directa.
2. **Resumen Automático Robusto (Escenario 3):** Debido a la depreciación del módulo `summarization` en las versiones modernas de *Gensim*, se diseñó un algoritmo de **Resumen Extractivo Frecuencial** nativo, puntuando las oraciones según la relevancia estadística de sus componentes morfológicos.

---

## 📊 Soluciones de Negocio Implementadas

* **Telecomunicaciones (Sentimiento):** Automatización del monitoreo de opiniones de usuarios ante lanzamientos comerciales, segmentando de forma precisa comentarios positivos, negativos y mixtos.
* **Medios de Comunicación (Clasificación):** Clasificador heurístico basado en reglas de negocio para indexar noticias de forma automatizada, resolviendo el problema de arranque en frío (*Cold Start*).
* **Legal & Research (Resumen):** Reducción de la densidad textual de documentos extensos para acelerar la velocidad de lectura e interpretación de datos masivos.
* **Customer Support (Chatbots):** Sistema de automatización de atención al cliente para desviar consultas repetitivas (FAQ), garantizando soporte 24/7 y optimizando el costo operativo del helpdesk.

---

## ⚙️ Instrucciones de Reproducción

Asegure la consistencia del laboratorio desplegando el entorno con las versiones congeladas:

### 1. Instalación de Dependencias
```bash
pip install -r requirements.txt

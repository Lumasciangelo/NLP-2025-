# 🎯 Proyecto Final NLP - RAG y Agente Inteligente sobre Cascadia

Este proyecto implementa un sistema **RAG** (*Retrieval-Augmented Generation*) y posteriormente un **agente inteligente con herramientas personalizadas** para responder preguntas y realizar tareas basadas en información sobre el juego de mesa **Cascadia**.

El trabajo fue realizado como **proyecto final** de la materia *Procesamiento del Lenguaje Natural* en la Tecnicatura Universitaria en Inteligencia Artificial (UNR).

---

## 📌 Objetivo
El objetivo principal fue **integrar un pipeline de procesamiento de lenguaje natural** que:
1. **Recupere información relevante** desde un conjunto de documentos del juego Cascadia.
2. **Genere respuestas contextuales** usando un modelo de lenguaje.
3. **Implemente herramientas personalizadas** que permitan a un agente inteligente ejecutar consultas más complejas.

---

## 🔄 Flujo de Trabajo

### 1. RAG (Retrieval-Augmented Generation)
- **Ingesta de datos**: Se recolectaron y limpiaron documentos de texto (manual, reseñas, descripciones).
- **Preprocesamiento**: Normalización, eliminación de stopwords, lematización.
- **Vectorización**: Generación de embeddings con modelo de lenguaje.
- **Búsqueda semántica**: Recuperación de fragmentos relevantes.
- **Generación de respuestas**: Uso del contexto recuperado para responder preguntas desde tres bases de datos diferentes: vectorial, tabular, y de ralacional.

### 2. Agente Inteligente con Tools
- Se crearon herramientas (*tools*) para acceder a funciones como:
  - Consulta a base vectorial.
  - Análisis de estadísticas del juego (tabular).
  - Consulta a la base de datos de grafos (relacional).
- Un agente orquestó el uso de estas herramientas para resolver consultas complejas.

---

## 📂 Dataset y Fuentes
Los datos provienen de:
- **Reglamento oficial de Cascadia**.
- **Reseñas de sitios especializados**.
- **Opiniones de usuarios en foros**.
- **Datos estadísticos** (diseñadores, calificaciones, partidas registradas).

Se realizó una limpieza exhaustiva para descartar archivos irrelevantes o con errores.

---

## 🛠 Tecnologías Utilizadas
- **Google Colab**
- **LangChain** (para orquestar RAG y agente)
- **Gemini API / Modelos de lenguaje**
- **ChromaDB** (almacenamiento vectorial)
- **NLTK / spaCy** (procesamiento de texto)
- **Pandas / NumPy** (manejo de datos)

---

## 📊 Resultados
El sistema puede responder preguntas sobre el reglamento, estrategias y detalles del juego.

El agente inteligente ejecuta búsquedas y análisis de forma autónoma utilizando las tools implementadas.

El RAG devuelve respuestas más precisas que un modelo sin recuperación contextual.

---
## ✨ Autor
**Lucía Masciángelo**
T.U.I.A - FCEIA - UNR
2025

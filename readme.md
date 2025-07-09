# 📚 Análisis y Recomendación de Películas y Series de Netflix

Este repositorio contiene dos notebooks en Jupyter Notebook (.ipynb) para análisis y generación de sistemas de recomendación basados en contenido, utilizando datos de películas y series de Netflix actualizados hasta 2025.

---

## 1️⃣ Netflix_Recommendation_System_Documented_Spanish.ipynb

✅ **Objetivo:**
Implementar un sistema de recomendación basado en contenido usando el campo de **descripción** de cada título para encontrar similitudes.

✅ **Características:**
- Limpieza básica (elimina nulos en `description`).
- Vectorización de texto con **TF-IDF**.
- Cálculo de **Similitud de Coseno** entre descripciones.
- Función de recomendación: sugiere títulos similares dado uno de entrada.
- Explicaciones en español, celda por celda.

✅ **Uso esperado:**
Ideal para probar filtrado basado en contenido con un solo CSV de catálogo (como `netflix_titles.csv` o el fusionado `netflix_dataset_2025.csv`).

---

## 2️⃣ Netflix_Analisis_Completo_2025.ipynb

✅ **Objetivo:**
Integrar y analizar el catálogo completo de Netflix hasta 2025, fusionando dos archivos separados (películas y series) en un solo dataset listo para análisis.

✅ **Características:**
- Carga dos archivos CSV:
  - `netflix_movies_detailed_up_to_2025.csv`
  - `netflix_tv_shows_detailed_up_to_2025.csv`
- Agrega la columna `type` para distinguir entre Movie y TV Show.
- Fusiona ambos datasets en uno solo y lo guarda como:
  - **netflix_dataset_2025.csv**
- Realiza carga del nuevo CSV fusionado y análisis exploratorio:
  - Limpieza de nulos en `description`.
  - Distribución Películas vs Series.
  - Distribución por año de estreno.
  - Conteo de producciones por país.
- Código bien documentado en español, explicando cada paso.

✅ **Uso esperado:**
Permite consolidar y analizar el catálogo de Netflix actualizado, y dejar un solo CSV listo para otros análisis o para usar en sistemas de recomendación.

---

## 📂 Estructura esperada del repositorio

📁 DatasetViejo/ <br>
├── netflix_movies_detailed_up_to_2025.csv<br>
├── netflix_tv_shows_detailed_up_to_2025.csv<br>
└── netflix_dataset_2025.csv (generado)<br>
📁 Notebooks/<br>
├── Netflix_Recommendation_System_Documented_Spanish.ipynb<br>
└── Netflix_Analisis_Completo_2025.ipynb

---

## 🚀 Cómo usar

1. Coloca los CSV originales en la carpeta correspondiente.  
2. Abre **Netflix_Analisis_Completo_2025.ipynb** y ejecútalo para fusionar los CSV y generar el dataset combinado.  
3. Abre **Netflix_Recommendation_System_Documented_Spanish.ipynb** para probar el sistema de recomendación usando el CSV combinado (`netflix_dataset_2025.csv`).  

---

## ✨ Autor
Carolina Arias Reyes
Desarrollado como parte de prácticas de análisis de datos y sistemas de recomendación usando Python y Jupyter Notebook.

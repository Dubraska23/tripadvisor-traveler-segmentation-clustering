# 🌍 Traveler Profile Segmentation: Tripadvisor Reviews
### Clustering Comparativo (K-Means vs. DBSCAN) y Reducción de Dimensionalidad (PCA)

Este proyecto desarrolla un análisis de segmentación de mercado basado en las preferencias de consumo de viajeros. A través de técnicas de aprendizaje no supervisado, se identifican perfiles de usuario según sus valoraciones en diversas categorías (parques, museos, servicios, etc.), permitiendo una personalización estratégica de la oferta turística.

---

## 🛡️ Visión de Gobierno de Datos y Gestión de Outliers
Desde la perspectiva de **Data Governance**, este análisis aborda retos críticos en la gestión de metadatos no estructurados y comportamiento de usuario:

1. **Gobernanza de Metadatos Conductuales:** Estandarización de las categorías de reseña para asegurar que las etiquetas de "preferencia" sean consistentes y comparables a través de todo el dataset.
2. **Gestión de Ruido y Outliers (DBSCAN):** Implementación de algoritmos basados en densidad para identificar y aislar "ruido" (usuarios con comportamientos atípicos). Esto garantiza que los clusters principales no se vean sesgados por datos anómalos, mejorando la integridad del activo de información.
3. **Calidad y Normalización:** Protocolo de escalado de variables para asegurar que las diferencias en el volumen de reseñas por categoría no distorsionen la métrica de distancia euclídea.
4. **Validación de Estabilidad:** Comparativa técnica entre **K-Means** (segmentación global estable) y **DBSCAN** (detección de micro-segmentos densos), facilitando una toma de decisiones gobernada sobre qué modelo aplicar según el objetivo de negocio.

---

## 🎯 Capacidades Técnicas
- **K-Means Clustering:** Definición de perfiles de usuario equilibrados e interpretables para segmentación de mercado masiva.
- **DBSCAN (Density-Based Spatial Clustering):** Detección de grupos de alta densidad y detección automática de valores atípicos (outliers).
- **PCA (Análisis de Componentes Principales):** Reducción de 10 dimensiones a componentes principales para optimizar la visualización y el rendimiento del algoritmo.
- **Análisis de Perfiles:** Interpretación de los centroides para asignar etiquetas de negocio (ej. "Amantes de la Cultura", "Turistas de Ocio", "Viajeros de Naturaleza").

---

## 📊 Fuente de los Datos
El proyecto utiliza el dataset de reseñas de Tripadvisor enfocado en destinos de Asia oriental.
- **Archivo de datos:** `tripadvisor_review.csv`.
- **Contenido:** Calificaciones de usuarios en 10 categorías (parques, museos, teatros, jardines, etc.).

---

## 🛠️ Stack Tecnológico
- **Lenguaje:** Python 3.10+
- **Machine Learning:** `Scikit-learn` (KMeans, DBSCAN, PCA, StandardScaler).
- **Análisis de Datos:** `Pandas`, `Numpy`.
- **Visualización:** `Seaborn`, `Matplotlib`.

---

## 🚀 Cómo utilizar este proyecto
1. Clona el repositorio.
2. Coloca el archivo `tripadvisor_review.csv` en la carpeta raíz.
3. Instala las dependencias:
   ```bash
   pip install pandas numpy scikit-learn seaborn matplotlib
4. Ejecuta el notebook tripadvisor_clustering_analysis.ipynb para visualizar la comparación de modelos y los perfiles de usuario resultantes.

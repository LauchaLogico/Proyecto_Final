## Entendimiento de la situación actual <br/>

## Objetivos <br/>
1. Generar un sistema de recomendaciones de restaurantes en base a los gustos/preferencias del usuario
2. Hacer un analisis detallados de los restaurantes con el fin de generar una API de consulta
3. Realizar un analisis detallados de los rubros Hoteles y Restaurantes
4. Analizar como afectan los otros rubros afines al turismo

 
## Alcance <br/>

📌 Contexto

El presente proyecto busca analizar y comparar las reseñas de negocios en Estados Unidos utilizando datos de Yelp y Google Maps. Se investigará la percepción de los usuarios sobre hoteles, restaurantes y otros negocios del sector turismo y ocio, aplicando técnicas de análisis de datos y machine learning.

📍 Alcance del Proyecto

Este análisis estará enfocado en:

✔ Consolidación de datos de múltiples fuentes: Unificación de información proveniente de Yelp y Google Maps en una base de datos estructurada.

✔ Exploración y limpieza de datos: Identificación y tratamiento de valores nulos, duplicados y outliers para asegurar la calidad de la información.

✔ Análisis de tendencias y reputación: Evaluación de calificaciones, distribución de reseñas y variaciones en el tiempo.

✔ Procesamiento de lenguaje natural (NLP): Aplicación de modelos para extraer insights a partir del contenido de las reseñas.

✔ Identificación de oportunidades de expansión: Análisis de ubicación para sugerir nuevas aperturas de negocios.

✔ Desarrollo de un dashboard interactivo: Visualización de métricas clave para facilitar la interpretación de los resultados.

✔ Implementación de un sistema de recomendación: Basado en preferencias y reseñas previas de los usuarios.


🛑 Fuera de Alcance (Posibles Extensiones Futuras)

🔸 Integración con redes sociales y otros factores externos (tendencias, valoraciones en otras plataformas).

🔸 Análisis en tiempo real de nuevas reseñas.

🔸 Modelos avanzados de predicción de demanda por ubicación.

🔸 Expansión del análisis a mercados fuera de EE.UU.

##  KPIs <br/>
Categorías de KPIs:

Calidad y Percepción del Servicio

Engagement y Popularidad

Análisis de Sentimiento y Tendencias

Expansión y Recomendación de Nuevos Locales


🔹 1. Calidad y Percepción del Servicio

✔ Puntaje Promedio de Reseñas (Promedio de calificaciones en Yelp y Google Maps por negocio, ciudad, o categoría).

✔ Distribución de Calificaciones (% de reseñas con 1-5 estrellas para evaluar consistencia del servicio).

✔ Frecuencia de Reseñas Negativas (Cantidad de reseñas ≤ 2 estrellas por mes/año/localidad).

✔ Principales Motivos de Reclamos (Análisis NLP de palabras clave en reseñas negativas: "servicio lento", "mala atención", etc.)


🔹 2. Engagement y Popularidad

✔ Cantidad Total de Reseñas por Negocio/Categoría/Ubicación (Métrica de actividad y relevancia de cada local o ciudad.)

✔ Tasa de Crecimiento de Reseñas (Variación mensual/anual de nuevas reseñas, ideal para ver tendencias en el tiempo.)

✔ Cantidad de Votos en Reseñas (Muestra cuáles reseñas generan mayor engagement, útil para identificar críticas con impacto.)

✔ Negocios con Mayor/Peor Crecimiento de Reseñas (Ayuda a detectar tendencias positivas o problemas emergentes.)


🔹 3. Análisis de Sentimiento y Tendencias

✔ Sentimiento Promedio de las Reseñas (Aplicación de NLP para clasificar comentarios en positivo, neutro o negativo.)

✔ Comparación de Sentimientos entre Yelp y Google Maps (Detectar diferencias en percepción según la plataforma.)

✔ Evolución del Sentimiento a lo Largo del Tiempo (Ver si la reputación de un negocio mejora o empeora con los meses/años.)

✔ Palabras Clave más Mencionadas en Reseñas Positivas y Negativas (Extraer insights de lo que más valoran o critican los clientes.)


🔹 4. Expansión y Recomendación de Nuevos Locales

✔ Ciudades/Barrios con Mayor Demanda Potencial (Análisis de cantidad de reseñas y sentimiento positivo en zonas con baja oferta de locales.)

✔ Categorías de Negocios en Crecimiento o Declive (Basado en la variación del número de reseñas y calificación promedio a lo largo del tiempo.)

✔ Ranking de Locales Mejor Valorados y Peor Valorados por Ciudad (Para evaluar benchmarking y oportunidades de mejora.)

✔ Sistema de Recomendación de Restaurantes (Basado en historial de calificaciones y preferencias del usuario.)


💡 Extras que Pueden Potenciar el Dashboard:

📍 Mapa Interactivo con Hotspots de Restaurantes Populares y Mal Calificados

📊 Comparación de Competencia en una Misma Categoría (Ej: mejores hamburgueserías en Nueva York según Yelp vs. Google.)

📈 Predicción de Tendencias (Usar modelos de ML para prever cuáles categorías o ubicaciones serán más demandadas.)


## Solución propuesta <br/>


📌 Enfoque Metodológico

Para cumplir con los objetivos del proyecto, utilizaremos una metodología ágil basada en Scrum, dividiendo el desarrollo en sprints semanales con entregables definidos. Se trabajará en equipo, asignando roles y tareas específicas para optimizar la ejecución del proyecto.


🛠 Tareas y Metodología

1️⃣ Recopilación y Estructuración de Datos

✔ Consolidación de datasets de Yelp y Google Maps.

✔ Creación de un Data Warehouse para almacenamiento estructurado.

✔ Evaluación de la calidad y confiabilidad de los datos.

✔ Definición de estrategias para la limpieza y transformación de datos.


2️⃣ Exploración y Análisis de Datos

✔ Análisis exploratorio de datos (EDA) para detectar patrones y relaciones.

✔ Identificación de datos faltantes, duplicados y outliers.

✔ Aplicación de técnicas de procesamiento de lenguaje natural (NLP) para analizar reseñas.


3️⃣ Desarrollo de Modelos de Machine Learning

✔ Implementación de modelos de Análisis de Sentimiento.

✔ Construcción de un Sistema de Recomendación basado en reseñas previas de los usuarios.

✔ Predicción de tendencias de negocios en crecimiento o declive.


4️⃣ Desarrollo del Dashboard Interactivo

✔ Diseño e implementación de KPIs clave.

✔ Visualización de insights sobre desempeño de negocios.

✔ Desarrollo de un mapa interactivo para recomendaciones de expansión.


5️⃣ Arquitectura Tecnológica (Stack)

✔ Almacenamiento y Procesamiento: PostgreSQL, Google BigQuery.

✔ Limpieza y transformación: Pandas, PySpark.

✔ NLP y Machine Learning: Scikit-learn, NLTK, TensorFlow.

✔ Desarrollo del Dashboard: Streamlit, Tableau o Power BI.

✔ Despliegue: Render para la API y GitHub para control de versiones.


⏳ Planificación y Estimación de Tiempos

Semana 1:

📌 Recopilación de datos, exploración y análisis preliminar.

📌 Definición del stack tecnológico.

📌 Primera prueba de limpieza y transformación de datos.


Semana 2:

📌 Desarrollo del Data Warehouse.

📌 EDA y Análisis de Sentimiento.

📌 Implementación de los primeros modelos de Machine Learning.


Semana 3:

📌 Ajuste de modelos y generación de insights.

📌 Diseño y desarrollo del dashboard interactivo.

📌 Integración del sistema de recomendación.


Semana 4:

📌 Ajustes finales y optimización.

📌 Presentación de resultados y conclusiones.


🕒 Diagrama de Gantt: Se detallará en función de las fechas específicas de cada entrega.


📊 Análisis de Calidad de Datos y Metadatos

✔ Fuentes de Datos: Yelp, Google Maps.

✔ Tipos de Datos: Texto (reseñas), numéricos (puntuaciones), geoespaciales 
(coordenadas).

✔ Fecha de Adquisición: Datos descargados en 2025.

✔ Frecuencia de Actualización: Datos estáticos, pero con posibilidad de 
actualización futura.

✔ Método de Adquisición: Archivos JSON y Parquet procesados en DataFrames.


💡 Conclusión

El enfoque propuesto permitirá cumplir con los objetivos del proyecto dentro del tiempo establecido, asegurando la calidad de los datos y la validez de los insights generados. 🚀
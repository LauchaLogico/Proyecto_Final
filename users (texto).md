# Análisis Exploratorio de Datos - Usuarios

Este documento presenta un análisis exploratorio del dataset de usuarios, destacando patrones clave y posibles pasos a seguir.

## 1. Descripción del Dataset

- **Cantidad de filas**: 2,105,597 usuarios.
- **Cantidad de columnas**: 22.
- **Tipo de datos**: Múltiples variables numéricas relacionadas con interacciones y actividad de los usuarios.

## 2. Estadísticas Generales

### 2.1 Columnas de Actividad del Usuario

- `review_count` (número de reseñas):
  - **Media**: 28.5 reseñas.
  - **Mínimo**: 0 reseñas.
  - **Máximo**: 17,473 reseñas.
  - **75% de los usuarios tienen ≤19 reseñas**, lo que indica que hay pocos usuarios con una cantidad muy alta.

- `useful`, `funny`, `cool` (cantidad de votos recibidos en estas categorías):
  - **Valores extremos**: Hay usuarios con más de 200,000 votos en "useful" o "cool".
  - **Mediana en 0**: La mayoría de los usuarios no han recibido votos.

- `fans` (número de seguidores):
  - **Mediana: 0** (la mayoría de los usuarios no tienen seguidores).
  - **Máximo: 12,497 seguidores**, lo que indica la presencia de usuarios influyentes.

### 2.2 Puntuación de los Usuarios

- `average_stars` (calificación promedio):
  - **Media: 3.64 estrellas**.
  - **Mínimo: 1.0**, **Máximo: 5.0**.
  - **El 75% de los usuarios tiene 4.5 estrellas o menos**.

### 2.3 Columnas de "Compliments"

- Las columnas como `compliment_hot`, `compliment_more`, etc., tienen una **media muy baja y una mediana de 0**, lo que sugiere que la mayoría de los usuarios no reciben estos cumplidos.
- Sin embargo, algunos usuarios tienen valores extremadamente altos (`compliment_funny` llega a 99,670), lo que sugiere **outliers** o usuarios muy activos/populares.

## 3. Posibles Análisis a Realizar

### 3.1 Detección de Usuarios Activos vs. Inactivos
- Definir un umbral para considerar a un usuario como "activo" (por ejemplo, más de X reseñas o interacciones).

### 3.2 Análisis de Usuarios Influyentes
- Filtrar usuarios con **más fans** o **mayor número de votos "useful" o "cool"**.

### 3.3 Detección de Outliers
- Visualizar distribución con:
  ```python
  import matplotlib.pyplot as plt
  df[['useful', 'funny', 'cool']].boxplot()
  plt.show()
  ```

### 3.4 Segmentación de Usuarios
- ¿Cuántos usuarios son "nuevos" (por `yelping_since`) vs. experimentados?
- ¿Los usuarios con más reseñas también tienen más votos?

---

Este README servirá como guía para el análisis de usuarios en la plataforma. Se recomienda complementar con visualizaciones y modelos de segmentación para obtener más insights.

Cualquier ajuste o nueva información puede agregarse a medida que avanzamos en el análisis.


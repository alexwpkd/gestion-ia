# Análisis de Tendencias de Búsqueda con Google Trends y BigQuery

Este proyecto tiene como objetivo identificar los términos de búsqueda con mayor crecimiento en Estados Unidos y Chile durante los últimos 30 días, utilizando datos públicos de Google Trends. El análisis se realiza mediante consultas SQL en BigQuery y visualización con Python (Pandas, Matplotlib).

---

## Componentes del sistema

- **Consulta SQL en BigQuery**: Extracción de términos en crecimiento (`top_rising_terms` e `international_top_rising_terms`).
- **Autenticación en Google Colab**: Acceso a BigQuery mediante API.
- **Procesamiento con Pandas**: Transformación de resultados a DataFrames.
- **Visualización**: Gráficos de barras horizontales para los 20 términos con mayor crecimiento promedio.

---

## Tecnologías utilizadas

- Python 3  
- Pandas / Matplotlib  
- Google BigQuery (API)  
- Google Colab  
- Google Cloud Platform

---

## Pipeline implementado

| Etapa | Descripción |
|-------|-------------|
| 1. Autenticación | Autenticación en Google Colab con cuenta de Google. |
| 2. Cliente BigQuery | Creación del cliente para ejecutar consultas SQL. |
| 3. Definición de consultas | SQL para calcular el promedio de `percent_gain` en los últimos 30 días, agrupado por término. |
| 4. Ejecución | Envío de consultas a BigQuery. |
| 5. Obtención de resultados | Recuperación de filas y conversión a DataFrame. |
| 6. Visualización | Gráfico de barras horizontales mostrando los términos más destacados. |

---

## Estructura del repositorio

---

## Cómo ejecutar el sistema

1. Clonar el repositorio  
   `git clone https://github.com/usuario/google-trends-analysis.git`

2. Abrir el notebook en Google Colab o en un entorno con acceso a BigQuery.

3. Configurar el `project_id` con el ID de tu proyecto de Google Cloud.

4. Ejecutar las celdas en orden:
   - Autenticación
   - Creación del cliente BigQuery
   - Definición y ejecución de consultas para EE.UU. y Chile
   - Visualización de resultados

5. Los resultados se mostrarán como DataFrames y gráficos dentro del notebook.

---

## Ejemplo de salida (EE.UU.)

| Término                | Crecimiento promedio (%) |
|------------------------|--------------------------|
| men’s march madness    | 41400.0                  |
| women’s march madness  | 38714.91                 |
| easter traditions      | 24725.0                  |
| ...                    | ...                      |

Se genera un gráfico de barras horizontales con los 20 términos principales.

---

## Documentación adicional

- [Google Trends Public Datasets en BigQuery](https://cloud.google.com/bigquery/public-data/google-trends)
- [API de BigQuery para Python](https://cloud.google.com/bigquery/docs/reference/libraries)

---

## Equipo

- Integrante 1 – Alexis Rios 
- Integrante 2 – Guillermo Herreros
- Integrante 3 – BAHIRON  ARELLANO 
- 

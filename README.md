# Tuberculosis Global Dashboard 

Análisis exploratorio y dashboard interactivo de casos de tuberculosis a nivel mundial, desarrollado como caso práctico para la Organización Mundial de la Salud.

## Objetivo

Apoyar al consejo directivo de la OMS en la comprensión de la situación actual de tuberculosis, sus tendencias por región e identificar países de éxito y países que requieren mayor apoyo, en el marco de las metas ONU 2025:

- Reducción del **50%** en tasa de incidencia (vs 2015)
- Reducción del **75%** en número de muertes (vs 2015)


## Proceso de datos

La limpieza se realizó en **Python (Google Colab)** sobre el dataset `who` de tidyr, que contiene casos de TB desagregados por país, año, género, grupo de edad y método de diagnóstico (1995–2013).

Las transformaciones principales fueron:

- Conversión de formato ancho a formato largo (tidy data)
- Separación de la columna de variables en: género, método diagnóstico y grupo de edad
- Join con tabla de población para calcular tasas de incidencia
- Eliminación de valores nulos y registros sin casos reportados

## Dashboard Power BI

El dashboard incluye las siguientes visualizaciones:

| Visual | Descripción |
|---|---|
| Mapa coroplético | Casos o tasa por 100,000 habitantes |
| Top 10 países | Países con mayor carga de Tuberculosis |
| Tendencia global | Evolución de casos 1995–2013 |
| Distribución por género | Proporción de casos masculino vs femenino |
| Pirámide de edad | Casos por grupo de edad |

Todos los visuales son interactivos y se filtran con segmentadores de año, género y método de diagnóstico.

## Tecnologías

- Python 3 / Google Colab — limpieza de datos
- Pandas — transformación y análisis
- Power BI Desktop — visualización y dashboard

## Dashboard

[Abrir dashboard en Power BI](https://app.powerbi.com/groups/me/reports/a70d17c8-31b0-4a47-ad72-a255b12ccaee/778c22c0e4d40b20d5c3?experience=power-bi)

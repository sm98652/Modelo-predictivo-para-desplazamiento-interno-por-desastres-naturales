# Predicción de Desplazamiento Interno Asociado a Eventos Climáticos

## Descripción
Proyecto de analítica predictiva desarrollado en el marco de una hackathon, orientado a estimar el riesgo de eventos climáticos y su potencial impacto sobre el desplazamiento interno a nivel municipal en Colombia.
El proyecto busca explorar cómo la integración de información climática, ambiental, territorial y socioeconómica puede contribuir a anticipar escenarios de afectación y apoyar la gestión preventiva del riesgo de desastres.

## Metodología
Se integraron múltiples fuentes de información para caracterizar las condiciones de los municipios, incluyendo:
* Información meteorológica y climática.
* Biomas y regiones naturales.
* Características geográficas y topográficas.
* Condiciones de vivienda.
* Variables demográficas y de vulnerabilidad socioeconómica.
* Historial de eventos climáticos y población afectada.
El proceso incluyó integración y limpieza de datos, construcción de variables (*feature engineering*), análisis exploratorio, validación temporal y modelamiento predictivo.

Para el modelamiento se utilizó LightGBM, abordando dos componentes:

1. **Predicción de ocurrencia de eventos climáticos**, formulada como un problema de clasificación.
2. **Estimación del número de personas desplazadas**, formulada como un problema de regresión.

## Resultados

El modelo de clasificación alcanzó un **AUC-ROC de 0.74**, mientras que el modelo de regresión obtuvo un **RMSE de 1.325**.
Estos resultados permitieron desarrollar un enfoque de analítica predictiva orientado a la **identificación anticipada de territorios con potencial riesgo de afectación y desplazamiento**, con posibles aplicaciones en procesos de gestión y planificación del riesgo de desastres.

## Estructura del proyecto

```text
├── data/
│   ├── raw/
│   └── processed/
├── notebooks/
├── src/
│   ├── data/
│   ├── features/
│   └── models/
├── results/
├── requirements.txt
└── README.md
```

## Enfoque

Más allá del componente predictivo, el proyecto busca mostrar cómo la ciencia de datos puede utilizarse para transformar múltiples fuentes de información en evidencia útil para comprender vulnerabilidades territoriales y apoyar la toma de decisiones frente al riesgo de desastres.

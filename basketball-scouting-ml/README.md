# Basketball Scouting ML

Sistema de clasificación de jugadores de la NBA basado en consistencia de rendimiento,
desarrollado como proyecto final de la materia Aprendizaje Automático.

## Descripción

Este proyecto construye un modelo de machine learning que clasifica jugadores de la NBA
como **consistentes** o **volátiles** a partir de la variabilidad estadística en sus
últimos 10 partidos jugados.

La métrica de consistencia se basa en el **Coeficiente de Variación (CV)** de
estadísticas clave (puntos, asistencias, rebotes), generando una etiqueta binaria
según un umbral definido sobre la mediana del CV del conjunto.

## Estructura del proyecto
## Dataset

`nba_game_logs_2024_25.csv` — registros partido a partido de jugadores NBA,
temporada 2024-25. Fuente: NBA Stats API.

## Modelos utilizados

- Regresión Logística
- SVM (kernel RBF)
- K-Means (análisis exploratorio)
- PCA (reducción de dimensionalidad)

## Autor

Ayrton Correa Vargas — Tecnicatura en Ciencia de Datos e Inteligencia Artificial

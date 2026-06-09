# Descripción y Formulación del Objetivo

## Contexto

El scouting deportivo es el proceso de evaluación de jugadores para la toma de
decisiones en equipos profesionales. En la NBA, contar con jugadores consistentes
es clave para la planificación táctica. Este proyecto propone automatizar la
clasificación de jugadores según su consistencia de rendimiento utilizando
técnicas de Aprendizaje Automático.

## Objetivo General

Desarrollar un modelo de clasificación que permita identificar si un jugador de
la NBA es **consistente** o **volátil** en base a la variabilidad de sus
estadísticas en sus últimos 10 partidos jugados.

## Objetivos Específicos

- Definir una métrica de consistencia basada en el **Coeficiente de Variación (CV)**
  de estadísticas clave: puntos, asistencias y rebotes.
- Construir la variable objetivo (etiqueta binaria) clasificando cada jugador como
  `consistente` o `volátil` según un umbral definido sobre la mediana del CV del conjunto.
- Explorar y preprocesar el dataset de game logs NBA 2024-25.
- Entrenar y comparar modelos de clasificación: Regresión Logística y SVM.
- Evaluar el rendimiento de los modelos con métricas apropiadas (accuracy, F1-score).

## Tipo de Problema

Clasificación binaria supervisada.

## Variable Objetivo

| Etiqueta | Criterio |
|----------|----------|
| `consistente` | CV promedio por debajo de la mediana del conjunto |
| `volátil` | CV promedio por encima de la mediana del conjunto |

## Modelos a Utilizar

- Regresión Logística
- SVM con kernel RBF
- PCA para reducción de dimensionalidad (preprocesamiento)
- K-Means para análisis exploratorio de agrupaciones

## Dataset

`nba_game_logs_2024_25.csv` — registros partido a partido de jugadores NBA,
temporada 2024-25. Incluye estadísticas de puntos, rebotes, asistencias, minutos
jugados, entre otras.

# Predicción de Incidentes de Seguridad en Perforación Diamantina — Explomin del Perú S.A.C.

Proyecto de investigación aplicada en Inteligencia Artificial. Evalúa si modelos de aprendizaje automático supervisado (Regresión Logística y Random Forest) permiten predecir la ocurrencia de un incidente de seguridad (`hubo_incidente`) en un turno de perforación diamantina, a partir de variables operativas registradas en partes diarios.

## 1. Problema
Explomin del Perú S.A.C. no cuenta con un mecanismo analítico que anticipe, a partir de sus partes diarios de operación, qué turnos de perforación tienen mayor probabilidad de registrar un incidente de seguridad (casi accidente o incidente menor).

## 2. Objetivo
Entrenar y evaluar experimentalmente modelos de clasificación binaria (Regresión Logística, Random Forest) para predecir `hubo_incidente`, documentando el desempeño obtenido.

## 3. Dataset
- Archivo: `data/explomin_dataset.csv`
- 1,000 registros (turnos), 25 columnas, periodo 2023–2025.
- Variable objetivo derivada: `hubo_incidente` (1 si `incidente_seguridad` ≠ "Ninguno").
- Procedencia: dataset parametrizado a partir de fuentes públicas y verificables sobre Explomin del Perú S.A.C. (ver informe, sección 16.1).

## 4. Cómo obtener los datos
El archivo `explomin_dataset.csv` ya está incluido. No requiere descarga externa.

## 5. Cómo ejecutar el código
1. Abrir `notebooks/Colab.ipynb` en Google Colab.
2. Ejecutar todas las celdas en orden (Runtime → Run all).
3. El notebook carga `data/explomin_dataset.csv`

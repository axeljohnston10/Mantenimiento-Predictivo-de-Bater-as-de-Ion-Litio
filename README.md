# 🔋 Mantenimiento Predictivo: Análisis de Degradación de Baterías de Ion-Litio

Este proyecto aplica técnicas de **Data Science** y **Machine Learning** para predecir la vida útil restante (**RUL - Remaining Useful Life**) y el estado de salud (**SOH - State of Health**) de baterías de litio, utilizando datos de sensores eléctricos y térmicos.

## 🎯 Objetivo del Proyecto
Desarrollar un modelo predictivo capaz de estimar cuántos ciclos de vida le quedan a una celda de batería basándose en su comportamiento físico durante los procesos de carga y descarga. Esto tiene aplicaciones críticas en vehículos eléctricos y sistemas de almacenamiento de energía renovable.

## 🛠️ Stack Tecnológico
- **Lenguaje:** Python (Desarrollado en entorno Mac M1).
- **Bibliotecas de Análisis:** `Pandas`, `NumPy`.
- **Visualización:** `Seaborn`, `Matplotlib`.
- **Machine Learning:** `Scikit-Learn` (Random Forest Regressor).
- **Automatización:** API de Kaggle (`kagglehub`).

## 🔬 Análisis
A diferencia de un análisis de datos convencional, este proyecto considera:
1. **Correlación Física:** Identificación de cómo la temperatura de descarga (`disT`) y el voltaje afectan la salud de la batería.
2. **Degradación No Lineal:** Uso de modelos de ensamble (Random Forest) para capturar la pérdida de capacidad que no sigue un patrón lineal simple.
3. **Validación:** El modelo fue validado comparando los valores reales contra las predicciones, obteniendo una alta precisión (R² Score) 90.02%.



## 📊 Resultados Clave
- **Variable más influyente:** El ciclo de vida y la capacidad de descarga demostraron ser los predictores más fuertes del SOH.
- **Precisión del Modelo:** Se logró una predicción del RUL con un error promedio mínimo, permitiendo anticipar fallos en las celdas. VEl modelo de Random Forest logró explicar el 90% de la varianza en la vida útil restante de las baterías. Esto demuestra que las variables físicas seleccionadas (voltaje, corriente y temperatura) son predictores robustos para el mantenimiento predictivo.

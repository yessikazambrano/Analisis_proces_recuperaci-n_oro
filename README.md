# ⚒️ Análisis de proceso de flotación para recuperación de oro con Gradient Boosting Regressor

Este proyecto estudia el proceso de flotación metalúrgica, identificando variables críticas y segmentando las etapas **rougher** y **cleaner** para evaluar su impacto en la calidad del concentrado de oro (Au).  

Se implementaron distintos modelos de regresión: **RandomForest, LinearRegression y GradientBoosting**, evaluando métricas de error cuadrático y error absoluto medio.

---

## 📐 Metodología
- **Preparación de datos**  
  - Limpieza de valores nulos y outliers.  
  - Normalización de variables numéricas para mejorar estabilidad en el entrenamiento.  
  - Segmentación de etapas (*rougher* y *cleaner*) para análisis diferenciado.  

- **División del dataset**  
  - Train/Test split en proporción 80/20.  
  - Validación cruzada para asegurar consistencia en los resultados.  

- **Modelos evaluados**  
  - **Linear Regression**: como baseline para medir mejoras.  
  - **Random Forest Regressor**: robusto ante variabilidad, útil para identificar importancia de variables.  
  - **Gradient Boosting Regressor**: modelo final, optimizado con *GridSearchCV* para hiperparámetros clave (learning rate, max depth, n_estimators).  

---

## 📊 Resultados obtenidos
- **Mejor modelo:** Gradient Boosting Regressor  
- **Error cuadrático medio (MSE):** 5.53% → indica baja dispersión de errores.  
- **Error absoluto medio (MAE):** 10.10% → refleja precisión aceptable en predicciones individuales.  

---

## ✨ Contribuciones del modelo
- Precisión y confiabilidad en las predicciones.  
- Identificación de variables críticas en el proceso de flotación.  
- Segmentación de etapas para un análisis más detallado.  
- Consolidación del modelo como la opción más adecuada para este conjunto de datos.  

---

## 📌 Interpretación técnica
El **Gradient Boosting Regressor** logró capturar relaciones no lineales entre las variables del proceso metalúrgico, superando al baseline de regresión lineal y al Random Forest en métricas de error.  
La segmentación de etapas (*rougher* y *cleaner*) permitió entender cómo cada fase impacta en la calidad del concentrado, aportando información clave para optimizar la recuperación de oro.  

---

⭐ **Conclusión:** Este análisis demuestra cómo los modelos de Machine Learning pueden optimizar procesos metalúrgicos y mejorar la recuperación de minerales valiosos.  

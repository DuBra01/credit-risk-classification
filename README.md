# credit-risk-classification
 📊 Análisis de Clasificación de Riesgo Crediticio 🚀

📌 Descripción del Proyecto

Este proyecto implementa un modelo de Regresión Logística para predecir el estado de un préstamo (saludable o de alto riesgo). Se utiliza un conjunto de datos con información financiera de los prestatarios y se aplican técnicas de aprendizaje supervisado para entrenar y evaluar el modelo. 🔍📈

🛠️ Pasos Realizados

1️⃣ Carga y Preparación de Datos

✅ Se cargó el archivo lending_data.csv en un DataFrame de Pandas.
✅ Se separaron las variables en:

X (features): Características del prestatario.

y (target): Estado del préstamo (0: saludable, 1: alto riesgo).
✅ Se dividió el dataset en conjuntos de entrenamiento y prueba.

2️⃣ Entrenamiento del Modelo con Datos Originales

🚀 Se instanció y entrenó un modelo de Regresión Logística con los datos originales.
📊 Se evaluó el rendimiento utilizando:

Balanced Accuracy Score 🎯

Matriz de confusión 📉

Reporte de clasificación 📑
⚠️ Se encontró un desequilibrio significativo en las clases (muchos préstamos saludables y pocos de alto riesgo), lo que afectaba la capacidad del modelo para detectar correctamente los préstamos de alto riesgo. ❌

3️⃣ Manejo del Desbalance con Oversampling

🔄 Se utilizó RandomOverSampler de imbalanced-learn para equilibrar las clases duplicando ejemplos de la clase minoritaria (1).
🎯 Se reentrenó el modelo con los datos balanceados.
📊 Se evaluó nuevamente el modelo con los mismos métricos.

4️⃣ Resultados y Conclusiones

✅ Balanced Accuracy Score mejoró a 0.9936 después del oversampling. 🚀
✅ Recall para los préstamos de alto riesgo aumentó al 99% 📈, indicando que el modelo ahora es mucho mejor detectando posibles incumplimientos.
⚠️ Se produjo un ligero aumento en los falsos positivos (préstamos saludables clasificados como riesgosos), lo que es un compromiso aceptable para minimizar préstamos incumplidos. 🔄

🏆 Conclusión Final

💡 La aplicación de RandomOverSampler mejoró significativamente la capacidad del modelo para detectar préstamos de alto riesgo, logrando un equilibrio adecuado entre sensibilidad y precisión. 🔥
🎯 Esto demuestra la importancia de abordar el desbalance de clases en problemas de clasificación para obtener predicciones más justas y útiles. 💪📊

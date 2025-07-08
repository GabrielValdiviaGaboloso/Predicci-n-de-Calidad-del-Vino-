🍷 Predicción de Calidad del Vino - Clasificación
📚 Descripción del Proyecto
Este proyecto se enfoca en predecir la calidad del vino tinto portugués “Vinho Verde” utilizando aprendizaje automático. Se trabaja con un dataset de clasificación multiclase, donde la calidad del vino (de 0 a 10) se ha simplificado en tres clases categóricas: bajo, medio y alto.

Aunque el modelo es sencillo, el desafío reside en que el conjunto de datos está desbalanceado: la mayoría de los vinos tienen calidad media, lo que dificulta la predicción de las clases minoritarias (bajo y alto).

🧪 Variables del Dataset
Entrada (características fisicoquímicas):

Acidez fija

Acidez volátil

Ácido cítrico

Azúcar residual

Cloruros

Dióxido de azufre libre

Dióxido de azufre total

Densidad

pH

Sulfatos

Alcohol

Salida (variable objetivo):

Calidad (convertida en clases: bajo, medio, alto)

🤖 Modelos Evaluados
Se compararon los siguientes modelos:

KNN Classifier

Logistic Regression

Random Forest (opcional, si fue evaluado también)

Se utilizó búsqueda de hiperparámetros, métricas de clasificación (accuracy, precision, recall, f1-score), matriz de confusión y curva ROC para evaluar el rendimiento de cada modelo.

📊 Resultados
✅ Mejor Modelo: Logistic Regression
Accuracy: 97%

Excelente rendimiento al clasificar correctamente la clase “medio”.

Soportado por curva ROC y AUC, mostrando un área elevada para esta clase.

❌ Debilidad: Desbalance de Clases
Ningún modelo logró predecir correctamente las clases "bajo" y "alto".

Estas clases contienen muy pocas muestras, lo que dificulta su aprendizaje por parte del modelo.

📈 Conclusión
✔️ El modelo Logistic Regression es el más adecuado para este problema, especialmente si se desea predecir correctamente la clase dominante (medio).

❌ Sin embargo, la clasificación de las clases minoritarias no es confiable, por lo tanto, el modelo no es robusto para todos los tipos de vino.

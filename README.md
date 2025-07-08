# Prediccion-de-Calidad-del-Vino-
Dataset de clasificación  de vinos
Descripción:
Este conjunto de datos está relacionado con las variantes tintas del vino portugués "Vinho Verde". Describe la cantidad de diversas sustancias químicas presentes en el vino y su efecto en su calidad. Los conjuntos de datos pueden considerarse como tareas de clasificación o regresión. Las clases están ordenadas y no equilibradas (por ejemplo, hay muchos más vinos normales que excelentes o deficientes). Su tarea consiste en predecir la calidad del vino utilizando los datos proporcionados.

Un proyecto sencillo pero desafiante: anticipar la calidad del vino.
La complejidad surge debido a que el conjunto de datos contiene menos muestras y presenta un alto desequilibrio.
¿Puedes superar estos obstáculos y construir un buen modelo predictivo para clasificarlos?

Este marco de datos contiene las siguientes columnas:

Variables de entrada (basadas en pruebas fisicoquímicas):\
1 - acidez fija\
2 - acidez volátil\
3 - ácido cítrico\
4 - azúcar residual\
5 - cloruros\
6 - dióxido de azufre libre\
7 - dióxido de azufre total\
8 - densidad\
9 - pH\
10 - sulfatos\
11 - alcohol\
Variable de salida (basada en datos sensoriales):\
12 - calidad (puntuación entre 0 y 10)


🏁 Conclusión del Análisis
✅ El mejor modelo evaluado fue Logistic Regression, con una precisión (Accuracy) del 97%. Este modelo mostró un rendimiento excelente al clasificar correctamente la clase "medio", que representa la gran mayoría de los datos.

❌ Sin embargo, ningún modelo fue capaz de predecir correctamente las clases "bajo" o "alto", debido a un fuerte desbalance de clases. Estas clases tienen muy pocas muestras en comparación con la clase "medio", lo que limita la capacidad de generalización del modelo hacia esas categorías.

📈 La curva ROC y los valores de AUC confirmaron que Logistic Regression es muy eficaz para distinguir la clase "medio", pero tiene bajo poder discriminativo para las otras clases.

🛠️ Recomendaciones
Aplicar técnicas de balanceo de clases como SMOTE o undersampling.

Recolectar más muestras para las clases minoritarias ("bajo" y "alto").

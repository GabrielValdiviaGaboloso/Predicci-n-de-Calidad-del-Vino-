
# 🍷 Predicción de Calidad del Vino - Clasificación

## 📚 Descripción del Proyecto

Este proyecto tiene como objetivo **predecir la calidad del vino tinto portugués “Vinho Verde”** a partir de características fisicoquímicas. El desafío principal radica en el **desbalance de clases**, ya que la mayoría de los vinos son de calidad media, mientras que los vinos de calidad baja o alta tienen muy pocas muestras.

Se trata de una tarea de **clasificación multiclase**, donde la variable `calidad` fue transformada en tres categorías: `bajo`, `medio` y `alto`.

---

## 🧪 Variables del Dataset

**Variables de entrada (características fisicoquímicas):**
1. Acidez fija  
2. Acidez volátil  
3. Ácido cítrico  
4. Azúcar residual  
5. Cloruros  
6. Dióxido de azufre libre  
7. Dióxido de azufre total  
8. Densidad  
9. pH  
10. Sulfatos  
11. Alcohol

**Variable de salida (objetivo):**
- Calidad (convertida en: `bajo`, `medio`, `alto`)

---

## ⚙️ Modelos Evaluados

Se compararon distintos modelos utilizando técnicas de clasificación supervisada:

- **KNN Classifier**
- **Logistic Regression**
- **Random Forest (opcional si fue usado)**

Para cada modelo se evaluó:

- **Accuracy**
- **Precision, Recall, F1-score**
- **Matriz de Confusión**
- **Curva ROC y AUC**

---

## 📊 Resultados Obtenidos

### ✅ Mejor Modelo: Logistic Regression
- **Accuracy:** `0.97`
- Excelente rendimiento prediciendo la clase `medio`, que representa la mayoría del dataset.
- Se confirmó su eficacia con la **curva ROC** y el **AUC**.

### ❌ Limitaciones:
- Ningún modelo logró predecir correctamente las clases `bajo` o `alto`.
- Esto se debe al **fuerte desbalance de clases**, lo que limita la capacidad de generalización para esas categorías.

---

## 📈 Visualizaciones Incluidas

- ✅ Matriz de Confusión para cada modelo
- ✅ Curva ROC por clase (`bajo`, `medio`, `alto`)
- ✅ Comparación de accuracy entre modelos


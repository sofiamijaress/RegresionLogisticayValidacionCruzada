# Regresi-nLog-sticayValidaci-nCruzada

Este repositorio contiene una práctica enfocada en la regresión logística aplicada a problemas de clasificación binaria Para lograrlo, se utilizó una base de datos con 200 observaciones publicada en [Kaggle](https://www.kaggle.com/datasets) y proporcionada por Wasiq Ali. La base original está en el siguiente [link](https://www.kaggle.com/datasets/wasiqaliyasir/diabates-dataset).  

El objetivo es evaluar la capacidad del modelo para predecir correctamente entre dos clases (0 o 1), utilizando diferentes métricas de desempeño como exactitud (accuracy), sensibilidad (recall), especificidad, precisión, F1-score, así como la curva ROC y el área bajo la curva (AUC).

La regresión logística es un modelo estadístico que, en lugar de predecir valores continuos, estima la probabilidad de pertenencia a una clase. A partir de esta probabilidad se define un umbral de clasificación: si la probabilidad es mayor o igual al umbral, se clasifica como 1; en caso contrario, como 0.
Para obtener un desempeño más robusto, se utiliza validación cruzada (Cross Validation). Esta técnica divide el conjunto de datos en varios subconjuntos (folds) y entrena el modelo múltiples veces, evaluándolo en diferentes particiones. De esta manera se reduce el riesgo de sobreajuste y se obtiene una medida más confiable de la capacidad del modelo.

Una de las herramientas principales de la práctica es la matriz de confusión, que permite comparar las predicciones con los valores reales. En ella se distinguen cuatro categorías: verdaderos positivos (TP), falsos positivos (FP), verdaderos negativos (TN) y falsos negativos (FN). A partir de esta tabla se calculan métricas clave:

* Accuracy (Exactitud): proporción de predicciones correctas respecto al total.

* Sensibilidad (Recall o TPR): mide la capacidad del modelo de identificar correctamente los casos positivos.

* Especificidad (TNR): mide la capacidad del modelo de identificar correctamente los casos negativos.

* Precisión (Precision): indica qué proporción de los casos predichos como positivos son realmente positivos.

* F1-Score: media armónica entre la precisión y la sensibilidad, útil cuando existe un desbalance de clases.

Además, se incluye la curva ROC (Receiver Operating Characteristic), que muestra la relación entre la sensibilidad (TPR) y el 1 - especificidad (FPR). Esta curva permite analizar cómo varía el desempeño del modelo al cambiar el umbral de clasificación.

En este proyecto trabajamos con el archivo “Diabetes.csv”; se le cambia el nombre para fines prácticos.

La base de datos contiene los siguientes elementos:

* PatientID: identificador único del registro (no aporta información clínica).

* Age: edad del paciente (años).

* Gender: género reportado (Male/Female).

* BMI: índice de masa corporal (kg/m²).

* BloodPressure: presión arterial (mmHg).

* Insulin: nivel de insulina (μU/mL).

* Glucose: concentración de glucosa en sangre (mg/dL).

* DiabetesPedigreeFunction: índice que resume la carga familiar/genética de diabetes.

* Outcome: variable objetivo (1 = tiene diabetes, 0 = no).

En este documento se incluyen los siguientes archivos: 
* [Reporte en formato .ipynb](A2.1_645700.ipynb)
* [Reporte en formato .html](A2.1_645700.html)
* [Base de datos](Diabetes.csv)

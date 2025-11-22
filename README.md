---

# **Proyecto Final — Predicción de Desembolsos en Cooperación Internacional**

Este proyecto aplica técnicas de ciencia de datos para analizar y predecir montos de **desembolsos de proyectos de cooperación internacional**, utilizando datos provenientes de IATI (International Aid Transparency Initiative).

El objetivo principal es desarrollar un modelo predictivo que permita identificar patrones y comprender qué variables influyen en el financiamiento otorgado a diferentes iniciativas de desarrollo.

---

##  **1\. Objetivo del Proyecto**

* Realizar limpieza, tratamiento y preparación de datos.

* Aplicar **feature selection** para reducir la dimensionalidad.

* Entrenar modelos de **regresión** (Regresión Lineal y Random Forest).

* Evaluar métricas de desempeño (MAE, RMSE, R2).

* Interpretar resultados y analizar las hipótesis planteadas.

---

##  **2\. Contenido del Repositorio**

`📦 proyecto-desembolsos/`  
`│`  
`├── Dataset_iati.xlsx                  → base de datos usada`  
`├── Proyecto_Final__Mercedes_Brito.ipynb  → notebook final del proyecto`  
`├── requirements.txt                   → librerías necesarias`  
`├── README.md                          → documentación del proyecto`

---

##  **3\. Tecnologías Utilizadas**

* Python

* Pandas

* Numpy

* Seaborn

* Matplotlib

* Scikit-learn

---

##  **4\. Modelos Entrenados**

### **🔹 Regresión Lineal**

* MAE: *214.51*

* RMSE: *524.86*

* R2: *0.2448*

### **🔹 Random Forest Regressor**

* MAE: *191.82*

* RMSE: *538.41*

* R2: *0.2053*

---

##  **5\. Conclusiones del Modelo**

La Regresión Lineal obtuvo un R² mayor que Random Forest en este caso, lo que sugiere que la linealidad del fenómeno es más clara que patrones no lineales complejos.  
 Las variables más influyentes fueron:

* **Categoría de sector**

* **Sector**

* **País o región receptores**

* **Año de inicio (Start Year)**

El modelo explica una parte limitada de la variabilidad, lo cual es comprensible dado que los montos dependen también de factores políticos, emergencias, prioridades estratégicas y acuerdos bilaterales no reflejados en la base de datos.

---

##  **6\. Hipótesis**

| Nº | Hipótesis | Resultado |
| ----- | ----- | ----- |
| H1 | El sector influye en el desembolso | ✔ Se verifica parcialmente |
| H2 | El país receptor influye | ✔ Se verifica parcialmente |
| H3 | El año de inicio es predictor relevante | ✔ Parcialmente |
| H4 | La combinación de país \+ sector \+ año mejora el modelo | ✔ Mejora, pero modestamente |

---


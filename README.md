![Banner del proyecto](assets/banner.jpeg)


# Detección de Fallas en Maquinaria Industrial con Machine Learning
Aprendizaje de Máquina — Universidad Industrial de Santander (UIS).
## Integrantes
- Lesly Gabriela Rodriguez 2251510
- Maria Jose Chavez Torres 2251727

## Objetivo
Analizar datos de sensores de maquinaria industrial para detectar fallas y predecir el torque de operación, mediante modelos de clasificación y de regresión.

## Descripción del proyecto
El proyecto parte de un conjunto de 10.000 registros de máquinas con y sin falla (3,39 % de fallas). Se hace un análisis exploratorio, se construyen modelos de clasificación para detectar si una máquina falla y de qué tipo, y modelos de regresión para predecir el torque a partir de las demás condiciones de operación.

## Dataset
Se utiliza el dataset [Machine Predictive Maintenance Classification](https://www.kaggle.com/datasets/shivamb/machine-predictive-maintenance-classification) de Kaggle, compuesto por 10 variables, incluyendo mediciones de temperatura del aire y del proceso, velocidad rotacional y desgaste de herramienta, junto con la variable objetivo de clasificacion que indica si hubo falla y de qué tipo y la variable objetivo de regresión el Torque.

| Variable | Descripción |
|---|---|
| `UDI` | Identificador de la fila |
| `Product ID` | Identificador del producto |
| `Type` | Calidad del producto: L (baja), M (media) o H (alta) |
| `Air temperature [K]` | Temperatura del aire |
| `Process temperature [K]` | Temperatura del proceso |
| `Rotational speed [rpm]` | Velocidad de rotación |
| `Torque [Nm]` | Torque |
| `Tool wear [min]` | Desgaste de la herramienta |
| `Target` | Falla: 0 = no falla, 1 = falla |
| `Failure Type` | Tipo de falla (o "No Failure") |
| `Temp_diff` | Variable creada: temperatura del proceso menos temperatura del aire |

- **Descarga:** [Machine Predictive Maintenance Classification](https://www.kaggle.com/datasets/shivamb/machine-predictive-maintenance-classification)
## Estructura del repositorio
```
├── data/           # Dataset original
├── notebooks/      # Notebooks de análisis y modelado
    ├── 01_eda.ipynb
│   ├── 02_clasificacion.ipynb
│   └── 03_regresion.ipynb
├── assets
├── README.md
```

## Metodología
1. **EDA:** análisis exploratorio de los datos.
2. **Modelos de clasificación:** detección de falla (binaria) y tipo de falla (multiclase).
3. **Modelos de regresión:** predicción del torque.

## Modelos y métodos
- **Clasificación:** Gaussian Naive Bayes, Decision Tree, Random Forest, SVM, SMOTE, F1.
- **Regresión:** Decision Tree, Random Forest, SVR, RMSE, MAE, R², validación cruzada (KFold).

## Herramientas
Python, pandas, NumPy, scikit-learn, matplotlib, seaborn, Google Colab, GitHub.

## Enlaces
- **Códigos:** [Notebooks](Notebooks/)
- **Video:** 
- **Repositorio:** https://github.com/gabbrod/Deteccion-de-Fallas-en-manteniminero-Predictivo

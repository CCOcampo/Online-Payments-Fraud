# Detección de Fraudes en Transacciones Financieras

Este proyecto tiene como objetivo el análisis y desarrollo de un modelo de machine learning para identificar transacciones fraudulentas en un conjunto de datos financieros.

---

## **Descripción del Proyecto**

La identificación temprana de fraudes financieros es crucial para garantizar la seguridad en las plataformas de transacciones. Este proyecto utiliza un conjunto de datos de transacciones para desarrollar un modelo que clasifique las transacciones como legítimas o fraudulentas.

El conjunto de datos contiene información detallada sobre cada transacción, como tipo, montos, y saldos antes y después de la transacción, así como si esta fue marcada como sospechosa. La variable objetivo es **`isFraud`**, que indica si una transacción es fraudulenta (`1`) o no (`0`).

---

## **Conjunto de Datos**

### **Fuente**

[Online Payments Fraud Detection Dataset](https://www.kaggle.com/datasets/rupakroy/online-payments-fraud-detection-dataset/data)

### **Características del Conjunto de Datos**

- **Número de filas:** 100,000
- **Número de columnas:** 11

| **No** | **Columna**        | **Descripción**                                              |
| ------ | ------------------ | ------------------------------------------------------------ |
| 1      | **step**           | Paso del proceso de transacción.                             |
| 2      | **type**           | Tipo de transacción (`PAYMENT`, `TRANSFER`, `CASH_OUT`).     |
| 3      | **amount**         | Monto de la transacción.                                     |
| 4      | **nameOrig**       | Identificador del origen de la transacción.                  |
| 5      | **oldbalanceOrg**  | Saldo anterior en la cuenta del origen.                      |
| 6      | **newbalanceOrig** | Nuevo saldo en la cuenta del origen tras la transacción.     |
| 7      | **nameDest**       | Identificador del destino de la transacción.                 |
| 8      | **oldbalanceDest** | Saldo anterior en la cuenta del destino.                     |
| 9      | **newbalanceDest** | Nuevo saldo en la cuenta del destino tras la transacción.    |
| 10     | **isFraud**        | Indicador de fraude (`1`: Fraudulenta, `0`: No fraudulenta). |
| 11     | **isFlaggedFraud** | Marcada como sospechosa (`1`: Sí, `0`: No).                  |

---

## **Metodología**

1. **Exploración de Datos:**

   - Análisis estadístico y visualización de las características principales.
   - Identificación y manejo de valores nulos o inconsistencias.

2. **Preprocesamiento:**

   - Transformación de variables numéricas.
   - Codificación de variables categóricas como `type`.
   - Eliminación de columnas redundantes o irrelevantes.

3. **Selección de Características:**

   - Evaluación de la importancia de cada característica.
   - División de los datos en conjuntos de entrenamiento y prueba.

4. **Modelado ML:**

   - Entrenamiento de modelos supervisados como Random Forest y Decision Tree Classifier.
   - Métricas como precisión, recall, F1-score, y área bajo la curva ROC para medir el rendimiento.

---

## **Resultados Esperados**

- Un modelo de clasificación capaz de detectar transacciones fraudulentas con alta precisión.
- Análisis de las características más relevantes para identificar actividades sospechosas.

---

## **Aplicaciones Industriales**

- **Bancos y Fintechs:**  
  Identificación temprana de fraudes para prevenir pérdidas económicas y proteger la confianza de los usuarios.
- **E-Commerce:**  
  Prevención de fraudes en plataformas de pagos digitales.
- **Aseguradoras:**  
  Análisis de patrones de fraude en reclamos y transacciones asociadas.

---

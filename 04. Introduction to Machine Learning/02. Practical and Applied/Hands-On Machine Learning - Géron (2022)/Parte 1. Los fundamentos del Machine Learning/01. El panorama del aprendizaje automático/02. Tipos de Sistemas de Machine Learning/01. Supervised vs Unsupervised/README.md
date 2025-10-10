# Supervised vs Unsupervised

## 🎓 Aprendizaje Supervisado

Los datos de entrenamiento incluyen la solución denominada **"label"**.

<div align="center">
  <img src="./assets/Aprendizaje_supervisado.png" alt="Aprendizaje Supervisado" width="600"/>
  <p><em>Un buen ejemplo de aprendizaje supervisado es la clasificación del spam en el correo electrónico. El aprendizaje supervisado se caracteriza porque todo el conjunto de datos que usas para entrenar un modelo está etiquetado, cada muestra contiene información sobre sí misma, para que el modelo pueda aprender.</em></p>
</div>

### Tareas Típicas

- **Clasificación** (como filtros de spam)
- **Regresión** (como predecir precios de coches)

> ⚠️ **Nota importante:** Algunos algoritmos de regresión pueden usarse para clasificación y viceversa.

### Algoritmos Más Importantes

- **k-nearest neighbors**
- **Linear regression**
- **Logistic regression**
- **Support Vector Machines (SVMs)**
- **Decision trees and random forests**
- **Neural networks** (aunque algunas arquitecturas pueden ser no supervisadas o semisupervisadas)

---

## 🔍 Aprendizaje No Supervisado (Unsupervised Learning)

En el aprendizaje no supervisado **no hay etiquetas**, los datos de entrenamiento no están etiquetados y el sistema intenta aprender **"sin un profesor"**.

### 📦 Clustering

- **K-means**
- **Hierarchical Cluster Analysis (HCA)**
- **Expectation Maximization**

### 📊 Visualización y Reducción de Dimensionalidad

- **Principal Component Analysis (PCA)**
- **Kernel PCA**
- **Locally-Linear Embedding (LLE)**
- **t-Distributed Stochastic Neighbor Embedding (t-SNE)**

### 🔗 Association Rule Learning

- **Apriori**
- **Eclat**

> 💡 **Buena práctica:** Siempre es recomendable aplicar reducción de dimensionalidad a los datos de entrenamiento sin perder demasiada información.

---

## 🎯 Aprendizaje Semisupervisado

Algunos algoritmos pueden trabajar con **datasets parcialmente etiquetados**, constituyendo el aprendizaje semisupervisado.

### Ejemplo Práctico

**Google Photos** agrupa fotos por personas que aparecen en ellas y solicita al usuario que las etiquete.

### Composición

La mayoría de algoritmos semisupervisados son **combinaciones de algoritmos no supervisados y supervisados**.

### Deep Belief Networks (DBNs)

Un caso específico son las **Deep Belief Networks (DBNs)**, que se basan en componentes no supervisados llamados **Restricted Boltzmann Machines (RBMs)** apilados.

**Proceso de entrenamiento:**
1. Los RBMs se entrenan secuencialmente de manera no supervisada
2. Todo el sistema se ajusta finamente (fine-tuned) utilizando técnicas de aprendizaje supervisado

---

## 🤖 Aprendizaje por Refuerzo (Reinforcement Learning)

En el aprendizaje por refuerzo, el sistema de aprendizaje se denomina **agente** y puede:

- 👁️ Observar el entorno
- ⚡ Seleccionar y ejecutar acciones
- 🎁 Obtener recompensas a cambio (o penalizaciones en forma de recompensas negativas)

### Policy

El agente debe aprender por sí mismo cuál es la mejor estrategia, llamada **policy**, para obtener la mayor recompensa a lo largo del tiempo.

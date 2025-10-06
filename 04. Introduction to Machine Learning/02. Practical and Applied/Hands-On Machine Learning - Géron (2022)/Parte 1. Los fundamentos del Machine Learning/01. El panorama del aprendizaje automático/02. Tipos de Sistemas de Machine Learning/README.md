# Tipos de Sistemas de Machine Learning

## 📊 Clasificación Principal

Los sistemas de ML se clasifican según **tres criterios principales**:

1. **Supervisión humana**: supervised, unsupervised, semisupervised, reinforcement learning
2. **Aprendizaje incremental**: online vs batch
3. **Estrategia de generalización**: instance-based vs model-based learning

---

## 🏷️ Supervised vs Unsupervised

### Aprendizaje Supervisado

Los datos de entrenamiento incluyen la solución denominada **"label"**.

**Tareas típicas:**
- **Clasificación** (como filtros de spam)
- **Regresión** (como predecir precios de coches)

> ⚠️ **Nota importante:** Algunos algoritmos de regresión pueden usarse para clasificación y viceversa.

### Aprendizaje No Supervisado (Unsupervised Learning)

En el aprendizaje no supervisado **no hay etiquetas**, los datos de entrenamiento no están etiquetados y el sistema intenta aprender **"sin un profesor"**.

---

## 🔄 Batch and Online Learning

Otro criterio para clasificar los sistemas de ML es si el sistema puede aprender incrementalmente desde el flujo (**stream**) de datos de entrada o no.

Esta distinción establece la diferencia entre:
- **Aprendizaje online**: El modelo puede actualizarse continuamente con nuevos datos
- **Aprendizaje batch**: Requiere entrenar desde cero con todo el conjunto de datos disponible

---

## 🎯 Instance-Based vs Model-Based Learning

Otra manera de categorizar sistemas de ML es según **cómo generalizan**, ya que el objetivo final es **predecir correctamente nuevas instancias**.

Existen **dos enfoques principales** de generalización:
- **Instance-based learning**
- **Model-based learning**

Cada uno con estrategias diferentes para hacer predicciones sobre datos no vistos previamente.

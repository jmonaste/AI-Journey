# Instance-Based vs Model-Based Learning

## 🎯 Objetivo de la Generalización

Otra manera de categorizar sistemas de ML es según **cómo generalizan**, ya que el objetivo final es **predecir correctamente nuevas instancias**.

Existen **dos enfoques principales** de generalización:
- **Instance-based learning**
- **Model-based learning**

Cada uno con estrategias diferentes para hacer predicciones sobre datos no vistos previamente.

---

## 💾 Instance-Based Learning

Posiblemente la forma más trivial de aprendizaje es **aprender de memoria**.

### Ejemplo: Clasificación de Spam

Por ejemplo, clasificar emails como spam cuando son idénticos a correos ya etiquetados como spam. No es la peor solución, pero ciertamente no es la mejor.

### Medida de Similitud

Se puede usar una **medida de similitud** para etiquetar correos parecidos al spam.

Una forma básica de similitud en el caso del spam es **contar el número de palabras que tienen en común**.

### Definición

> 📌 **Instance-based learning:** El sistema aprende los ejemplos de memoria y luego generaliza a nuevos casos usando medidas de similitud.

---

## 🔬 Model-Based Learning

Otra forma de generalizar a partir de un conjunto de ejemplos es **construir un modelo** de esos ejemplos y luego usar dicho modelo para hacer predicciones.

### Ejemplo: Satisfacción de Vida vs GDP

Si descargamos datos de GDP per cápita de países y el índice de satisfacción de vida:

1. Hacemos un gráfico
2. Observamos una especie de relación lineal
3. Decidimos modelar la satisfacción de vida como una función lineal del GDP per cápita

### Model Selection

> 📊 **Model Selection:** Hemos seleccionado un modelo lineal de la satisfacción de vida con un solo atributo, el GDP per cápita.

### Selección de Parámetros

Antes de usar el modelo, debemos seleccionar algunos **parámetros** para la función lineal.

Para elegir estos parámetros, debemos definir una **medida de rendimiento**.

### Funciones de Evaluación

Podemos definir:

- **Utility function** (o fitness function): mide qué tan **bueno** es el modelo
- **Función de costo**: mide cuán **malo** es

### Regresión Lineal

Para problemas de **regresión lineal**, se usa típicamente una función de costo que mide la distancia entre:
- La predicción del modelo lineal
- Las muestras de ejemplo

> 🎯 **Objetivo:** Minimizar esta distancia, y aquí es donde el **algoritmo de regresión lineal** entra en escena.

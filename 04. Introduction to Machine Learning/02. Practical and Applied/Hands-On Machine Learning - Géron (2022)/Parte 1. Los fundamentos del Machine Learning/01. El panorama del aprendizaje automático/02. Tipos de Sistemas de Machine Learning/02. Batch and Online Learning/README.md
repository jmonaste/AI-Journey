# Batch and Online Learning

## 📋 Criterio de Clasificación

Otro criterio para clasificar los sistemas de ML es si el sistema puede aprender incrementalmente desde el flujo (**stream**) de datos de entrada o no.

Esta distinción establece la diferencia entre:
- **Aprendizaje online**: El modelo puede actualizarse continuamente con nuevos datos
- **Aprendizaje batch**: Requiere entrenar desde cero con todo el conjunto de datos disponible

---

## 📦 Batch Learning (Aprendizaje por Lotes)

En el batch learning, el sistema **no puede aprender incrementalmente** y debe ser reentrenado utilizando todos los datos disponibles.

### Características

- Se realiza **offline** porque requiere mucho tiempo y recursos computacionales
- Por esta razón se denomina **offline training**
- El proceso puede automatizarse (entrenar, evaluar, lanzar)

### Limitaciones

> ⚠️ **Problema principal:** El entrenamiento sobre nuevos datos junto con los antiguos puede durar horas, lo que representa una limitación significativa cuando se necesita actualizar el modelo con frecuencia.

---

## 🔄 Online Learning

En el online learning, el modelo se entrena de manera **incremental** alimentándolo con instancias de datos secuenciales individualmente o en pequeños grupos llamados **mini-batches**.

### Ventajas

- ⚡ Cada paso de aprendizaje es **rápido y económico**
- 🔁 El sistema aprende sobre la marcha con nuevos datos según van llegando
- 💻 Es una buena opción cuando se tienen **recursos limitados**

### Out-of-Core Learning

Los algoritmos de aprendizaje online también pueden usarse para entrenar sistemas sobre **grandes datasets que no caben en la memoria** de una máquina, proceso conocido como **out-of-core learning**.

### Learning Rate

Un parámetro importante es el **learning rate**, que determina qué tan rápido se adapta el sistema a los cambios.

### ⚠️ Desafíos

Uno de los principales retos es evitar que el rendimiento decaiga cuando entran **datos de mala calidad** al sistema.

> 💡 **Solución:** Para minimizar este riesgo, es necesario monitorizar tanto el sistema como su entrada de datos.

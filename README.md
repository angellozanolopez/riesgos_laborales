# ⚠️ Análisis Estadístico de Riesgos Laborales  
📊 **Formación en Modelos de Clasificación y Comparativas Estadísticas**  

---

## **📝 Introducción**  
En este proyecto desarrollaremos un **sistema de clasificación** para detectar **incongruencias** en los resultados de análisis de prevención de **riesgos laborales** en distintas empresas.  

🔍 **Problema actual:**  
1. Un técnico evalúa los riesgos de una empresa y redacta un informe.  
2. Teóricamente, las evaluaciones entre empresas del mismo sector deberían ser similares.  
3. En la práctica, hay grandes diferencias debido a errores humanos (evaluaciones "de memoria").  
4. Esto puede ser **peligroso**, ya que se omiten riesgos importantes.  

🎯 **Objetivo del proyecto:**  
✔️ Crear un modelo en **Sklearn** que, en base al **sector de cada empresa** (`nSectorEmp`), detecte **si una evaluación de riesgos es correcta o no**, basándose en un histórico de evaluaciones.  

Adicionalmente, identificaremos:  
✅ **% de similitud** entre evaluaciones del mismo sector.  
✅ **Riesgos comunes** por sector (`nSectorEmp`).  
✅ **Riesgos atípicos** que aparecen en una empresa pero no son habituales.  

---

## **📂 Datos y Dataset**  
📂 **Acceso al dataset:**  
🔗 [riesgos_ejercicio.zip](https://apioverstand.es/training/riesgos_ejercicio.zip)  

📊 **Campos relevantes del dataset:**  
| Campo         | Descripción |
|--------------|------------|
| `sCodCliente` | Código de la empresa (ignorar `idEmpresa`). |
| `nSectorEmp` | Código del sector de la empresa. |
| `idEvaluacion` | Código de la evaluación de riesgos (cada empresa tiene varias). |
| `ixRiesgo` | Riesgo identificado en la evaluación. |
| `ixPuesto` | Puesto donde se detectó el riesgo (ej. Administración, Logística, etc.). |
| `ixFuenteRL` | Particularidad asociada al riesgo. |

⚠️ **Importante:**  
Un riesgo **siempre** estará vinculado a **un puesto (`ixPuesto`) o a una fuente (`ixFuenteRL`), pero nunca a ambos simultáneamente**.  

📌 **Material adicional:**  
También se proporciona un **diagrama UML** de la base de datos para facilitar la comprensión del dataset.  

---

## **📌 Entregables**  

### **✅ Entregable 1: Análisis de Tecnologías**  
🔍 Evaluación de herramientas disponibles, priorizando **tecnologías open source** sin costes.  
📸 Si alguna opción tiene coste, se debe incluir un **pantallazo del precio**.  

### **✅ Entregable 2: Desarrollo de la solución**  
📦 Todos los archivos deben enviarse en un único **WeTransfer** e incluir:  

1️⃣ **Código fuente de la solución.**  
2️⃣ **Video explicativo del código fuente** (máximo **3 minutos**).  
3️⃣ **Video mostrando e interpretando los resultados** (máximo **2 minutos**).  

---

## **🎥 SOLUCIÓN**  
**📌 ENTREGABLE 1: ANÁLISIS DE TECNOLOGÍAS Y ELECCIÓN DE LA TECNOLOGÍA**  

El desarrollo de un sistema de clasificación para detectar incongruencias en los resultados de análisis de prevención de riesgos laborales de empresas implica varios pasos que podemos ver a continuación:

### 1. Análisis de Tecnologías:
• **Lenguaje de Programación:** Python es una elección sólida debido a su amplia comunidad, bibliotecas de aprendizaje automático y herramientas de análisis de datos.  
• **Librerías de Machine Learning:** Para la clasificación, podemos utilizar **Scikit-Learn**, una biblioteca de aprendizaje automático en Python. Es open source y ampliamente utilizada.  
• **Procesamiento y visualización de Datos:** **Pandas** y **NumPy** para la manipulación y procesamiento de datos, y **Matplotlib** para visualizar datos.  
• **Entorno de Desarrollo:** **Jupyter Notebooks** o IDEs como **VSCode**.  
• **Herramientas para Modelado:** **Scikit-Learn** dispone, entre otros, del algoritmo **cosine_similarity()**, ideal para nuestro proyecto.

### 2. Costes Asociados:
La mayoría de las tecnologías mencionadas son **open source** y no tienen costos asociados, excepto que decidamos utilizar servicios en la nube para el almacenamiento de datos o entrenamiento de modelos. En ese caso, no lo hemos necesitado, aunque dependiendo del proyecto, quizás sea necesario utilizar plataformas como **AWS**, que dispone tanto de un nivel gratuito con algunos límites, como niveles no gratuitos.

### 3. Elección de la Tecnología:
Dado que se prefiere el uso de tecnologías **open source** sin costos asociados, **Python** con **Scikit-Learn** y las bibliotecas mencionadas es una elección adecuada para este proyecto.

---

**📌 ENTREGABLE 2: DESARROLLO Y ENTREGA**

Esta segunda parte, se ha realizado en **notebook** dividido en 3 partes:

1. **Preparación de datos:** eliminación de columnas, duplicados, etc.
2. **Análisis de datos y extracción de estadísticas:** riesgos más frecuentes, menos frecuentes, riesgos por sector, por cliente, etc.
3. **Obtención de la similitud** entre una evaluación determinada con todas las demás del mismo sector, usando el algoritmo **cosine_similarity()**.

📌 **Código fuente:** [![Ver en YouTube](https://img.shields.io/badge/🎥%20Ver%20Video-red?logo=youtube&logoColor=white)](https://youtu.be/S1xIJju6wTY?si=xA9MO0RhUO_gbYKZ)<br>📌 **Demostración:**  [![Ver en YouTube](https://img.shields.io/badge/🎥%20Ver%20Video-red?logo=youtube&logoColor=white)](https://youtu.be/7_tDV2Zjfg0?si=WNhU-LVcD-JWGK6h)  


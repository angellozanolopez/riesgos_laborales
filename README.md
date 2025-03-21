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

📌 **Código fuente:** [![Ver en YouTube](https://img.shields.io/badge/🎥%20Ver%20Video-red?logo=youtube&logoColor=white)](https://youtu.be/S1xIJju6wTY?si=xA9MO0RhUO_gbYKZ)  
📌 **Demostración:**  [![Ver en YouTube](https://img.shields.io/badge/🎥%20Ver%20Video-red?logo=youtube&logoColor=white)](https://youtu.be/7_tDV2Zjfg0?si=WNhU-LVcD-JWGK6h)  


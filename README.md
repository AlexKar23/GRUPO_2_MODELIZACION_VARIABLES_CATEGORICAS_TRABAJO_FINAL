# Calculadora de ROI para Admisiones de Máster Premium 🎓📊

**Trabajo Final - Modelización de Variables Categóricas (MVC)**
*Título Superior de Data Science (TSDS) - ESIC University*

## 👥 Integrantes del Equipo
* Ignacio García
* Alejandro Karambasis
* Patricia García
* Ignacio Iturralde

## 🎯 Descripción y Pregunta de Investigación
Hemos seleccionado la **Pregunta E** propuesta en la guía del proyecto. Nuestro objetivo es desarrollar una herramienta predictiva (Calculadora de ROI) para el equipo de admisiones de una escuela de negocios. 

El modelo predecirá el **tramo salarial esperado (`TR_SUELDO`)** de un candidato tras finalizar su máster en función de su perfil de entrada. Esta variable objetivo es de tipo **ordinal** (7 tramos desde <700€ hasta ≥3.000€). Al predecir el salto salarial, la herramienta busca justificar la inversión económica que supone la matrícula del máster en ventas B2C.

## 🗂️ Datos y Metodología
* **Dataset:** Encuesta de Inserción Laboral de Universitarios (EILU 2019) - **Egresados de Máster**.
* **Target:** `TR_SUELDO` (Ordinal). Se ha tratado de forma especial el ~12% de registros sin empleo y el ~3% de NS/NC.
* **Variables predictoras clave:** `RAMA`, `T_UNIV`, `ESTUDIOS_PADRE`, `ESTUDIOS_MADRE`, `SEXO`, `MOV_IN`, `TIC`, `JORNADA`.
* **Modelos a evaluar:** Regresión Logística Ordinal (basado en *proportional odds*) vs. Modelos basados en árboles de decisión (Random Forest, XGBoost/LightGBM).

## 💡 Principales Hallazgos
*(🚨 Nota para el equipo: Según las reglas del repositorio, debéis rellenar este apartado al finalizar el proyecto para que sea legible sin abrir los notebooks. Aquí tenéis una estructura de ejemplo para cuando terminéis).*

1. **Hallazgos del EDA:** [Ej: La moda salarial se sitúa en el tramo 4 (1.500-1.999€, ~33% de los empleados), pero varía fuertemente según la rama de conocimiento].
2. **Rendimiento de los Modelos:** [Ej: El modelo de Regresión Logística Ordinal logró un accuracy de X%, pero el XGBoost redujo los errores de salto entre tramos extremos].
3. **Variables más determinantes (SHAP):** [Ej: La movilidad interprovincial (MOV_IN) y la rama (RAMA) son los factores que más influyen en alcanzar los tramos 6 y 7 (≥2.500€)].


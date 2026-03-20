# Proyecto Final - Data Xperience
## Análisis de la Infraestructura de Internet Fijo en Colombia (2023)
### Evaluación Estadística y Modelado Predictivo de la Conectividad a Nivel Municipal

---

## 📝 Descripción del Proyecto
Este proyecto realiza un análisis integral del estado de la conectividad de internet fijo en Colombia durante el año 2023, con el objetivo de transformar datos crudos en información estratégica mediante técnicas de **Data Wrangling**, **Estadística Descriptiva** y modelos de **Machine Learning**.

Este análisis permite identificar brechas regionales, dominios tecnológicos y la relación entre la velocidad de oferta y la adopción del servicio en diferentes áreas de Colombia.

---

## 🚀 Estructura del Código

El desarrollo está organizado en tres módulos lógicos fundamentales:

### 1. Preparación y Limpieza de Datos (ETL)
*   **Carga:** Conexión con Google Drive y lectura de archivos CSV con codificación `latin-1`.
*   **Limpieza:** Eliminación de comillas innecesarias, espacios en blanco y caracteres especiales.
*   **Normalización:** Conversión de formatos decimales (comas a puntos) y transformación de tipos de datos de *String* a *Numeric* (Float/Int).
*   **Tratamiento de Nulos:** Identificación y llenado de valores faltantes para asegurar la integridad de los modelos.

### 2. Análisis Estadístico y Visualización
*   **Métricas de Tendencia Central:** Cálculo de Media, Mediana y Moda para velocidades y tecnologías.
*   **Análisis de Dispersión:** Evaluación de la Desviación Estándar y Rangos de velocidad para entender la desigualdad del servicio.
*   **Visualizaciones:** 
    *   *Gráfico de Barras:* Top 10 departamentos con mayor volumen de accesos.
    *   *Gráfico de Torta:* Distribución del mercado entre Segmento Hogares y Empresas.

### 3. Modelado Predictivo (Machine Learning)
*   **Regresión Lineal:** Modelo para predecir la cantidad de accesos en función de la velocidad de bajada (Mbps).
*   **Clasificación (Random Forest):** Clasificador entrenado para distinguir automáticamente entre infraestructura de "Alta Tecnología" (Fibra/HFC) y tecnologías legadas.
*   **Validación:** Generación de Matrices de Confusión para medir la precisión del algoritmo.

---

## 🛠️ Tecnologías Utilizadas
*   **Lenguaje:** Python 3.x
*   **Librerías:** 
    *   `Pandas`: Manipulación de DataFrames.
    *   `Matplotlib` & `Seaborn`: Visualización de datos.
    *   `Scikit-Learn`: Modelos de aprendizaje automático.
    *   `Numpy`: Operaciones vectorizadas.

---

## 📊 Variables Principales del Dataset

| Variable | Descripción |
| :--- | :--- |
| `DEPARTAMENTO` | Ubicación geográfica del acceso. |
| `TECNOLOGIA` | Medio de transmisión (Fibra Óptica, Cobre, Cable, etc.). |
| `VELOCIDAD_BAJADA` | Velocidad nominal de descarga en Mbps. |
| `ACCESOS` | Número de suscripciones registradas. |
| `SEGMENTO` | Tipo de usuario (Hogar o Empresas). |

---

## 📈 Conclusiones Destacadas
*   **Concentración Urbana:** Los 10 departamentos principales que concentran la gran mayoría de la conectividad nacional.
*   **Predominio de Hogares:** El segmento residencial (Hogares) representa el motor principal del crecimiento en accesos.
*   **Eficacia del Modelo:** El modelo de clasificación permite segmentar con éxito el tipo de infraestructura basándose únicamente en métricas de rendimiento (velocidad).

---
**Desarrollado como parte del programa Data Xperience - EAN 2026.**

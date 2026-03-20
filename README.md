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
*   **Lenguaje:** Python 3.12.13
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
*   **Concentración Urbana:** Los 10 departamentos principales que concentran la gran mayoría de la conectividad nacional. (Bogotá, Antioquia, Valle del Cauca, Cundinamarca, Atlántico, Santander, Bolívar, Tolima, Risaralda, Norte de Santander).
*   **Predominio de Hogares:** El segmento residencial (Hogares) representa el motor principal del crecimiento en accesos. (Estratos 1, 2 y 3)
*   **Eficacia del Modelo:** El modelo de clasificación permite segmentar con éxito el tipo de infraestructura basándose únicamente en métricas de rendimiento (velocidad).

---

*   **Link Video:** https://www.canva.com/design/DAHEWV1KDww/BLf_Ti821x_8sjDat8cf2Q/edit?utm_content=DAHEWV1KDww&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton
*   **Link Google Colab:** https://colab.research.google.com/drive/1LChEe5V3rVjmoaVCUMeGNeT5Qm2U_ZNx?usp=sharing
*   **Link Dataset usando en el proyecto:** https://drive.google.com/file/d/1oeRT7I3H27LmDPMtlpluM5FeChi3RkFX/view?usp=sharing
  
---

**Desarrollado como parte del programa Data Xperience - EAN 2026.**

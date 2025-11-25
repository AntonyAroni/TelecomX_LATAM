# 📊 TelecomX LATAM – Análisis Integral, Limpieza y Evaluación de Datos para Detección de Evasión (Churn)

Este documento describe de manera completa y detallada el análisis del dataset **TelecomX LATAM**, cuyo objetivo principal es identificar los factores que influyen en la *evasión de clientes* (Churn). El estudio se desarrolla dentro de un entorno de **Google Colab**, el cual permite ejecutar el análisis sin necesidad de instalaciones adicionales.

---

# 📘 1. Introducción

El comportamiento de abandono de clientes es uno de los principales retos en la industria de telecomunicaciones. Comprender por qué un cliente decide cambiar de proveedor permite a las empresas diseñar estrategias más efectivas, optimizar campañas de retención y mejorar la calidad del servicio.  
Este proyecto desarrolla un análisis profundo del dataset **TelecomX LATAM**, comenzando desde la exploración inicial de sus variables hasta la identificación de patrones relevantes asociados al churn.

---

# 📂 2. Contenido del Proyecto

Este repositorio incluye el notebook:

- **TelecomX_LATAM.ipynb**: documento principal con la ejecución paso a paso del análisis.  
No requiere archivo de dependencias ya que el notebook está diseñado para Google Colab.

---

# 🔍 3. Objetivos del Proyecto

## 🎯 Objetivo General
Realizar un análisis exploratorio, descriptivo y de limpieza del dataset TelecomX LATAM para preparar los datos con miras a etapas avanzadas de modelado predictivo.

## 🎯 Objetivos Específicos
- Identificar y comprender la estructura completa del dataset.  
- Analizar el significado de cada variable mediante su diccionario oficial.  
- Detectar problemas en los datos que afecten un análisis confiable.  
- Transformar y estandarizar valores para garantizar consistencia.  
- Determinar cuáles variables influyen de manera más significativa en el churn.  
- Producir visualizaciones claras que resuman el comportamiento del dataset.

---

# 🧪 4. Metodología del Análisis

El estudio se divide en etapas secuenciales:

## 4.1 Exploración Preliminar
Incluye:
- Revisión de columnas.
- Inspección de tipos de datos.
- Identificación de estructuras anidadas (JSON dentro del dataset).
- Insight general sobre el volumen y contenido de la data.

## 4.2 Verificación con Diccionario de Datos
Cada columna es contrastada con su significado real.  
Esto permite:
- Detectar incoherencias entre nombres y descripciones.
- Inferir relaciones entre segmentos de información (cliente, internet, pagos, etc.).

## 4.3 Limpieza de Datos
En esta fase se revisan minuciosamente:
- **Valores nulos o faltantes**: Se identifican y analizan según su impacto.
- **Duplicados**: Detección de registros repetidos y evaluación de su eliminación.
- **Errores de formato**: Fechas corruptas, números en formato texto, strings inconsistentes.
- **Categorías incorrectas**: Combinaciones irregulares como “Yes”, “yes”, “Y”, “1”.

## 4.4 Transformación y Homogeneización
Incluye acciones como:
- Conversión uniforme de valores categóricos.
- Normalización de variables numéricas si es necesario.
- Reestructuración de datos provenientes de formatos API/JSON.
- Renombrado consistente de columnas (siguiendo el diccionario oficial).
- Selección preliminar de variables relevantes para churn.

## 4.5 Análisis Exploratorio Profundo (EDA)
Se estudia el comportamiento de churn en relación con:
- Servicios contratados.
- Duración del cliente (tenure).
- Tipo de contrato.
- Uso de internet y servicios adicionales.
- Métodos de pago.
- Costos mensuales y totales.

También incluye análisis multivariado mediante correlaciones y visualizaciones.

---

# 📊 5. Visualizaciones y Resultados

El notebook genera gráficos útiles para interpretar patrones relevantes. Entre ellos:

### 🔹 Distribuciones individuales
- Histogramas para variables numéricas.
- Boxplots para detectar outliers.

### 🔹 Comparaciones entre clientes churn y no churn
- Gráficos de barras categoricos.
- Comparación de medias y medianas de pagos.

### 🔹 Mapa de calor (Heatmap)
- Correlación entre variables numéricas.
- Identificación de relaciones que influyen directamente en la decisión de abandono.

### 🔹 Análisis segmentado
- Clientes con contrato mensual vs anual.
- Clientes con servicios múltiples vs servicios básicos.
- Impacto de métodos de pago automáticos y tarjetas.

Cada visualización se acompaña de interpretación contextual dentro del notebook.

---

# 🧼 6. Conclusiones del Análisis Preliminar

Tras la limpieza y exploración detallada del dataset, se concluye lo siguiente:

- Existen variables altamente correlacionadas con el churn, especialmente:
  - Método de pago.  
  - Tenure (tiempo con la compañía).  
  - Tipo de servicio de internet.  
  - Cargos mensuales elevados.
- El dataset presenta inconsistencias propias de fuentes reales, pero fueron corregidas.
- La segmentación entre churners y no churners muestra diferencias claras en:
  - Nivel de servicios contratados.
  - Comportamiento de pago.
  - Permanencia histórica del cliente.
- Se encuentran patrones repetitivos que justifican el uso posterior de modelos predictivos.
- El proceso de limpieza y estandarización deja los datos listos para análisis más avanzados, incluyendo machine learning.

---

# 👨‍💻 7. Tecnologías Utilizadas
- Python 3.x  
- Pandas  
- NumPy  
- Matplotlib  
- Seaborn  
- Google Colab

---

# ▶️ 8. Ejecución del Notebook
No requiere instalación manual de dependencias.  
Solo debes:

1. Abrir Google Colab.  
2. Cargar el archivo **TelecomX_LATAM.ipynb**.  
3. Ejecutar cada celda en orden.

---

# ✨ 9. Autor
**Antony Aroni**  
Proyecto académico y analítico orientado a la exploración y limpieza de datos reales.

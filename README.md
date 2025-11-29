# Luzu TV — Performance Analysis

## Descripción
Este proyecto analiza la performance de los contenidos de **Luzu TV** utilizando datos obtenidos mediante la **YouTube Data API**.  
El objetivo es identificar patrones de audiencia, nivel de engagement, diferencias entre programas y tendencias de crecimiento a lo largo del tiempo.

---

## Fuente de Datos
Los datos se obtienen directamente desde la **YouTube Data API**, consultada desde Python mediante:

- `google-api-python-client`  
- `requests`

> *El repositorio no contiene un archivo de datos porque los datos se descargan dinámicamente desde la API en el notebook.*

---

## Objetivos del análisis
- Evaluar el rendimiento de los distintos programas del canal.  
- Analizar visualizaciones, likes, engagement y crecimiento. 
- Identificar patrones semanales, horarios y estacionales.  
- Detectar picos de audiencia y sus posibles causas.  
- Construir y evaluar un modelo predictivo que estime la probabilidad de que un video supere ciertos umbrales de views.

---

## Tecnologías utilizadas
- Python  
- Pandas  
- NumPy  
- Matplotlib  
- Seaborn  
- Requests  
- google-api-python-client 
- Google Colab

---

## Contenido del repositorio
- /notebooks → Notebook completo del análisis (.ipynb)
- /presentation → Presentación del informe (PDF)
- /images → Gráficos exportados (opcional)
- /requirements.txt → Librerías necesarias para reproducir el proyecto

---

## Principales hallazgos

### Conclusiones generales sobre el contenido
- **Tópicos y tono:** Los temas cercanos, humorísticos o polémicos generan mayor interacción.  
  ➤ *Recomendación:* mantener títulos naturales y formatos conversacionales.

- **Duración óptima:** Los videos con mejor desempeño suelen durar entre **60 y 150 minutos**.  
  ➤ *Recomendación:* sostener este rango salvo en eventos especiales.

- **Timing de publicación:** **Jueves y viernes** muestran mejor rendimiento.  
  ➤ *Recomendación:* priorizar estrenos y contenidos clave en esos días.

- **Driver principal del engagement:** Interés temático y conexión emocional con la audiencia.  
  ➤ *Recomendación:* reforzar la identidad del canal y su estilo narrativo.

- **Patrones horarios:** Los picos de visualizaciones suelen concentrarse entre la mañana y el mediodía, con descenso hacia la noche.

- **Picos por evento:** Se observaron picos importantes que coinciden con programas especiales o clips virales.

### Conclusiones del modelo predictivo
- La performance final depende fuertemente de la **reacción temprana** del público (likes y comentarios iniciales).  
- Los videos con **alto engagement inicial** tienen mayor probabilidad de superar las **100k views**.  
- La **duración del video** impacta de forma moderada pero consistente.  
- Los **factores de programación** (día y hora) influyen, pero menos que las señales tempranas del público.

---

### Cómo reproducir el análisis
1. Clonar o descargar este repositorio.
2. Instalar dependencias:
   
pip install -r requirements.txt

3. Ejecutar el notebook:
   
/notebooks/luzu_performance_analysis.ipynb

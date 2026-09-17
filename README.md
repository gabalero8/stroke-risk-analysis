# Análisis de factores asociados al riesgo de accidente cerebrovascular

Proyecto de análisis estadístico con Python que explora la relación entre variables demográficas y clínicas y la presencia de accidentes cerebrovasculares (ACV).

Combina análisis exploratorio, ajuste de distribuciones, estimación, pruebas de hipótesis y un modelo experimental de regresión logística.

## Objetivos

- Explorar las características del conjunto de datos.
- Estudiar la relación entre la presencia de ACV y variables como la edad, el nivel promedio de glucosa, la hipertensión y las enfermedades cardíacas.
- Estimar parámetros y construir intervalos de confianza.
- Evaluar el ajuste de distribuciones mediante pruebas estadísticas.
- Explorar un modelo de clasificación e interpretar sus limitaciones.

## Datos

El archivo `stroke-dataset.csv` contiene las variables utilizadas en el análisis, entre ellas:

- Edad y género.
- Hipertensión y enfermedades cardíacas.
- Nivel promedio de glucosa.
- Índice de masa corporal (IMC).
- Historial de tabaquismo.
- Tipo de trabajo y residencia.
- Presencia de accidente cerebrovascular.

## Contenido del análisis

### Análisis exploratorio

Inspección de los datos, estadísticas descriptivas y visualizaciones para estudiar la distribución de las variables y sus relaciones.

### Estimación y ajuste de distribuciones

- Estimación mediante el método de los momentos y máxima verosimilitud.
- Construcción de intervalos de confianza.
- Ajuste de distribuciones para variables como la edad y la glucosa.
- Simulación mediante el método de la transformada inversa.

### Pruebas de bondad de ajuste

- Prueba de Shapiro-Wilk para evaluar la normalidad de la edad.
- Prueba de Anderson-Darling para evaluar el ajuste de la glucosa a una distribución Gamma.
- Estimación del valor p mediante bootstrap.
- Exploración de la estimación de densidad por kernels (KDE) como alternativa no paramétrica.

### Pruebas de hipótesis

Comparación de variables clínicas entre personas con y sin ACV para estudiar diferencias estadísticas entre ambos grupos.

### Regresión logística

Exploración de un modelo que utiliza la glucosa promedio y la presencia de enfermedades cardíacas como predictores.

Esta sección aborda una limitación importante de la clasificación con clases desbalanceadas: una exactitud global elevada puede coexistir con una baja sensibilidad para detectar la clase minoritaria.

## Tecnologías

- Python
- pandas y NumPy
- SciPy
- Matplotlib y Seaborn
- scikit-learn
- Jupyter Notebook

## Cómo ejecutar el proyecto

Se requiere Python y `pip`.

1. Clonar el repositorio:

   ```bash
   git clone https://github.com/gabalero8/stroke-risk-analysis.git
   cd stroke-risk-analysis
   ```

2. Instalar las bibliotecas utilizadas:

   ```bash
   pip install pandas numpy scipy matplotlib seaborn scikit-learn notebook
   ```

3. Iniciar Jupyter Notebook:

   ```bash
   jupyter notebook
   ```

4. Abrir `stroke_analysis.ipynb` y ejecutar las celdas en orden.

El archivo `stroke-dataset.csv` debe permanecer disponible en la carpeta del proyecto.

## Estructura del repositorio

```text
.
├── README.md
├── stroke_analysis.ipynb   # Notebook principal del análisis
├── stroke-dataset.csv     # Datos utilizados
└── stroke.jpg             # Imagen del proyecto
```

## Contexto académico y autores

Proyecto desarrollado originalmente para la asignatura INF280.

Integrantes:

- Cristobal Martinez
- Gabriel Lira
- Francisco Pino
- Catalina Zenteno

## Alcance y limitaciones

Este proyecto tiene fines académicos y de aprendizaje. Las asociaciones estudiadas no permiten establecer causalidad y el modelo experimental no constituye una herramienta de diagnóstico médico.

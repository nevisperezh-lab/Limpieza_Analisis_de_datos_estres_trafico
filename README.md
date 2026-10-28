# Análisis del Índice de Estrés del Tráfico en Ciudades Inteligentes

Este proyecto realiza un análisis exploratorio y proceso de limpieza de datos sobre el comportamiento del tráfico urbano, condiciones meteorológicas y 
el nivel de estrés de los conductores, utilizando el conjunto de datos *Traffic Stress Index Dataset for Smart Cities* de Kaggle.

##Descripción del Proyecto

El objetivo principal es preparar y explorar los datos para comprender las variables que impactan el índice de estrés vial (`stress_index`). 

El flujo de trabajo implementado incluye:
* **Inspección de datos:** Verificación de tipos de variables, dimensiones y presencia de valores nulos o registros duplicados.
* **Limpieza de datos:** Identificación y eliminación de columnas redundantes (`weather_condition.1`).
* **Análisis Exploratorio (EDA):** Inspección visual de la distribución de las variables numéricas y categóricas mediante histogramas y conteos de frecuencia.

## Estructura de los Datos

El conjunto de datos contiene 50,000 registros y 8 variables tras la limpieza:
* `traffic_density`: Densidad del tráfico.
* `horn_events_per_min`: Frecuencia de uso del claxon por minuto.
* `avg_speed`: Velocidad promedio del vehículo.
* `signal_wait_time`: Tiempo de espera en semáforos.
* `weather_condition`: Estado del clima (`Clear`, `Rainy`, `Foggy`, `Hot`).
* `road_quality_score`: Evaluación de la calidad de la vía (escala 1 a 10).
* `driver_experience_level`: Nivel de experiencia del conductor (`Beginner`, `Intermediate`, `Expert`).
* `stress_index`: Índice de estrés del conductor (variable objetivo de 0 a 100).

##Requisitos e Instalación

Para ejecutar este proyecto de forma local, clona este repositorio e instala las dependencias necesarias:

```bash
git clone [https://github.com/TU-USUARIO/analisis-estres-trafico.git](https://github.com/TU-USUARIO/analisis-estres-trafico.git)
cd analisis-estres-trafico
pip install -r requirements.txt

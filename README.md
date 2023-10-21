# Revolución en Seguridad Vial

## Finalidad del Proyecto
El proyecto se enfoca en el [análisis y la predicción del riesgo de accidentes de tráfico en los Estados Unidos](https://www.kaggle.com/datasets/sobhanmoosavi/us-accidents) utilizando un extenso conjunto de datos que abarca desde febrero de 2016 hasta marzo de 2023. Este conjunto de datos, con aproximadamente 7.7 millones de registros de accidentes, fue recopilado en tiempo real utilizando diversas [APIs de tráfico](https://api.data.gov/signup/). Las fuentes de información son variadas, incluyendo departamentos de transporte, agencias policiales, cámaras de tráfico y sensores de carreteras.

## Objetivos Específicos
- **Predicción de la Severidad de los Accidentes**: Utilizar variables como la hora del día, condiciones climáticas y ubicación para modelar y predecir la severidad de los accidentes.
- **Análisis de Hotspots de Accidentes**: Identificar áreas geográficas con altas tasas de accidentes.
- **Impacto de las Condiciones Climáticas y Ambientales**: Examinar cómo factores como la lluvia, la presión atmosférica y la visibilidad afectan la probabilidad de accidentes.
- **Evaluación de Infraestructuras Viales**: Analizar el impacto de las señales de tráfico, rotondas y otros elementos de infraestructura.
- **Comportamiento de Conducción durante la Pandemia de COVID-19**: Utilizar datos más recientes para analizar cambios en el comportamiento del tráfico y accidentes durante la pandemia.

## Fuentes de Datos:
- **Dataset**: [US Accidents Dataset](https://www.kaggle.com/datasets/sobhanmoosavi/us-accidents)
- **DMV USA**: [Registro en DMV USA](https://api.data.gov/signup/)
- **Weather API**: [API del Clima](https://spire.com/weather/?utm_source=adwords&utm_medium=ppc&utm_campaign=&utm_term=weather+api&hsa_acc=1880479595&hsa_cam=15617857150&hsa_grp=135127222310&hsa_ad=570432678121&hsa_src=g&hsa_tgt=kwd-13737666095&hsa_kw=weather+api&hsa_mt=p&hsa_net=adwords&hsa_ver=3&gad=1&gclid=CjwKCAjwp8OpBhAFEiwAG7NaEvHXdVlVCUCeDD5uaNrrHMJWRpBIXRwvu2tTWNZWIFiNCLh9Y3rEXBoCU_8QAvD_BwE)
- **Road Sensor Api**: [API de Sensores de Carreteras](https://www.isarsoft.com/solutions/traffic?gad=1&gclid=CjwKCAjwp8OpBhAFEiwAG7NaEu16xrf7MXoF8-tZvEqSFqoaANoVVxSNwb1bRb0ac_s6PoltDyqIrRoCYPwQAvD_BwE)

## Componentes de Metodologías y Herramientas Avanzadas:
- **Hadoop y Cluster de Hadoop**: Para el procesamiento de grandes volúmenes de datos.
- **BigQuery**: Para consultas SQL en datasets muy grandes.
- **Jupyter Notebooks**: Para el análisis exploratorio de datos y el prototipado rápido.
- **Datamarts**: Para consultas más rápidas y específicas.
- **Streaming de Datos en Tiempo Real**: Implementación de un pipeline de datos en tiempo real utilizando Kafka.
- **Almacenamiento en Columnas**: Utilidad de Google Bigtable o Apache Cassandra utilizada para consultas analíticas rápidas.
- **Control de Versiones para Datos (DVC)**: Utilizado para mantener un control de versiones de datasets y modelos de machine learning.
- **Automatización y Orquestación de Flujos de Trabajo**: Herramientas como Apache Airflow o Luigi se utilizan para automatizar el pipeline ETL.

## Valor Añadido
Este proyecto no solo proporciona análisis estadísticos, sino insights accionables diseñados para impulsar cambios significativos en la seguridad vial. Al combinar tecnologías de vanguardia en el procesamiento y análisis de Big Data, aspiramos a convertir estos millones de registros en una carretera más segura para todos.

# Diagrama Conceptual del Proceso ETL

Este documento detalla el diagrama conceptual para entender el flujo del proceso ETL (Extracción, Transformación y Carga). Este proceso está organizado en varias fases, cada una con bloques específicos para describir las tareas necesarias.

---

## Fase 1: Configuración del Entorno en la Nube

### Bloque 1.1: # Configuración de Google Cloud Platform (GCP)

En este documento, se detallan los pasos para configurar un proyecto en Google Cloud Platform (GCP) y habilitar las API necesarias.

## Crear un nuevo proyecto en GCP

1. Inicia sesión en tu cuenta de Google o crea una nueva si aún no tienes una.
2. Accede a [Google Cloud Console](https://console.cloud.google.com/).
3. En el panel de navegación, haz clic en "Proyectos".
4. Haz clic en el botón "Crear proyecto" para iniciar el proceso de creación de un nuevo proyecto.
5. Ingresa un nombre único para tu proyecto y opcionalmente puedes personalizar el ID del proyecto.
6. Selecciona la organización (si corresponde) y la ubicación geográfica para el proyecto.
7. Haz clic en "Crear" para crear el proyecto.
8. 
## Habilitar las APIs necesarias

Para habilitar las API necesarias en tu proyecto de GCP, sigue estos pasos:

1. En el panel de navegación de la [Consola de Google Cloud](https://console.cloud.google.com/), haz clic en "API y servicios" y luego en "Biblioteca".
2. Busca la API que deseas habilitar utilizando la barra de búsqueda.
3. Haz clic en la API que deseas habilitar.
4. En la página de la API, haz clic en el botón " Habilitar".

### Bloque 1.2: Configurar Google Storage

- **Sub-bloque**: Crear un nuevo bucket.

:arrow_down_small:  
(*Una flecha desde Fase 1 a Fase 2 indica que la configuración del entorno en la nube debe completarse antes de la ingesta de datos.*)

---

## Fase 2: Ingesta de Datos

### Bloque 2.1: Configurar Kafka para Streaming en Tiempo Real

- **Sub-bloque**: Instalar y configurar Kafka.
- **Sub-bloque**: Definir topics.

### Bloque 2.2: Configurar Flume para Ingesta de Datos en Batch

- **Sub-bloque**: Instalar y configurar Apache Flume.
- **Sub-bloque**: Definir flujos.

:arrow_down_small:  
(*Flechas conectarían las demás fases en orden secuencial.*)

---

## Fase 3: Procesamiento de Datos

### Bloque 3.1: Configurar Cluster de Hadoop

- **Sub-bloque**: Desplegar cluster.
- **Sub-bloque**: Configurar HDFS y MapReduce.

### Bloque 3.2: Configurar Elasticsearch

- **Sub-bloque**: Instalar y configurar Elasticsearch.

:arrow_down_small:

---

## Fase 4: Análisis y Transformación

### Bloque 4.1: Jupyter Notebooks

- **Sub-bloque**: Crear notebooks.

### Bloque 4.2: BigQuery

- **Sub-bloque**: Realizar consultas y análisis.

:arrow_down_small:

---

## Fase 5: Presentación y Visualización

### Bloque 5.1: Tableau

- **Sub-bloque**: Conectar Tableau al Data Warehouse o BigQuery.

### Bloque 5.2: APIs

- **Sub-bloque**: Desarrollar APIs.

:arrow_down_small:

---

## Conexiones

Las fases están conectadas por flechas que indican la secuencia de las operaciones:

- Una flecha desde Fase 1 a Fase 2: Esto implica que la Fase 1 debe completarse antes de pasar a la Fase 2.
- Similarmente, las fases subsecuentes están conectadas por flechas para indicar el flujo de las operaciones.

## Conclusión
Este modelo operacional sirve como una guía detallada para implementar y ejecutar el proyecto "Revolución en Seguridad Vial" de manera eficiente y efectiva.

# Revisión Final del Proyecto "Revolución en Seguridad Vial"

## Resumen
El proyecto "Revolución en Seguridad Vial" tiene como objetivo mejorar significativamente la seguridad en las carreteras de Estados Unidos. Utilizando un conjunto de datos integral de aproximadamente 7.7 millones de registros de accidentes, el proyecto destaca por su ambición de convertir datos en acciones que pueden salvar vidas.

## Fortalezas
- **Enfoque Basado en Datos**: El proyecto utiliza eficazmente un gran conjunto de datos para obtener ideas significativas.
- **Objetivos Integrales**: Desde el modelado predictivo hasta la evaluación del impacto de la COVID-19 en los patrones

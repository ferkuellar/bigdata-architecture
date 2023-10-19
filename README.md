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

## Limitaciones y Consideraciones Legales
Es importante tener en cuenta que el conjunto de datos podría tener días faltantes debido a problemas de conectividad durante la recopilación de datos. Además, el uso de este dataset está restringido a fines de investigación y académicos, y requiere la citación de trabajos académicos específicos.

## Valor Añadido
Este proyecto no solo proporciona análisis estadísticos, sino insights accionables diseñados para impulsar cambios significativos en la seguridad vial. Al combinar tecnologías de vanguardia en el procesamiento y análisis de Big Data, aspiramos a convertir estos millones de registros en una carretera más segura para todos.

# Modelo Operacional del Proyecto "Revolución en Seguridad Vial"

## Introducción
Este documento describe el modelo operacional del proyecto, detallando los pasos a seguir para ejecutar cada componente de la arquitectura propuesta.

## Secuencia de Pasos

### Fase 1: Configuración del Entorno en la Nube
1. **Configurar Google Cloud Platform (GCP)**
    - Crear un nuevo proyecto en GCP.
    - Habilitar las APIs necesarias (BigQuery, Google Storage, etc.).
    
2. **Configurar Google Storage**
    - Crear un nuevo bucket para almacenar los datasets y otros recursos.

### Fase 2: Ingesta de Datos
1. **Configurar Kafka para Streaming en Tiempo Real**
    - Instalar y configurar Kafka en un cluster.
    - Definir los topics para las distintas fuentes de datos.

2. **Configurar Flume para Ingesta de Datos en Batch**
    - Instalar y configurar Apache Flume.
    - Definir los flujos para la ingestión de datos.

### Fase 3: Procesamiento de Datos
1. **Configurar Cluster de Hadoop**
    - Desplegar un cluster de Hadoop en la nube o en servidores locales.
    - Configurar HDFS y MapReduce.

2. **Configurar Elasticsearch**
    - Instalar y configurar Elasticsearch para análisis en tiempo real.

### Fase 4: Análisis y Transformación
1. **Jupyter Notebooks**
    - Crear notebooks para análisis exploratorio de datos y prototipado.
    
2. **BigQuery**
    - Realizar consultas complejas y análisis profundos usando BigQuery.

### Fase 5: Presentación y Visualización
1. **Tableau**
    - Conectar Tableau al Data Warehouse o a BigQuery para crear dashboards.

2. **APIs**
    - Desarrollar APIs para compartir resultados en tiempo real.

### Fase 6: Monitoreo y Mantenimiento
1. **Herramientas de Monitoreo**
    - Implementar herramientas de monitoreo para evaluar el rendimiento del sistema.

2. **Control de Versiones con DVC**
    - Implementar DVC para el control de versiones de datasets y modelos de machine learning.

## Conclusión
Este modelo operacional sirve como una guía detallada para implementar y ejecutar el proyecto "Revolución en Seguridad Vial" de manera eficiente y efectiva.

# Revisión Final del Proyecto "Revolución en Seguridad Vial"

## Resumen
El proyecto "Revolución en Seguridad Vial" tiene como objetivo mejorar significativamente la seguridad en las carreteras de Estados Unidos. Utilizando un conjunto de datos integral de aproximadamente 7.7 millones de registros de accidentes, el proyecto destaca por su ambición de convertir datos en acciones que pueden salvar vidas.

## Fortalezas
- **Enfoque Basado en Datos**: El proyecto utiliza eficazmente un gran conjunto de datos para obtener ideas significativas.
- **Objetivos Integrales**: Desde el modelado predictivo hasta la evaluación del impacto de la COVID-19 en los patrones

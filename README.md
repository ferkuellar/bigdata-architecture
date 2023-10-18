# Traffic Accident Risk Prediction Project

## Finalidad del Proyecto
El proyecto se enfoca en el análisis y la predicción del riesgo de accidentes de tráfico en los Estados Unidos. Utiliza un extenso conjunto de datos que abarca desde febrero de 2016 hasta marzo de 2023. Este conjunto de datos, con aproximadamente 7.7 millones de registros de accidentes, fue recopilado en tiempo real utilizando diversas APIs de tráfico. Las fuentes de información son variadas, incluyendo departamentos de transporte, agencias policiales, cámaras de tráfico y sensores de carreteras.

## Objetivos Específicos
- **Predicción de la Severidad de los Accidentes**: Utilizar variables como la hora del día, condiciones climáticas y ubicación para modelar y predecir la severidad de los accidentes.
- **Análisis de Hotspots de Accidentes**: Identificar áreas geográficas con altas tasas de accidentes.
- **Impacto de las Condiciones Climáticas y Ambientales**: Examinar cómo factores como la lluvia, la presión atmosférica y la visibilidad afectan la probabilidad de accidentes.
- **Evaluación de Infraestructuras Viales**: Analizar el impacto de las señales de tráfico, rotondas y otros elementos de infraestructura.
- **Comportamiento de Conducción durante la Pandemia de COVID-19**: Utilizar datos más recientes para analizar cambios en el comportamiento del tráfico y accidentes durante la pandemia.

## Metodologías y Herramientas Avanzadas
- **Hadoop y Cluster de Hadoop**: Para el procesamiento de grandes volúmenes de datos.
- **BigQuery**: Para consultas SQL en datasets muy grandes.
- **Jupyter Notebooks**: Para el análisis exploratorio de datos y prototipado rápido.
- **Datamarts**: Para consultas más rápidas y específicas.
- **Streaming de Datos en Tiempo Real**: Implementación de un pipeline de datos en tiempo real usando Kafka.
- **Almacenamiento en Columnas**: Utilidad de Google Bigtable o Apache Cassandra para consultas analíticas rápidas.
- **Control de Versiones para Datos (DVC)**: Para mantener un control de versiones de datasets y modelos de machine learning.
- **Automatización y Orquestación de Flujos de Trabajo**: Uso de herramientas como Apache Airflow o Luigi para automatizar el pipeline ETL.

## Limitaciones y Consideraciones Legales
Es importante tener en cuenta que el conjunto de datos podría tener días faltantes debido a problemas de conectividad durante la recopilación de datos. Además, el uso de este dataset está restringido a fines de investigación y académicos, y requiere la citación de trabajos académicos específicos.

## Fuentes de Datos
- APIs de Tráfico
- Sensores de Carreteras
- Bases de datos de agencias gubernamentales

## Ingesta de Datos
- Kafka para streaming de datos en tiempo real
- Flume para la ingesta de datos en batch

## Procesamiento y Almacenamiento
- Cluster de Hadoop con HDFS para almacenamiento y MapReduce para procesamiento
- Elasticsearch para búsquedas de texto completo y análisis en tiempo real

## Análisis y Transformación de Datos
- Jupyter Notebooks para análisis exploratorio y prototipado

## Datamarts y Data Warehouse
- Creación de datamarts específicos para diferentes aspectos como condiciones climáticas, ubicaciones geográficas, etc.
- Data Warehouse para un almacenamiento más estructurado y consultas

## Orquestación y Automatización
- Control de Versiones para Datos (DVC)

## Presentación y Visualización
- Tableau para dashboards y visualizaciones interactivas
- APIs para compartir resultados en tiempo real con otras aplicaciones o stakeholders

## Monitoreo y Mantenimiento
- Herramientas de monitoreo para el rendimiento del sistema y la calidad de los datos

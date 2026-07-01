Proyecto: Pipeline de Datos Escalable para Análisis Financiero (AdventureWorks)
Descripción del Proyecto Este proyecto fue desarrollado para resolver la necesidad de centralizar y visualizar datos transaccionales masivos. El desafío principal fue superar las limitaciones de red e infraestructura para construir un Data Warehouse (DWH) en la nube funcional y escalable, capaz de soportar análisis de inteligencia de negocios.

Pipeline ETL (Extract, Transform, Load)
El pipeline fue diseñado bajo una arquitectura de ingeniería de datos moderna:

Extracción: Generación de datos sintéticos masivos mediante Python (Pandas y NumPy) en memoria para asegurar la disponibilidad inmediata de la fuente.

Transformación: Aplicación de reglas de negocio para el cálculo de métricas financieras (Facturación Bruta, Ganancia Neta) y normalización de tipos de datos para asegurar la integridad financiera.

Carga: Ingesta de datos hacia una instancia de PostgreSQL alojada en la nube (Render), garantizando la persistencia y seguridad mediante protocolos SSL.

Tecnologías Utilizadas
Python: Orquestación del pipeline, transformación de datos y automatización de procesos.

PostgreSQL (Render): Data Warehouse centralizado y escalable en la nube.

Power BI: Capa de visualización y análisis interactivo (BI).

SQLAlchemy: Gestión de conexiones seguras entre el pipeline y el servidor de base de datos.

Visualizaciones
Dashboard principal mostrando la tendencia de facturación y el margen de beneficio por producto. Esquema relacional optimizado, incluyendo la Tabla de Calendario para análisis temporal.

Conclusiones e Insights
Tras el modelado y visualización, se obtuvieron los siguientes hallazgos:

Tendencia de Crecimiento: La visualización de la serie temporal permitió identificar periodos pico de facturación que no eran evidentes en los datos crudos.

Análisis de Rentabilidad: Se detectaron productos de alto volumen pero baja rentabilidad, lo que permite proponer estrategias de optimización de costos o ajustes de precios.

Eficiencia del Pipeline: La automatización del flujo ETL redujo drásticamente el tiempo de preparación de datos, permitiendo que el reporte se actualice de forma dinámica directamente desde la fuente en la nube.

## Proyecto: Data Engineering Pipeline & Analytics (AdventureWorks)
Descripción
Este proyecto implementa un flujo completo de Ingeniería de Datos (ETL), desde la generación y transformación de datos hasta la creación de un sistema de Business Intelligence (BI). El objetivo fue centralizar transacciones masivas de AdventureWorks en un Data Warehouse en la nube para habilitar la toma de decisiones basada en datos.

## Stack tecnologico ##

Lenguajes: Python (Pandas, NumPy).

- Ingeniería Cloud: PostgreSQL alojado en Render (Infraestructura como servicio).

- Conectividad: SQLAlchemy (ORM para gestión de bases de datos).

- Business Intelligence: Power BI (Modelado de datos, DAX y visualización).

- Versionado: Git & GitHub (Gestión del ciclo de vida del código).


## Arquitctura del pipeline ##
El flujo de datos sigue el estándar de la industria:

- Extracción (Extract): Simulación de carga masiva de transacciones en memoria (RAM) mediante Python para asegurar independencia y agilidad.

- Transformación (Transform): Limpieza de datos, imputación de valores faltantes y cálculo de KPIs financieros clave (Facturación Bruta, Margen Neto).

- Carga (Load): Ingesta estructurada hacia una base de datos PostgreSQL remota, utilizando protocolos SSL para garantizar la seguridad en tránsito.

- Presentación (BI): Creación de un modelo de datos relacional en Power BI, utilizando una Tabla de Calendario dedicada para habilitar la Inteligencia de Tiempo (Time Intelligence).

## Hallazgos y Resultados ##

- Optimización de Datos: Se logró transformar miles de transacciones crudas en un modelo relacional limpio, listo para visualización.

- Inteligencia de Tiempo: Gracias al modelado con CALENDARAUTO(), el sistema permite comparativas temporales avanzadas (Año contra Año, tendencia mensual).

- Despliegue Cloud: El pipeline demuestra capacidad para operar en entornos cloud remotos, manejando credenciales y conexiones seguras.

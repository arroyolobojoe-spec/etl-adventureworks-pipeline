ETL Pipeline: AdventureWorks Analytics
Proyecto de ingeniería de datos desarrollado para extraer, transformar y cargar (ETL) información masiva de transacciones, con un enfoque en calidad de datos, imputación analítica y despliegue en entornos en la nube.

🚀 Descripción del Proyecto
Este pipeline automatiza el procesamiento de datos transaccionales simulados de AdventureWorks. El objetivo principal es transformar datos crudos en un esquema relacional estructurado, optimizado para el análisis financiero y la toma de decisiones. El flujo incluye la aplicación de reglas de negocio, manejo de valores nulos, generación de indicadores clave (KPIs) y carga en una base de datos PostgreSQL alojada en la nube (Render).

🛠 Tecnologías Utilizadas
Lenguaje: Python 3.x

Procesamiento de datos: Pandas, NumPy

Conectividad: SQLAlchemy (PostgreSQL)

Infraestructura: Render (Cloud PostgreSQL)

Entorno de desarrollo: Google Colab

⚙️ Arquitectura del Pipeline (E-T-L)
Extract (E): Generación y carga en memoria de 25,000 registros transaccionales con integridad referencial.

Transform (T):

Cruce de dimensiones (Productos vs. Ventas).

Limpieza y estandarización de esquemas.

Imputación de valores nulos basada en promedios estadísticos.

Cálculo de métricas financieras: facturacion_bruta y ganancia_neta.

Load (L): Inyección de datos estructurados hacia una instancia de PostgreSQL en la nube mediante un túnel seguro.

ESTRUCTURA DEL REPOSITORIO

etl-adventureworks-pipeline/
├── NOTEBOOK/
│   └── PROYECTO_REAL_ETL.ipynb    # Pipeline principal (ETL)
├── .gitignore                     # Archivos excluidos (entornos y secretos)
└── README.md                      # Documentación del proyecto
Seguridad y Buenas Prácticas
Manejo de Secretos: Este proyecto utiliza google.colab.userdata para la gestión segura de las credenciales de la base de datos, evitando la exposición de contraseñas en el código fuente.

Control de Versiones: Se han implementado archivos .gitignore para asegurar que archivos temporales, caché y variables de entorno no sean registrados en el historial del repositorio.

Resultados del Pipeline
El proceso garantiza una ingesta de alta velocidad, validando los datos en tiempo real mediante un sistema de logging DevOps que monitorea cada fase de la ejecución, asegurando la trazabilidad del proceso desde la extracción hasta la persistencia final en PostgreSQL.



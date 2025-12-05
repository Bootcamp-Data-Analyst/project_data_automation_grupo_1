📦 Proyecto de Automatización
MySQL → Python → CSV → Excel Dashboard

Autores: Dani · Raúl · Alejandro

📝 Descripción General del Proyecto

Este proyecto implementa un pipeline automatizado de extracción, transformación y carga (ETL) que conecta una base de datos MySQL con un entorno de análisis basado en Python y Excel.
El objetivo final ha sido crear un sistema que permita actualizar datos automáticamente y visualizar esa información de forma clara mediante un dashboard profesional en Excel.

El proyecto se ha realizado en equipo (Dani, Raúl y Alejandro) aplicando buenas prácticas de desarrollo, control de versiones y reparto equilibrado de tareas.

🎯 ¿Qué hemos hecho?
✔ 1. Diseñamos un flujo de trabajo completo y automatizado

Creamos un pipeline donde Python extrae datos de MySQL, los transforma con Pandas y genera un fichero CSV listo para Excel.
El dashboard de Excel se actualiza automáticamente al abrirse.

✔ 2. Construimos un script ETL profesional

Conexión a MySQL con sqlalchemy y mysql-connector-python.

Consultas SQL optimizadas sobre la base de datos Sakila.

Limpieza, combinación y transformación de tablas con Pandas.

Exportación automática a output/datos_sakila.csv.

✔ 3. Creamos un dashboard visual e interactivo

Diseñamos un archivo Excel con 3 hojas:

Datos: conectado al CSV

Tablas dinámicas: base analítica

Dashboard: gráficos, KPIs y segmentaciones

✔ 4. Documentamos y organizamos el proyecto

Incluimos esta guía (README), variables de entorno, estructura limpia de carpetas y un control de versiones con Git y GitHub.

🧠 ¿Cómo lo hemos hecho?
1) Organización del Trabajo en Equipo

El trabajo se ha desarrollado de forma cooperativa entre:

👨‍💻 Alejandro

Configuración del entorno (venv, dependencias, .env).

Estructura del proyecto y archivo main.py.

Redacción de la documentación (README final).

Integración y pruebas completas del pipeline.

👨‍💻 Dani

Encargado de consultas SQL y testeo en la base Sakila.

Limpieza y normalización de datos con Pandas.

Comprobación de integridad y calidad del dataset generado.

Diseño inicial del dashboard (gráficos y segmentaciones).

👨‍💻 Raúl

Conexión a MySQL y módulo config.py.

Automatización de la exportación a CSV.

Generación de la hoja “Datos” y control de rutas.

Depuración de errores y testing conjunto.

🤝 Trabajo colaborativo

Todo el proyecto versionado en GitHub.

Correcciones y pruebas hechas en conjunto.

Reuniones breves para tomar decisiones (estructura, diseño del dashboard, consultas SQL, etc.).

🧩 Proceso Técnico
1. Instalación y entorno

Configuración de MySQL con base Sakila

Creación de entorno virtual

Instalación de dependencias

Configuración de credenciales en .env

2. Desarrollo del pipeline
🔎 Extracción

Consultas SQL realizadas por Dani y Raúl para obtener:

Clientes

Ciudades y países

Alquileres

Pagos

Ingresos y patrones temporales

🔧 Transformación

Uso de pandas para:

Uniones entre tablas

Limpieza de duplicados

Cálculo de ingresos por cliente, ciudad, país

KPI básicos: tickets medios, número de alquileres, clientes VIP

📤 Carga

Exportación automática al CSV final:

output/datos_sakila.csv

3. Visualización en Excel

El equipo diseñó conjuntamente:

Tablas dinámicas

Gráficos de líneas, barras y mapas

Segmentaciones por país, cliente o fecha

Dashboard profesional con diseño unificado

🗂️ Estructura del Proyecto
proyecto-sakila-automation/
│
├── main.py                       
├── src/
│   ├── __init__.py
│   ├── sakila_ETL.py           
│   └── config.py               
│
├── output/
│   └── datos_sakila.csv        
│
├── dashboard/
│   └── sakila_dashboard.xlsx   
│
├── requirements.txt
├── .env
├── .env.example
├── .gitignore
└── README.md

▶️ Ejecución
python main.py


Esto ejecuta todo el pipeline y actualiza el CSV.
Después, solo hay que abrir el Excel para que se refresquen los datos.

🧪 Criterios Cubiertos

✔ Automatización del entorno de trabajo
✔ Gestión y coordinación del equipo
✔ ETL funcional y documentado
✔ Evaluación y depuración del dataset
✔ Dashboard dinámico y profesional
✔ Uso correcto de Git y GitHub
✔ Documentación clara y completa

👥 Autores

Dani – Raúl – Alejandro
Trabajo colaborativo en Python, MySQL y Excel.

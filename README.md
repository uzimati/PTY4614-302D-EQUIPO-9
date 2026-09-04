# Proyecto_Capstone_302D
#  Sistema de Automatización de Firmas Digitales y Migración a Oracle

![Status](https://img.shields.io/badge/Estado-En_Desarrollo-orange?style=flat-square)
![Database](https://img.shields.io/badge/Base_de_Datos-Oracle-red?style=flat-square&logo=oracle)
![ETL](https://img.shields.io/badge/ETL-Python-blue?style=flat-square&logo=python)

##  Descripción del Proyecto
Este proyecto es una solución empresarial diseñada para automatizar el proceso de legalización de firmas digitales, eliminando cuellos de botella administrativos y reduciendo el margen de error humano. 

El núcleo del proyecto aborda la migración de un sistema de gestión documental obsoleto (basado en archivos planos de Excel) hacia una arquitectura de base de datos relacional robusta en **Oracle**. Esto permite establecer un entorno seguro, escalable y con trazabilidad completa sobre las interacciones de los usuarios y los documentos firmados.

##  Características Principales (Features)

- **Migración ETL (Excel a Oracle):** Scripting automatizado para la extracción, limpieza (data wrangling), normalización y carga masiva de registros históricos desde hojas de cálculo hacia el modelo relacional.
- **Automatización de Firmas Digitales:** Flujo automatizado para la validación y aplicación de firmas en documentos, asegurando su integridad y valor legal.
- **Control de Acceso Basado en Roles (RBAC):** Gestión granular de permisos donde cada usuario tiene accesos restringidos según su perfil (Ej. Administrador, Firmante, Auditor).
- **Trazabilidad y Auditoría:** Registro inmutable (Logs) de cada acción realizada en el sistema, capturando timestamps, usuario y tipo de operación para cumplir con normativas de seguridad.

##  Arquitectura y Modelo de Datos

La transición desde un modelo plano a un modelo relacional en Oracle se estructura en torno a las siguientes entidades principales (esquema inicial):

* `USUARIOS`: Credenciales, datos personales y estado.
* `ROLES` / `PERMISOS`: Definición de accesos (RBAC).
* `DOCUMENTOS`: Metadatos del archivo, rutas de almacenamiento y estado de la firma.
* `AUDITORIA`: Historial inmutable de eventos del sistema (triggers).

##  Stack Tecnológico

* **Base de Datos:** Oracle Database (PL/SQL, Triggers, Relational Modeling).
* **ETL & Scripting:** Python (Pandas, cx_Oracle / SQLAlchemy).
* **Gestión de Proyecto:** Metodologías ágiles, control de calidad (QA) y documentación técnica.

##  Instalación y Configuración Local

1. **Clonar el repositorio:**
   ```bash
   git clone [https://github.com/tu-usuario/nombre-del-repo.git](https://github.com/tu-usuario/nombre-del-repo.git)
   cd nombre-del-repo

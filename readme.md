# Instructivo: exportación de datos a la DB SQL-UNLu

El objetivo de este instructivo es explicar los pasos a seguir para exportar los registros relacionados a la actividad académica de la Universidad a una base de datos relacional, compatible con PostgreSQL 9.5, para la ejecución de consultas complejas para la generación de información para la toma de decisiones.

## 1. Conceptos iniciales

### 1.1. Modelo de datos

A continuación se presenta el modelo de datos de la Base de Datos SQL:

### 1.2. Herramientas de software

Para la exportación de los datos, la gestión de la información y la persistencia se utilizarán las siguientes herramientas:
- PHP 7.0,
- PostgreSQL 9.5,
- PgAdmin 3.

## 2. Ejecución del proceso

### 2.1. Creación de la Base de Datos

Se asume que la base de datos ya existe y posee el nombre __exportaciones_unlu__, no obstante si se deseara generar una base de datos habría que seguir los siguientes pasos:

1. Abrir PgAdmin 3 y hacer doble click sobre el Servidor (en nuestro caso __Localhost__) o presionar click derecho y seleccionar _Connect_.

![Conectar Servidor](./imagenes/C1.png)

2. Se presiona el click derecho en el ícono _Databases_, dependiente del Servidor, y se selecciona _New Database..._.

![Crear DB](./imagenes/C2.png)

3. Aquí se define el nombre en la etiqueta _Name_ y en la pestaña _Definition_ nos aseguramos que el encoding sea _UTF-8_.

![Atributos DB](./imagenes/C3.png)

Si pudimos seguir estos pasos, ya tenemos una base de datos creada y nos podemos conectar a la misma haciendo doble click.

### 2.2. Actualización de la Base de Datos desde Backup

### 2.3. Actualización de la Base de Datos desde Exportaciones del Módulo Externo









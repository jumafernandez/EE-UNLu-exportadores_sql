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

Es una buena práctica de preservación de los datos ir generando backups periodicamente para evitar perdidas de información y al mismo tiempo conservar diferentes estados de la Base de Datos para reconstruir series de Anuarios Estadísticos publicados.
A continuación, se explica paso a paso como generarlos y como restaurar esos Backups.

#### 2.2.1. Crear Backup desde la Base de Datos

Para generar un backup con los datos de la Base de datos desde PgAdmin, debe conectarse al Servidor y haciendo click derecho presionamos sobre _Backup_.

![Realizar Backup](./imagenes/C4.png)



#### 2.2.2. Restaurar Backup de la Base de Datos

Para restaurar el Backup, previamente debemos crear la Base de Datos de acuerdo a los pasos explicados en _2.1. Creación de la Base de Datos_. Una vez creada la Base de Datos, desde PgAdmin, debe conectarse al Servidor y haciendo click derecho sobre la Base creada elegimos la opción _Restore_. Seleccionamos el archivo creado mediante los pasos de _2.2.1 Crear Backup desde la Base de Datos_ y presionamos el botón _Restore_.

### 2.3. Actualización de la Base de Datos desde Exportaciones del Módulo Externo









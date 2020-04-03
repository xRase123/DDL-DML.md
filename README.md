# Apuntes/DDL&DML-JavierCamposAlvedro(ASI105)
Apuntes sobre DDL e DML de la asignatura de Bases de Datos.

# Índice:
1. [DDL](#DDL)
2. [Ej-DDL](#Ejemplos_Prácticos-DDL)
3. [DML](#DML)
4. [Ej-DML](#Ejemplos_Prácticos-DML)
5. [WebGrafía / Infografía](#WebGrafía-Infografía)

# DDL
Es un lenguaje de programación para definir estructuras de datos, proporcionado por los sistemas gestores de bases de datos. En inglés, Data Definition Language, de ahí sus siglas DDL.

# Ejemplos_Prácticos-DDL
1.  - Check: Nos permite limitar los valores de los atributos.

2.    *CREATE TABLE mecánicos (
  nombre VARCHAR(25) PRIMARY KEY,
  fechaInicio DATE, 
  fechaFinalización DATE,
  CONSTRAINT Check_fechas
    CHECK (fechaInicio < fechaFinalización),
    );*
    
3.  - Create: Nos permite crear una base de datos, tabla, vistas, etc.

4.   *CREATE DATABASE <nombre_bd>;*

5.  - Drop: Nos permite eliminar los objetos de la estructura, por ejemplo un índice o una secuencia.

6.   *DROP DATABASE <nombre_bd>*

7.  - Alter: Nos permite modificar la tabla y añadir o quitar columnas.

8.   *ALTER TABLE <nombre_tabla>
    [RENAME TO <nuevo_nombre>],
    [RENAME COLUMN <nombre_columna> TO <nuevo_nombre>],
    [ADD | DROP [COLUMN | CONSTRAINT] <nombre>];*

# DML
También es un lenguaje proporcionado por los sistemas gestores de bases de datos. En inglés, Data Manipulation Language (DML).

Utilizando instrucciones de SQL, permite a los usuarios introducir datos para posteriormente realizar tareas de consultas o modificación de los datos que contienen las Bases de Datos.

# Ejemplos_Prácticos-DML
1.  - Select: Nos permite realizar consultas sobre los datos.

2.  *SELECT nombre_columna, nombre_columna2
     FROM nombre_tabla;*
     
3.  - Insert: Nos permite insertar valores en una base de datos.

4.  *INSERT INTO <nombre_tabla> *

5.  - Update: Nos permite modificar los valores de uno o varios registros.

6.  *UPDATE <nombre_tabla>*

7.  - Delete: Nos permite eliminar las filas de una tabla.

8.  *DELETE FROM <nombre_tabla>*

# WebGrafía-Infografía
1. [POSTGRESQL](https://www.postgresql.org/docs/)
2. [WIKIPEDIA](https://es.wikipedia.org/wiki/SQL)
3. [POSTGRESQL](https://todopostgresql.com/diferencias-entre-ddl-dml-y-dcl/)
4. [EDU4JAVA](http://www.edu4java.com/es/sql/sql4.html)


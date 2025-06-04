# 📌 Introducción a SQL

**SQL** (*Structured Query Language*) es un lenguaje estándar para gestionar bases de datos relacionales. Permite crear, consultar, actualizar y eliminar datos de forma estructurada.

## 🔍 Conceptos Básicos

### 1. **Bases de Datos Relacionales**
- Datos organizados en **tablas** (filas y columnas).
- Cada tabla tiene una **clave primaria** (identificador único).

### 2. **Comandos Principales**
| Categoría       | Comandos                 | Ejemplo                          |
|-----------------|--------------------------|----------------------------------|
| **Consultas**   | `SELECT`                 | `SELECT * FROM clientes;`        |
| **Modificación**| `INSERT`, `UPDATE`, `DELETE` | `INSERT INTO clientes (nombre) VALUES ('Ana');` |
| **Estructura**  | `CREATE`, `ALTER`, `DROP`| `CREATE TABLE productos (id INT, nombre VARCHAR(50));` |

## 📊 Ejemplo Práctico

### Crear una tabla y consultar datos:
```sql
-- Crear tabla
CREATE TABLE empleados (
    id INT PRIMARY KEY,
    nombre VARCHAR(50),
    salario DECIMAL(10, 2)
);

-- Insertar datos
INSERT INTO empleados (id, nombre, salario)
VALUES (1, 'Carlos', 3000.50);

-- Consultar
SELECT nombre, salario FROM empleados WHERE salario > 2000;
🔗 Recursos Útiles
SQLZoo: Tutoriales interactivos.

W3Schools SQL: Guía de referencia rápida.

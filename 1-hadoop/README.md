# 🐘 **Hadoop - Mis Notas**  

Hadoop es un framework de código abierto diseñado para el procesamiento distribuido de grandes volúmenes de datos (Big Data) en clusters de computadoras. 

¿Qué es Hadoop?
Definición: Plataforma que permite almacenar y procesar datos masivos de forma distribuida y paralela.

Origen: Creado por Apache (inspirado en los papers de Google sobre MapReduce y GFS).

Lenguaje: Principalmente Java, pero soporta otros como Python o Scala.

Componentes principales:
HDFS (Hadoop Distributed File System):

Sistema de archivos distribuido (almacena datos en múltiples servidores).

Ejemplo en bash:
hdfs dfs -ls /data  # Lista archivos en HDFS

YARN (Yet Another Resource Negotiator):Gestiona recursos del cluster (CPU, memoria).  

MapReduce: Modelo de programación para procesar datos en paralelo.  

Librerías adicionales: HBase (base de datos NoSQL), Hive (consultas SQL), Spark (procesamiento en memoria).  

En resumen:
1. Almacenas datos en HDFS (bash): Almacenas datos en HDFS (bash):  
hdfs dfs -put datos.csv /input
2. Procesas con MapReduce/Spark.
3. Resultados se guardan en HDFS o bases de datos.
-----------------------------------------------------------



## 1. HDFS  
**Aprendido hoy**:  
- Los bloques en HDFS por defecto son de **128MB**.  
- La replicación se configura en `hdfs-site.xml`.  

## 2. Comando que usé  
```bash
# Subir un archivo local al HDFS  
hdfs dfs -put /home/user/data.csv /datos-entrada/
```  

## 3. Dudas pendientes  
- ¿Cómo optimizar el tamaño de bloques para datasets pequeños?  
 
 
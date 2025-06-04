# 🐘 **Hadoop - Mis Notas**  

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
# big-data-learning ( Ejemplo del inicio y creación de carperta)
Paso 1.  
Crear en github.com/new.  
a) Nombre: big-data-learning (nombre de repositorio).  
b) "Add a README file" (opcional, pero útil).  
c) "Create repository".  

Paso 2.  
Clonar repositorio local  

git clone https://github.com/nilyeh/big-data-learning.git  
cd big-data-learning  

Paso 3.  
Estructura Recomendada del Repositorio  
Crea estas carpetas y archivos dentro de big-data-learning:  

código bash:  
mkdir -p {1-hadoop,2-spark,3-kafka,proyectos}/ejemplos  
touch README.md 1-hadoop/README.md 2-spark/README.md recursos.md  
$ mkdir -p docs/imagenes  # Crea la carpeta si no existe  
git add docs/imagenes/mi-imagen.png # mi-imagen.png = estructura 1.jpg    
git commit -m "Agregar imagen para README"  
git push origin main  

3.2. Insertar la imagen en el README.md  
Opción A: Markdown (recomendado)  
![Estructura inicial](docs/imagenes/estructura1.jpg)  

Nota: la imagen se inserta directo en el Readme.md, Usa rutas relativas (desde la raíz del repositorio), no absolutas  
En este ejemplo de inserción de imagen, no se incluye la carpeta docs que contiene las imagenes**  
codigo:  
![Texto alternativo](ruta/a/la/imagen.png)

# GUÍA  GIT & MARKDOWN

## 1. COMANDOS GIT ESENCIALES

### Crear repositorio desde cero:
mkdir nombre-proyecto
cd nombre-proyecto
git init
touch README.md
git add .
git commit -m "Initial commit"
git remote add origin [URL_DEL_REPO]
git push -u origin main

### Subir cambios:
git add nombre-archivo
git commit -m "Descripción del cambio o Mensaje"
git push origin main

## 2. ESTRUCTURA DE CARPETAS

### Crear estructura con subdirectorios:
mkdir -p {1-hadoop,2-spark,3-kafka,proyectos}/ejemplos  
Explicación:
-p: Flag que permite crear múltiples directorios anidados de una vez.

### Crear archivos base:
touch README.md 1-hadoop/README.md 2-spark/README.md recursos.md  
Explicación Archivos creados:  
README.md: En el directorio raíz del proyecto.  
1-hadoop/README.md: Dentro de la carpeta 1-hadoop.  
2-spark/README.md: Dentro de la carpeta 2-spark.  
recursos.md: En el directorio raíz.  
touch: Comando para crear archivos vacíos (o actualizar su fecha de modificación si ya existen).  

## 3. IMÁGENES EN README.md

### Pasos para agregar imágenes:
1. Crear carpeta para imágenes:
mkdir -p docs/imagenes

2. Mover imagen a la carpeta:
mv ruta/origen/imagen.png docs/imagenes/

3. Insertar en README.md:
![Texto alternativo](docs/imagenes/imagen.png)

## 4. FORMATO MARKDOWN

### Espacios y saltos de línea:
- Dos espacios al final + Enter para salto de línea  
- Línea vacía para nuevo párrafo

### Encabezados:
# Título Principal
## Subtítulo
### Subsección

### Listas:
- Item 1
- Item 2
  - Subitem (con 2 espacios)

### Códigos:
`git status` (inline)


# big-data-learning
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
git add docs/imagenes/mi-imagen.png # laimagen se llama estructura 1  
git commit -m "Agregar imagen para README"  
git push origin main  

3.2. Insertar la imagen en el README.md  
Opción A: Markdown (recomendado)  
![Estructura inicial](docs/imagenes/estructura1.jpg)  

Nota: la imagen se inserta directo en el Readme.md, Usa rutas relativas (desde la raíz del repositorio), no absolutas  

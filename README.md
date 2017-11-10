# Curso Git-Github

## Que es un sistema de control de versiones

Registra los cambios realizados sobre un  archivo \(o cunjunto de archivos\) en el tiempo.

## Tipos de sistemas de control de versiones

* **Local**: Almacenado en el sistema de archivos local
* **Centralizado**: El repositorio esta almacenado en un server que provee copias a otras terminales para que puedan modificarlo. 
* **Distribuido**: Cada usuario que participa en el repositorio tiene una copia completa del repositorio en su equipo, es el caso de **git**.

## Beneficios de usar Git

Creado por Linus Torvalds cuanto hicieron propietario el software que usaba para versionar el kernel de linux.

**Ventajas**

1. Velocidad.
2. Diseño sencillo. 
3. Desarrollo no lineal.
4. Distribuido.
5. Puede mantener grandes proyectos.

Guarda _referencias_ de todos los archivos en el tiempo.

## Estados de Git

1. ### Working Directory

   1. Archivos locales que aun no se han incluido al repositorio e.g un archivo HTML local al que no se le ha hecho commit
2. ### Staging Area

   1. Archivos del working directory que estan listos para ser agregados al repositorio.
3. ### Git Directory

   1. En donde se almacenan los cambios, es el repositorio en si.

## Github

Es un hosting en el que se almacenan los cambios en internet, permite la colaboración en un proyecto por medio de internet, ayuda en la organización de los proyectos

* Permite marcar bugs.
* Permite poner tareas.
* Mantiene una copia en la _nube_ de el repositorio.
* Tiene muchas otras funcionalidades.

## Instalación en Linux \(debian\)

```
sudo apt-get install git
```

## Configuración basica

```
git config --global user.email user@host.com
```

```
git config --global user.name mcnameface
```

```
git config --global color.ui true
```

## Comandos basicos de terminal para git

```
cd ## permite moverse entre carpetas 
cd .. navega hacia atras en las carpetas
```

```
mkdir ## crea carpetas desde la terminal
touch ## crea (archivos) 
rm ## borra archivos
rm -rf ## borra directorios vacios (o todo tu pc)
ls ## lista los ficheros
```

## Crear repositorios de forma local

```
git init primer_repo ## crea un repositorio en la carpeta primer_repo
```

```
rm -rf .git
```

## Agregar, quitar y ver status de los archivos

```
touch index.html
```

```
git status ## muestra el estado del repositorio
```

```
git add index.html ## agrega el archivo al staging
```

```
git rm --cached index.html ## saca el archivo del staging
```

```
git add -A ## agrega todos los archivos al staging
```

```
git rm -f [archivo] ## borra el archivo del staging y de el equipo
```

```
git add  -n [archivo] muestra si un archivo existe
```

## Confirmando cambios

```
git commit -m "mensaje" ## confirma los cambios y agrega un mensaje
```

```
--amend ## concatena este commit con un commit anterior
```

```
git log ## muestra historial de commits
```

## Etiquetando confirmaciones

```
git tag ## agrega etiquetas
 -a anotación
 -m mensaje
 -l lista de etiquetas
 -d borra un tag
 -f para agregar un tag adicional o para reemplazar un tag anterior
```

```
git tag [tag] [sha1] ## agrega tag al commit con un sha1 determinado
```

```
## agrega un tag con un mensaje al commit con un sha1 determinado
git tag -f -a [tag] -m "mensaje" [sha1]
```

## Revisar el historial del proyecto

```
git log
```

```
git log --oneline un log resumido
```

```
## muestra un grafico detallado del proyecto en caso de que este contenga branches
git log --oneline --graph
```

```
git log -[num] muestra un número determinado de commits
```

Es un comando altamente configurable \(revisar la documentación de git\)

## Revisando cambios entre versiones

```
git diff [sha1] ## muestra cambios entre el commit inicial
```

```
git diff [sha1A] [sha1B]  ## compara dos commits (versiones)
```

## Quitar cambios

```
git reset --soft [sha1] 
## quita los cambios de el commit que sigue al sha1 determinado 
## no borra cambios en los archivos
```

```
git reset --mixed [sha1]
## quita los cambios del repositorio y del stage
git reset HEAD [archivo] 
## mixed reset manual
```




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

   1. En donde se almacenan los cambios.

## Github

Es un hosting en el que se almacenan los cambios en internet, permite la colaboración en un proyecto por medio de internet, ayuda en la organización de los proyectos

* Permite marcar bugs.
* Permite poner tareas.
* Mantiene una copia en la _nube_ de el repositorio.

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




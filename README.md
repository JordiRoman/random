Modulo 5 Ejercicio P2P Obligatorio

# Objetivo
El objetivo del ejercicio es habituarse al uso de git de forma basica

# Origen del proyecto
El proyecto original lo podemos clonar desde https://github.com/jquemada/random

# Instrucciones y/o guion de trabajo
Primero configuraremos los aspectos basicos de la instalacion de git local
 $ git config --global user.name "Jordi Román Mejias"
 $ git config --global user.email jordi.roman@gmail.com
 $ git config --list

A continuación podemos clonar el repositario original con el comando

 $ git  clone https://github.com/jquemada/random
 Cloning into 'random'...
 remote: Counting objects: 7, done.
 remote: Total 7 (delta 0), reused 0 (delta 0), pack-reused 7
 Unpacking objects: 100% (7/7), done.
 Checking connectivity... done.

El resultado es un directorio random, con el fichero random.js

# Modificaciones
Añadimos 2 ficheros: 
* README.md 
* LICENSE.md

El contenido de los mismos lo tenemos que replicar de otros proyectos
En README.md colocare el guion del ejercicion
En LICENSE.md la licencia con que queremos compartir el proyecto. Busco ejemplos y me encuentro con http://choosealicense.com/ y escojo una licencia del MIT

Para comprobar que ficheros no estan en el control de versiones 
 $ git status
 On branch master
 Your branch is up-to-date with 'origin/master'.
 Untracked files:
  (use "git add <file>..." to include in what will be committed)

	.README.md.swp
	LICENSE.md
	README.md

 nothing added to commit but untracked files present (use "git add" to track)

Veo que puedo/debo añadir los 2 ficheros md al proyecto y que puedo ignorar los ficheros ocultos con extension .swp , asi que lo añado el patron a .gitignore

Para añadir los ficheros tengo varias opciones
 $ git add .
 $ git add README.md; git LICENSE.md

Tras comprobar veo que se han añadido los ficheros y he modificaco el .gitignore

Ahora ya puedo hacer commit 
 $ git commit -m "P2P Obligatorio Modulo 5"
 
y subir el proyecto al repositorio remoto de  github
 $ git remote add JordiRoman https://github.com/JordiRoman/random


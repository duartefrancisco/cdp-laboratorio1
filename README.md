# cdp-laboratorio1
Laboratorio #1 - Ciencia De Datos En Python - Universidad Galileo

# Git

Es un sistema de control de versiones multiplataforma, es de código abierto desarrollado inicialmente por Linus Torvalds, cuenta un arquitectura distribuida, esto lo convierte en un sistema de control de versiones distribuido. Permitiendo que cada persona involucrada en el proyecto cuenta un repositorio que alberga los cambios realizados.

## Estados
Git lleva control usando de los siguientes estados:

 - Committed: significa que los datos están almacenados en la base de datos local de git
 - Modified: significa que se ha modificado el archivo pero todavía no lo esta siendo seguido (trackeado) por git.
 - Staged: significa que se ha marcado un archivo modificado en su versión actual para que vaya en una próxima confirmación(commit) y sea seguido(trajeado).

# Comandos

### git init / git init `<directorio>`
Inicializa un nuevo repositorio

Si ya estamos en el directorio del proyecto:

    git init

En un directorio especifico:

    git init /users/pcname/proyecto

### git status
Conocer el estado del repositorio.

    git status

### git add
Para agregar los archivos al stage y sea tracked por git.
agrega un archivo especifico:
    git add <nombrearchivo>
  agrega todos los archivo:
  

    git adde .

### git commit
Para confirmar los cambios y establecerlos como una nueva versión.

    git commint -m "mensaje del commit"

### git brach
Lista las ramas del repositorio

Lista las ramas locales:

    git branch
Lista las ramas locales y remotas:

    git branch -a
elimina una rama:

    git branch -d <nombrerama>
   ### git checkout
   realizar cambios entre ramas.

Crea una nueva rama:

    git checkout -b <nombrerama>
  Cambio de rama:


    git checkout <nombrerama>
### git merge
Fusiona las ramas, los cambios de la rama actual los fusiona(lleva) a la rama solicitada.

    git merge <nombrerama>
### git clone
Clona un repositorio existente.

Clona un repositorio local:

    git clone /users/username/proyecto
   clonar un repositorio remoto:
   

    git clone username@host:/username/proyecto
    git clone https://username@github.com/username/repositorio
### git remote
Agrega/sincroniza/conecta un repositorio remoto.

    git remote add origin <servidor>

### git push
 Envía los datos  al servidor remoto.
 

    git push origin master
### git pull
 Obtiene la versión actual del servidor remoto
 

    git pull <serividor>
## git ignore
Sirve para agregar todos aquellos archivos que git debe ignorar, básicamente que no debe darle seguimiento.
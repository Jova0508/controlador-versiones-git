# Guía de Comandos de Git

## Comandos 

### Introducción al control de versiones: Comandos Básicos

- `git`: Se utiliza para obtener la lista de comandos disponibles en git.

- `git config --global user.name "Nombre"`: Se utiliza para configurar el nombre de usuario a nivel global en Git.

- `git config --global user.email "correo@ejemplo.com"`: Se utiliza para configurar tu dirección de correo electrónico a nivel global en Git.

- `git config --list`: Se utiliza para listar la configuración de Git.

- `cd [Carpeta]`: Se utiliza para cambiar el directorio de trabajo en una terminal.

- `dir`: Se utiliza para listar de archivos y carpetas en el directorio actual.

- `mkdir [Nombre del repositorio]`: Crea un nuevo directorio.

- `git init`: Inicializa un nuevo repositorio de Git en un directorio vacío.

- `code .`: Abre Visual Studio Code.

- `git status`: Verifica el estado de tu repositorio local.

- `git add [Nombre del archivo]`: Agrega archivos o cambios específicos.

- `git commit -m "Mensaje del commit"`: Crea un nuevo commit (punto de control).

- `git log`: Muestra el historial de commits.

- `git diff`: Muestra las diferencias entre el directorio de trabajo actual y el inicial.

- `git add .`: Agrega todos los archivos modificados.

- `HEAD`: Puntero de Git para especificar branch/commit actual.

### Trabajo en equipo con Git: Ramas en profundidad: creación, fusión y resolución de conflictos

- `git branch`: Muestra la lista de ramas en el repositorio.

- `git checkout -b [Asignar-responsable-a-rama/nombre-de-actividad]`: Crea una nueva rama y cambia a ella en un solo paso.

- `git checkout [Nombre de rama o commit]`: Cambia entre ramas o commits.

- `git merge [Nombre de rama/Nombre de actividad]`: Combina una rama en la rama en la que te encuentras actualmente.

### Trabajo en equipo con Git: Etiquetas y versionado semántico

- `git tag [0.0.1]`: Crea etiquetas para marcar versiones en la posicion del HEAD.

- `git tag -d [nombre]`: se utiliza para eliminar una etiqueta tag específica.

### Trabajo en equipo con Git: Gitignore y gestión de archivos binarios y sensibles

- `.gitignore`: Archivo de configuración para especificar qué archivos o directorios deben ser ignorados.

### Trabajo en equipo con Git: Hooks de Git y automatización de tareas

- `git commit -m "Mensaje del commit" -n`: Ignora el precommit.

La carpeta `.git/hooks` contiene scripts que te permiten personalizar respuestas a eventos específicos en tu flujo de trabajo de Git.

## Git Avanzado Git Rebase

- `git rebase [branch]`: Se utiliza para reorganizar la historia de la rama actual (actualizar) .

- `git rebase -i [id commit]`: Permite realizar un rebase interactivo a partir de un commit específico.

- `git rebase -i HEAD~n`: Permite realizar un rebase interactivo para los últimos n commits de la rama actual.

### Palabras clave comunes en el Rebase Interactivo

- `Pick (p)`: Conserva un commit tal como está en la historia.

- `Reword (r)`: Indica que se desea editar el mensaje del commit.

- `Squash (s)`: Se integra hacia arriba pero mantiene el mensaje del commit.

- `Fixup (f)`: Se integra hacia arriba pero se pierde toda referencia.

## Git Avanzado Git Stash

- `git stash`: Se utiliza para guardar temporalmente cambios que se han realizado en el directorio de trabajo.

- `git stash list`: Se utiliza para ver una lista de todos los stashes guardados en el repositorio.

- `git stash pop`: Trae el stash más reciente y lo borra de la pila.

- `git stash apply stash@{n}`: Trae un stash específico pero no lo borra de la pila.

- `git stash pop stash@{n}`: Trae un stash específico y lo borra de la pila.

## Git Avanzado Recuperación de Cambios Eliminados: Cherry-pick y Revert

- `git cherry-pick [id commit]`: Permite seleccionar un commit y aplicarlo en otra rama directamente. 

- `git revert [id commit]`: Deshace los cambios introducidos por el commit especificado, creando un nuevo commit que revierte los cambios. 

## Git Avanzado Referencias Remotas: Origin, Upstream, Fetch y Pull

- `Origin`: Hace referencia al repositorio remoto desde el cual se clonó el proyecto.

- `Upstream`: Se refiere al repositorio remoto del cual se realizó un fork (bifurcación) de un proyecto. 

- `Fetch`: Recupera los cambios desde el repositorio remoto, pero no los fusiona en tu rama local. 

- `Pull`: Recupera y fusiona los cambios desde el repositorio remoto en tu rama local.

## Git Avanzado Otros Comandos

- `git show`: Se utiliza para mostrar información detallada sobre un commit específico, incluyendo los cambios realizados.

- `git checkout -- .`: Descarta todos los cambios en tu directorio de trabajo.

# Comandos de GitHub

- `git clone [url]`: Clona un proyecto desde una URL remota a la computadora.

- `git remote -v`: Verifica la configuración de los repositorios remotos asociados con tu proyecto en la nube.

- `git branch -M main`: Cambia el nombre de la rama "master" a "main".

- `git push -u origin main`: Se utiliza para empujar la rama local "main" a un repositorio remoto llamado "origin" y establecer una relación de seguimiento.

- `git push`: Agrega los cambios realizados en tu repositorio local a la nube.


Este README proporciona una introducción a comandos y conceptos esenciales de Git. 

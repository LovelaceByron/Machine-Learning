# Machine-Learning
Respositorio de trabajo del equipo iART de la asignatura Trabajo en Equipo en Red de la UOC.

## Primeros pasos
### Registro y Fork
Cada miembro del equipo debe crearse una cuenta en github y hacer Fork de este repositorio (Botón en la esquina superior derecha).
### Pull Request
Actividad: Una vez que tenemos el repositorio _forkeado_, hacemos una modificación en algún archivo y procedemos a hacer ***Pull Request***.

## Trabajando desde local
### Instalar aplicación Github
1. Descargar la aplicación de escritorio de Github: https://desktop.github.com/
2. Instalar la aplicación
3. Hacemos login en la aplicación y seleccionamos la opción: "Clone", nos aparecerá nuestro repositorio y sólo tendremos que seleccionar en qué carpeta del disco duro instalarlo.

### Usando Visual Studio Code
_Nota: Se puede usar cualquier otro editor, pero si estáis acostumbrados a otro, tipo Sublime Text, Atom, etc. y no habéis probado éste... Probadlo ;-)_
1. Descargarse el Visual Studio Code (En adelante: Code): https://code.visualstudio.com/
2. Instalar Git: https://git-scm.com/. Durante la instalación, seleccionar:
  - Use Visual Studio Code as Git's default editor
  El resto de las opciones, dejar las que vienen por defecto.
3. Abrir Code y añadir la carpeta local: File -> Add Folder to Workspace.
4. A la izquierda hay un menú con iconos. Debajo de la lupa está el icono de "Source Control". Al hacer clic, se abre automáticamente.
5. Actividad: Crear o modificar algún archivo y hacer commit desde Code: Escribir un mensaje descriptivo de los cambios realizados y presionar Ctrl+Enter.

## Flujo de trabajo
_Falta depurar el flujo de trabajo, que lo haremos a base de práctica_
Una vez que tenemos nuestro repositorio local y nuestro repositorio remoto, trabajaremos de la siguiente forma:
1. Descargarse el proyecto actualizado
  'git pull'
2. Guardar nuestros cambios
  'git commit -m "Descripción de los cambios"'
3. Subir nuestros cambios
  'git push'

Con eso habremos actualizado nuestro repositorio remoto, pero faltará integrar los cambios en el repositorio oficial, para lo cual, haremos un "pull request".

## Pull Request desde Code
Instalar la extensión: https://marketplace.visualstudio.com/items?itemName=GitHub.vscode-pull-request-github

## Markdown en Code
Instalar las extensiones:
- https://marketplace.visualstudio.com/items?itemName=yzhang.markdown-all-in-one
- https://marketplace.visualstudio.com/items?itemName=hnw.vscode-auto-open-markdown-preview

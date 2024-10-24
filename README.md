# Curso de GIT
---
### Alcances de los repositorios
* system
* global
* local
---
### Configuraciones Iniciales
Nombre de usuario del dueño del repo
```git
git config --global user.name "<USERNAME>"
```
Email vinculado a una cuenta existente de GitHub
```git
git config --global user.email "<USEREMAIL>"
```
Mostrar configuraciones
```
git config --list
git config local --list
git config global --list
```
Vincular editor de codigo
```
git config --global core.editor "code --wait"
```
Resaltar entradas relacionadas con git

`git config --global color.ui true`

Configurar el auto carriage return
```git
git config --global core.autocrlf true  #Windows
git config --global core.autocrlf input #LInux, Mac, Unix
```
---
### Áreas de GIT
![GitAreas](img/GitAreas.png "GIT")
---
### Comandos Básicos
```HTML
<!-- Visualizar estado de los archivos que conforman al respositorio -->
git status
<!-- Agregar archivos al área de staging uno por uno o todos -->
 git add <NOMBREARCHIVO> || git add . 
<!-- Eliminar un elemento del área de staging -->
 git rm --cached <NOMBREARCHIVO>
 gti rm --cached -f <NOMBREELEMENTO> 
<!-- Hacer un commit -->
 git commit -m "<MENSAJE>"
 git commit 
```
---
### RESTORE, CHECKOUT Y MÁS
---
#### restore
Recupera un archivo que este presente en el area de staging pero ya no en el working directory

`git restore <NOMBREARCHIVO>`
#### checkout
Deshace los cambios realizados a un archivo en el working directory a una versión que toma como referencia el último commit

`git checkout <NOMBREARCHIVO`
#### restore
Deshace los cambios presentes en el área de staging y en el working directory para remplazarlos por el último commit registrado

`git reset --hard`
#### rename
Modifica el nombre de un archivo

`git mv <NOMBREARCHIVOORIGINAL> <NOMBREARCHIVONUEVO>`

#### short
Salida del comando `git status` más simplificada

`git status -s || git status --short`

Revisado por Edwin David 

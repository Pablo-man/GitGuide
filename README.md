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
* Workspace
* Staging Area
* Reposity
---
### Comandos Básicos
```HTML
<!-- Visualizar estado de los archivos que conforman al respositorio -->
git status
<!-- Agregar archivos al área de staging uno por uno o todos -->
 git add <NOMBREARCHIVO> || git add . 
<!-- Eliminar un elemento del área de staging -->
 git rm --cached <NOMBREARCHIVO>
```


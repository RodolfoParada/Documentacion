# GitHub
- [Volver al Inicio](../README.md)

Libro digital https://git-scm.com/book/en/v2

### **Instrucciones Git**

***Obtener últimos cambios de repositorio***
```Github
git pull
```
**Crear y moverse a una nueva rama**
```Github
git checkout -b nombre-rama
```
**Ver cambios en archivos**
```Github
git status
```
**Agrega cambios e Ignora archivo para no subirlo .env**
```Github
git add . :!.env
```
**Agrega Todos los cambios**
```Github
git add .
```
**Crear commit con mensaje**
```Github
git commit -m “convetional : mensaje ”
```
**Subir cambios a rama creada**
```Github
git push origin nombre-rama
```
**Cambiarse a rama develop**
```Github
git checkout develop
```
**Mezclar rama develop con nueva rama (nombre de la rama que se va a unir a develop)**
```Github
git merge --no-ff nombre-rama
```
**Subir rama develop con cambios meclado**
```Github
git push
```

### **Otros comandos Git**

**Muestra el historial de commits en la rama actual, incluidos sus hash (los id de cada commit) y sus tags.**
```Github
git log
```
**Crea la carpeta .git/ para iniciar el repositorio**
```Github
git init
```
**Te permite hacer configuraciones a git.**
```Github
git confing
```
**Listar ramas locales**
```Github
git branch
```
**Listar ramas remotas**
```Github
git branch -r
```
**Listar todas las ramas (locales y remotas)**
```Github
git branch -r
```
**Listar archivos en el repositorio**
```Github
git ls-files
```
**Listar cambios entre commits o ramas**
```Github
git diff
```




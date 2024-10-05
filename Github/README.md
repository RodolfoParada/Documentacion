# GitHub
- [Volver al Inicio](../README.md)
- [Instrucciones Git](#instrucciones-git)
  - [Obtener últimos cambios de repositorio](#obtener-últimos-cambios-de-repositorio)
  - [Crear y moverse a una nueva rama](#crear-y-moverse-a-una-nueva-rama)
  - [Ver cambios en archivos](#ver-cambios-en-archivos)
  - [Agregar cambios e ignorar archivo .env](#agregar-cambios-e-ignorar-archivo-env)
  - [Crear commit con mensaje](#crear-commit-con-mensaje)
  - [Subir cambios a rama creada](#subir-cambios-a-rama-creada)
  - [Cambiarse a rama develop](#cambiarse-a-rama-develop)
  - [Mezclar rama develop con nueva rama](#mezclar-rama-develop-con-nueva-rama)
  - [Subir rama develop con cambios mezclados](#subir-rama-develop-con-cambios-mezclados)
- [Otros comandos Git](#otros-comandos-git)
  - [Ver historial de commits](#ver-historial-de-commits)
  - [Iniciar repositorio](#iniciar-repositorio)
  - [Configuraciones de Git](#configuraciones-de-git)
  - [Listar ramas locales](#listar-ramas-locales)
  - [Listar ramas remotas](#listar-ramas-remotas)
  - [Listar todas las ramas](#listar-todas-las-ramas)
  - [Listar archivos en el repositorio](#listar-archivos-en-el-repositorio)
  - [Listar cambios entre commits o ramas](#listar-cambios-entre-commits-o-ramas)

Libro digital https://git-scm.com/book/en/v2

### **Instrucciones Git**

**Obtener últimos cambios de repositorio**
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




# GitHub
- [Volver al Inicio](../README.md)
- [Instrucciones Git](#instrucciones-git)
- [Otros comandos Git](#otros-comandos-git)
 
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

### Subir Un Proyecto Local a GitHub
**Inicializar el proyecto local para ser subido a GitHub**
```Github
git init
```
git add .
**Se agrega el proyecto para ser subido a GitHub**
```Github
git add .
```
**Agregar primer commit**
```Github
git commit -m "first commit"
```

**Se conecta con el repositorio en GitHub**
```Github
git remote add origin https://github.com/NOMBRE_USUARIO/NOMBRE_PROYECTO.git
```
**Se sube el proyecto local a GitHub**
```Github
git push -u origin master
```

### Subir Un Proyecto Local al Github de Amorfia
**Inicializar el proyecto local para ser subido a GitHub**
```Github
git init
```
git add .
**Se agrega el proyecto para ser subido a GitHub**
```Github
git add .
```
**Agregar primer commit**
```Github
git commit -m "first commit"
```

**Se conecta con el repositorio en GitHub**
```Github
git remote set-url origin git@github-secundario:Rodolfotech/repo2.git
```
**Se sube el proyecto local a GitHub**
```Github
git push -u origin master
```

### Subir Un Proyecto Local al Github de Amorfia
**Clonar proyectos desde Github de Amorfia**
```Github
git clone git@github-secundario:Rodolfotech/nombre-repo.git
```
### Como hacer deploy en github 



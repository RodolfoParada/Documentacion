# GitHub
- [Volver al Inicio](../README.md)

Libro digital

https://git-scm.com/book/en/v2

### **Git Instruction**



**Obtener últimos cambios de repositorio**
```Github
git pull
 
```



**git pull**

Crear y moverse a nueva rama

**git checkout -b nombre-rama**

Ver cambios en archivos

**git status**

Agreaga cambios e Ignorar archivo para no subirlo 

- el archivo ignorado es .env

**git add . :!.env**

Agregar Todos los cambios

**git add .**

Crear commit con mensaje

**git commit -m “convetional : mensaje ”**

Subir cambios a rama creada 

**git push origin nombre-rama**

Cambiarse a rama develop

**git checkout develop**

Mezclar rama develop con nueva rama (Nombre de la rama que se va a unir a develop)

git merge --no-ff nombre-rama

 Subir rama develop con cambios mezclados  

git push

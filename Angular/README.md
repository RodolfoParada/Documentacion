# Angular 18
- [Volver al Inicio](../README.md)

### Instalar angular 
**Para crear un proyecto en Angular**
```
npm install -g @angular/cli
```

### Se debe crear un una carpeta antes para crear un proyecto en angula 
**Para crear un proyecto en Angular**
```
ng new nombre-de-proyecto
```
**Para levantar el proyecto angular en el navegador**
```
ng serve -o
```
**Para generar un nuevo componente sin el test**
```version larga 
ng generate component nombre-componente --skip-test
```
```version corta
ng g c nombre-componente --skip-test
```
**Crear componente inline**
```
ng g c nombre-componente --inline-template --inline-style --skip-tests
```
**Instalar bootstrap en Angular**
```
npm install bootstrap@latest --save
```
**Instalar libreria poppers**
```
npm i @popperjs/core --save
```

**Para crear un proyecto compatible con versiones anteriores**
```esta aplicación es de modulos anterir a la version 18
ng new nombre-proyecto --stalone=false
```
**Para crear un servicio**
```esta aplicación es de modulos anterir a la version 18
ng g s nombreComponente --skip-tests
```

**Crear un proyeto standalone**
```para versiones anteriores
ng new  mi-primera-app --standalone=false
```

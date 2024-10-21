# Angular
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
**Para crear un proyecto compatible con versiones anteriores**
```esta aplicación es de modulos anterir a la version 18
ng new nombre-proyecto --stalone=false
```

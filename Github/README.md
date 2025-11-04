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

### Clonar Proyectos del Github de Amorfia
**Clonar proyectos desde Github de Amorfia**
```Github
git clone git@github-secundario:Rodolfotech/nombre-repo.git
```
__________________________________________________________________________________________________________________-
### Simular un "rollback" a la versión anterior"
```Github
git checkout HEAD~1
cat app.js  # Vemos la versión anterio
```
### Volvemos a la versión actual"
```Github
git checkout master
cat app.js  # Vemos la versión completa
```
_________________________________________________________________________________
| **1. Convención**        |
| **Elemento** | **Descripción / Ejemplo** |
|---------------|----------------------------|
| **Importancia de los mensajes de commit** | Los mensajes de commit son una parte esencial del historial de un proyecto. Una buena convención facilita la revisión del código, la comprensión de los cambios y la generación automática de registros de cambios (*changelogs*). |
| **1. Uso Imperativo en el Asunto (Subject)** | El asunto o primera línea del mensaje debe utilizar el modo imperativo. Esto significa que debe sonar como una orden o instrucción. |
| **Regla** | El mensaje debe completar la frase imaginaria: “Si se aplica este commit, este commit hace/hará...” |
| **Mal Ejemplo (No Imperativo)** | Arreglando el error de autenticación<br>Añadida la nueva característica X<br>Actualiza la documentación de instalación |
| **Buen Ejemplo (Imperativo)** | Arreglar error de autenticación<br>Añadir característica X<br>Actualizar documentación de instalación |

________________________________________________________________________________
| **2. Prefijo (Type)** | **Propósito del Cambio** | **Ejemplo** |
|---------------------|---------------------------|-------------|
| feat: | Una nueva característica. | `feat: Añadir formulario de contacto` |
| fix: | Una corrección de un error (bug). | `fix: Corregir fallo de login en Safari` |
| docs: | Cambios solo en la documentación. | `docs: Actualizar guía de contribución` |
| style: | Cambios que no afectan la lógica del código (formato, comas, etc.). | `style: Formatear código con Prettier` |
| refactor: | Un cambio de código que no añade funcionalidad ni arregla errores. | `refactor: Simplificar la función de usuario` |
| test: | Añadir o corregir pruebas unitarias o de integración. | `test: Añadir pruebas para servicio de pago` |
| chore: | Tareas de mantenimiento (builds, dependencias, etc.). | `chore: Actualizar versión de dependencias` |

________________________________________________________________________________
| **3. Claridad**        |
| **Elemento** | **Descripción** | **Ejemplo** |
|---------------|----------------|--------------|
| **Asunto (Subject Line)** | Debe ser conciso y describir **qué hace el cambio**. | `feat: Implementar cache para rutas estáticas` |
| **Cuerpo (Body)** | Explica **por qué y cómo** se realizó el cambio. Es opcional, pero recomendable cuando el cambio no es trivial. | ```Implementar cache para rutas estáticas

La implementación de la cache reduce significativamente el tiempo
de respuesta de las rutas que no cambian con frecuencia. Se usó
Redis para almacenar los resultados del `fetch` inicial,
expirando cada 5 minutos para asegurar cierta frescura.

Esto resuelve el problema de rendimiento reportado en el ticket #40.``` |
| **Formato general** | `[tipo](ámbito opcional): [descripción concisa en imperativo]` | `feat(rutas): Implementar cache para rutas estáticas` |
| **Regla adicional** | Separar el asunto, cuerpo y pie con **una línea en blanco**. | *(Ver ejemplo completo más abajo)* |

_______________________________________________________________________________
| **4. Longitud**        |
| **Parte** | **Límite recomendado** | **Motivo / Beneficio** |
|------------|------------------------|--------------------------|
| **Asunto (Subject Line)** | Máximo **50 caracteres** | Permite que el mensaje se muestre completo en GitHub, Git log, y otras herramientas. |
| **Cuerpo (Body)** | Máximo **72 caracteres por línea** | Mejora la legibilidad en la terminal y mantiene un formato estándar. |
| **Espaciado** | Dejar una **línea en blanco** entre el asunto y el cuerpo. | Facilita la separación visual entre las secciones. |
| **Estructura completa recomendada** | ```<tipo>(<ámbito opcional>): <descripción concisa en imperativo> (50 caracteres)

<cuerpo opcional con más detalles de por qué/cómo> (72 caracteres por línea)

<pie opcional para referencias de tickets o Breaking Changes>``` | Estandariza todos los commits y permite generar changelogs automáticamente. |



### Como hacer deploy en github 






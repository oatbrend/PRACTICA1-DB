# CONTROL DE VERSIONES CON GIT Y GITHUB

## VERSION CONTROL SYSTEM Y TRABAJO EN EQUIPO

Los sistemas de control de versiones (o VCS, por sus siglas en inglés: Version Control System) son herramientas de software diseñadas para gestionar y registrar los cambios realizados en un conjunto de archivos, como el código fuente de un proyecto[cite: 1].

Gracias a los VCS, los equipos de desarrollo pueden colaborar de forma rápida y eficiente mientras preservan la integridad del código[cite: 1]. Esto permite a los programadores trabajar simultáneamente con la tranquilidad de que los conflictos de edición se gestionan de manera segura[cite: 1].

Al operar a nivel del sistema de archivos, un VCS rastrea continuamente la adición, modificación o eliminación de archivos y directorios[cite: 1]. Para mantener la integridad del proyecto, las actualizaciones individuales se guardan periódicamente en registros de cambios llamados confirmaciones (commits)[cite: 1]. Posteriormente, estos cambios se fusionan de manera segura con el código fuente principal, garantizando un historial completo, una copia de seguridad constante y una gestión de conflictos transparente para todo el equipo[cite: 1].

En la actualidad, los VCS son indispensables para mantener flujos de trabajo eficientes, ya que constituyen la única “fuente de verdad” para el equipo[cite: 1]. Actúan como una red de seguridad vital, evitan que la pérdida accidental o la modificación incorrecta de un archivo local ponga en riesgo todo el proyecto y permiten que cada desarrollador contribuya a la base de código de forma independiente y segura[cite: 1].

---

## GIT Y GITHUB

Git y GitHub no son lo mismo[cite: 1]. La diferencia principal es que Git es un sistema de control de versiones que se ejecuta de forma local para rastrear los cambios en archivos, mientras que GitHub es una plataforma en la nube que aloja esos proyectos de Git para facilitar el respaldo y el trabajo colaborativo[cite: 1].

Por un lado, Git nació para tomar el espacio de otros sistemas de control, siendo su principal creador Linus Torvalds (el mismo creador de Linux)[cite: 1]. A diferencia de la mayoría de los VCS tradicionales, Git almacena cada versión guardada como una ‘instantánea’ en lugar de una lista de cambios archivo por archivo[cite: 1]. Esto te permite trabajar en tu propia copia local, registrar el historial, consultar instantáneas antiguas cuando lo necesites y crear nuevas cada vez que modificas el proyecto[cite: 1].

Por otro lado, GitHub se basa en Git alojando esos proyectos (denominados repositorios) en la nube[cite: 1]. Además, añade herramientas visuales, de planeación y de revisión de código que facilitan a los equipos combinar su trabajo y colaborar de forma segura desde cualquier lugar[cite: 1].

---

## DEFINICIONES CON EJEMPLO

### Repositorio
Repositorio es la carpeta donde se almacenan todos los archivos de un proyecto, junto con el historial de cambios desde el inicio[cite: 1].

**Ejemplo:**  
Repositorio para todas las tareas de la materia base de datos[cite: 1].  
`“ Tareas-BD-27-1 ”`[cite: 1]

### Confirmacion (Commit)
Commit es cada acción de guardar una modificación del archivo y que puede ser etiquetado con un mensaje que señala el cambio efectuado[cite: 1].

**Ejemplo:**  
Commit del cambio del archivo que contiene la tarea 1 de base de datos[cite: 1].  
`“ 📄Tarea1-InstalacionSGBD.pdf    Agrega imágenes finales  yesterday”`[cite: 1]

### Rama (Branch)
Las ramas son las distintas líneas de trabajo que un proyecto puede tener sin alterar de manera directa la ruta principal de trabajo[cite: 1].

**Ejemplo:**  
Rama principal  
`“main”`[cite: 1]  
Rama secundaria  
`“propuestas de mejora”`[cite: 1]

### Fusión (merge)
Una fusión es el proceso de unir todos los cambios de una rama, dentro de otra[cite: 1].

**Ejemplo:**  
Rama secundaria $\rightarrow$ merge $\rightarrow$ Rama principal[cite: 1]  
`“propuestas de mejora”  → merge →  “main”`[cite: 1]

### Conflicto de fusión
Ocurre cuando un cambio se realiza en la misma ubicación por dos ramas distintas al mismo tiempo, en este caso Git no puede decidir qué modificación conservar[cite: 1]. Se resuelve manualmente para elegir la versión correcta[cite: 1].

**Ejemplo:**  
Línea original (main):  
`“Título: El camino a la casa verde “`[cite: 1]

| Rama 1 | Rama 2 |
| :--- | :--- |
| `“Título: El camino a la casa azul”`[cite: 1] | `“Título: El camino a la casa rosa”`[cite: 1] |

### Pull Request
Es la petición que se realiza al equipo (en Github) cuando se ha concluido con los cambios en una rama y se desea revisión antes de una fusión con otra[cite: 1].

**Ejemplo:**  
Base(destino) $\leftarrow$ Compare (origen)[cite: 1]  
Base(main) $\leftarrow$ Compare (imagenes-extras)[cite: 1]  

**Título:**  
Agrega imágenes extra a la Practica1[cite: 1]  

**Descripción:**  
Equipo en este Pull Request se implementa:[cite: 1]
- Todas las imágenes faltantes en formato PNG[cite: 1].
- Pie de foto para cada uno de los agregados[cite: 1].

Se pide revisión para su posterior adición (merge) a la rama principal[cite: 1].

### Archivo .gitignore
El archivo `.gitignore`, sirve para indicarle a Github qué archivos o carpetas no debe rastrear y mejor ignorar[cite: 1].

**Ejemplo:**  
Archivo $\rightarrow$ `.gitignore`[cite: 1]  
Dentro $\rightarrow$ `contraseñas-BaseDeDatos.txt`[cite: 1]

### Archivo READ ME
Es el archivo de presentación de cada repositorio, en este se agrega todo el texto que explique el proyecto, depende del contenido del repositorio, vienen diversas indicaciones en este archivo READ ME[cite: 1].

**Ejemplo:**  
```markdown
# Brenda Roa Venegas
# Número de boleta
# Inteligencia Artificial
** Índice del contenido completo de la Práctica 1
```[cite: 1]

---

## FLUJO DE TRABAJO EN RAMAS Y REVISIÓN PREVIO A FUSIÓN
**(Feature Branch Workflow)**

El flujo de trabajo basado en ramas consiste en desarrollar nuevas funcionalidades, corregir errores o experimentar con ideas dentro de una línea de trabajo aislada en lugar de hacerlo sobre la línea principal[cite: 1]. Esto permite trabajar con total libertad sin alterar el código que ya está funcionando, protegiendo así la rama principal contra fallos por cambios accidentales[cite: 1].

Además de facilitar el desarrollo independiente, este flujo aprovecha las solicitudes de extracción (pull requests) para abrir un canal de revisión y debate sobre los cambios propuestos[cite: 1]. De esta manera, el código se revisa entre pares antes de fusionarse, lo que brinda al equipo la oportunidad de validar la solución, detectar errores a tiempo, garantizar la calidad y mantener estándares compartidos en todo el proyecto[cite: 1].

---

## CUENTA EN GITHUB Y REPOSITORIO

**Dirección del repositorio:**  
https://github.com/oatbrend/PRACTICA1-DB[cite: 1]

<!-- Las capturas de pantalla de la salida de "git log --oneline --graph --all" y del Pull Request fusionado se anexan en la carpeta evidencias -->

---

## REFERENCIAS

- Microsoft. (2025). *¿Qué es el control de versiones?* Microsoft Learn. https://learn.microsoft.com/es-es/devops/develop/git/what-is-version-control[cite: 1]
- Microsoft. (2025). *¿Qué es Git?* Microsoft Learn. https://learn.microsoft.com/es-es/devops/develop/git/what-is-git[cite: 1]
- Unity. *Sistema de control de versiones*. Glosario de Unity. http://unity.com/es/glossary/version-control[cite: 1]
- Atlassian. *Software de control de versiones*. Bitbucket. https://bitbucket.org/product/es/version-control-software[cite: 1]
- Silveira, P. (2021). *Git y GitHub: Qué son y primeros pasos*. Blog de Alura Cursos. https://www.aluracursos.com/blog/git-y-github-que-son-y-primeros-pasos[cite: 1]
- Kinsta. (2025). *Git vs GitHub: ¿Cuál es la diferencia y cómo empezar?* Kinsta Blog. https://kinsta.com/es/blog/git-vs-github/[cite: 1]
- GitHub. *¿Qué es GitHub?* Documentación de GitHub. https://docs.github.com/es/get-started/start-your-journey/what-is-github[cite: 1]
- GitHub. *Acerca de las ramas*. Documentación de GitHub. https://docs.github.com/es/pull-requests/reference/branches[cite: 1]
- Atlassian. *Flujo de trabajo Feature Branch en Git*. Atlassian Git Tutorials. https://www.atlassian.com/git/tutorials/comparing-workflows/feature-branch-workflow[cite: 1]
- Mergify. (2025). *Feature branch workflow: A practical guide for Git*. Mergify Blog. https://mergify.com/blog/feature-branch-workflow-a-practical-guide-for-git[cite: 1]
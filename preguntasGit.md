# Preguntas sobre Git
## Preguntas Basicas

1. >¿Que es Git?
    - Git es una tecnlogia diseada para poder cambiar, restrear y guardar cambios en cualquier tipo de archivos de computadora. Normalmente las empresas utilizan Git para administrar y seguir el progresp de sus proyectos.
        ### LOGO DE GIT
        <img height="200px" width="400px" src="https://git-scm.com/images/logos/downloads/Git-Logo-1788C.png">
2. >¿Cuál es la diferencia entre un "repositorio simple" y un "directorio de trabajo"?
    - Repositorio Simple:
        - No cuenta con ningun archivo de trabajo que se use en Git y no hay ni subdirectorios ni control de versiones.
    - Directorio de trabajo:
        - Contiene todos los archivos, subdirectorios... 
3. >¿Cuál es la diferencia entre una "bifurcación" y una "rama"?
    - Bifurcacion:
        - Es una copia de un directorio que esta completamente separado
    - Rama:
        - Se usa para cambiar ciertas partes de un programa, para luego fusionar los cambios en el nucleo (main/master)
4. >Has creado una confirmación y la has enviado, ahora es pública. Sin embargo, has notado que todavía hay cosas que deben cambiarse. ¿Puedes hacerlo en la etapa de confirmación? y si es así, ¿Cómo?
    - Se pueden realizar cambios incluso despues de la confirmacion con el comando llamada ***git revert***.
    - Es un comando que actua como parche.
5. >¿Qué es "cherry-picking"?
    - Ocurre cuando decides elegir algún tipo de confirmación de una rama basada en Git y luego aplicar sus características a otra rama. 
6. >¿Qué es un "stash"?
    - El Stash actua como una unidad de almacenamiento, donde guardar tu proyecto y todas las caracteristicas, por lo que te deja regresar en el tiempo y continuar trabajando donde lo dejaste.
7. >¿Cómo resuelves "conflictos " en Git?
    - Hay varios conflictos pero uno de los mas normales es tener algun cambio duplicado, por ejemplo cambios en VisualCode y en Github a la vez. Por lo tanto emitira un conflicto por lo que hay que utilizar los comandos "git add" y "git commit" y despues juntarlos.
8. >¿Cuál es el lenguaje utilizado en Git?
    - Git utiliza el lenguaje "C"
    <br>
    <img height="200px" width="400px" src="https://i.blogs.es/21f7ba/c-lenguaje/1366_521.jpg">
   
9. >¿Qué es una "solicitud de extracción"?
    - Es cuando tomas un repositorio y despues creas tu propia rama. Despues hacemos cambios y lo juntamos con la rama principal.
10. >¿Cuál es la manera más eficiente de encontrar una mala confirmación?
    - Con el comando "git bisect"
## Preguntas Avanzadas
1. >¿Qué es un "encabezado"?
    - Un encabezado es utilizado para referirse al objeto de una confirmacion.
2. >¿Para qué se utiliza el comando "Git CONFIG"?
    -  Sirve para configurar la mayoria de opciones que necesitaras en Git. Ya sea informacion del usuario o la forma en la que funciona el repositorio.
3. >¿Se pueden arreglar las confirmaciones rotas?
    - Si, se puede hacer mediante el comando git commit - amend.
        - Encuentra la confirmacion rota y restaura su funcionalidad.
4. >¿Cuál es la diferencia entre "obtener" y "extraer"?
    - **Extraer**: Cuando **_extraes_** datos, los mismos se descargan y luego se combinan inmediatamente con sus archivos de trabajo actuales.
    - **Obtener**: **_Obtener_** datos es el camino a seguir si deseas descargarlos, pero sin fusionar los archivos.

# LAS 10 PREGUNTAS/RESPUESTAS MAS INTERESANTES
## EN STACKOVERFLOW
1. >¿Cómo revertir un commit, si ya subí los cambios al origen?
    - Eliminar el ultimo commit es una opcion con el comando:
        - **git rebase -i HEAD~1**
        - Debes comentar la linea de código correspondiente al commit, guardar y salir del editor.
        - Y despues ejecutar
        - **git push -f origin master**
    - Otra opcion es ir a un commit anterior con la informacion deseada para subir.
        - Primero conseguimos los hash mediante **git log --oneline**
        - Y utilizamos este comando **git reset --hard (hash)**
2. > ¿Cómo modificar el mensaje de un commit en particular?
    - Con el comando:
    - git commit --amend -m "your new message"
3. > ¿Cuál es la diferencia entre 'git rebase' y 'git merge'?
    - **git-rebase** – Genera una serie de commits secuencialmente, de modo que puedan aplicarse directamente sobre la cabeza del nodo.
    - **git-merge** – Une dos o más historiales de desarrollo
4. > ¿Cómo ver qué archivos son diferentes entre 2 ramas con Git?
    - Con el comando:
    - **git diff branch1..branch2**
5. > ¿Cómo puedo deshacer el último commit en Git?
    - Si quieres mantener los cambios.
        - **git reset [--mixed] HEAD~1**
    - Si además no quieres cargarte el commit (sólo mover el head al anterior):
        - **git reset --soft HEAD~1**
    - Y si no quieres mantenerlos (y volver al estado del commit anterior, en la práctica, destruir el último commit completamente como si nunca hubiera existido):
        - **git reset --hard HEAD~1**
6. > ¿Cuál es la diferencia entre pull y fetch en git?
    - **git fetch** baja los cambios de la rama determinada y la coloca en una rama espejo que simplemente es una clase de rama escondida en la cual tú puedes mirar los cambios de dicha rama, para posteriormente hacer merge con tu rama local.
    - El **git pull** simplemente es un git fecth + git merge. No utilizar el git pull si en realidad está dudoso de qué cambios puedan traerse del repositorio remoto.
7. > Regresar un repositorio a un commit especifico
    - Para hacerlo hay que seguir estos pasos
        - **git log --oneline** = Con esto sacaremos los hash de los commit
        - **git checkout** (hash)
8. > ¿Para qué se usan los tags en Git?
    - Una etiqueta que te ayuda a encontrar algo que estas buscando.
9. > ¿Cómo ignorar los cambios de permisos en git (chmod)?
    - **% git config core.fileMode false**
10. > Diferencias en comandos de git add
    - Sirven para indicar que se va a anexar cualquier archivo al stage, desde ese punto estos archivos y sus cambios serán monitoreados
        - **git add . , git add -A  y git add --all**
    - Te enseñara que cambios estan siendo rastreados y cuales no.
        - **git add --help**
    - Esta opción puede ser usada para separar opciones de línea de comando de la lista de archivos, útil cuando los nombres de los archivos se pueden confundir con las opciones de línea de comandos.
       - **git add —** 

11. >Configurar name y email en git
    - Con el comando **git config --list --show-origin**
        - Obtienes la ruta de tu archivo .gitconfig
        - Y agregas esto
            - [user] 
            - name = Tu nombre 
            - email = Tu email
        - Luego ejecutas **git config --list** y te saldran los datos introducidos.

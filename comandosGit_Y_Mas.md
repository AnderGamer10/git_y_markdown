# LOS COMANDOS SOBRE GIT Y GITHUB
1. >GIT:
    - git version
    - git init: para inicializar git
    - git status -s: para saber que archivos no tienen seguimientos

    - git add . : añadimos todos los archivos al área temporal. Si quieres añadir solo un archivo quitamos el “.” y añadimos el nombre del archivo.

    - git commit -m “el mensaje”: para mandarlo al siguiente nivel y guardar su momento exacto (como una foto) con un mensaje.

    - git log --oneline : sirve para ver los identificadores de los commit

    - git reset --hard (identificador) : sirve para viajar a ese archivo guardado según su identificador pero borra los que están por encima.

    - git checkout (identificador) = Lo mismo que el de arriba pero no borra ningún commit

    - git reset --soft (identificador): Lo mismo que el de arriba pero no borra ningún commit y todo lo que se haga se quedará en contenido local.

    - git reset --soft master = te lleva al commit master

    - git reset --mixed (identificador): Todo lo que se añada no se pondrá en commits futuros.

    - git push : sirve para subir a github archivos
    
    - >Maneras de añadir un repositorio:
        - git remote add origin https://github.com/AnderGamer10/git_y_markdown.git  = esto sirve para añadir el repositorio donde guardar los archivos en github.

        - git remote add origin git@github.com/AnderGamer10/git-ejemplo.git  = lo mismo que el de arriba pero version SSH

    - git commit --amend -m “nuevo mensaje” = sirve para cambiar el nombre del ultimo commit

    - git clone https://github.com/AnderGamer10/git_y_markdown.git =Para clonar el repositorio en otro pc

    - git checkout master: cambiar a la rama master.

    - git merge dev: juntar el contenido de las ramas.

    - git rebase : igual que el de arriba pero no sale que hay conflicto.

    - git log --oneline

    - git branch DEV : para crear una rama.

    - git branch -a : para ver los branch que hay
    
2. CMD:
    - CD: Para ir a un directorio
    - DIR: Para ver que hay en el directorio
    - TREE: Enseña el arbol de directorios
    - RENAME ARCHIVO: Cambia el nombre del archivo
    - TYPE ARCHIVO.EXTENSION: Te permite crear un archivo desde la propia ventana de comandos.
    - echo holamundo < archivo.txt : Sirve para crear un archivo txt con el texto holamundo
    - COPY ARCHIVO DESTINO: Para hacer una copia de un archivo y guardarlo en un destino.     
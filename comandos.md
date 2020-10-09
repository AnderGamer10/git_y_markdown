# LOS COMANDOS SOBRE GIT Y GITHUB
1. GIT:
- git version
- git init: para inicializar git
- git status -s: para saber que archivos no tienen seguimientos

- git add . : añadimos todos los archivos al área temporal. Si quieres añadir solo un archivo quitamos el “.” y añadimos el nombre del archivo.

- git commit -m “el mensaje”: para mandarlo al siguiente nivel y guardar su momento exacto (como una foto) con un mensaje.

- git log --oneline : sirve para ver los identificadores de los commit

- git reset --hard (identificador) : sirve para viajar a ese archivo guardado según su identificador

- git push : sirve para subir a github archivos
dos maneras:
- git remote add origin https://github.com/AnderGamer10/git-ejemplo.git   
- git remote add origin git@github.com/AnderGamer10/git-ejemplo.git   
esto sirve para añadir el repositorio donde guardar los archivos en github.

2. GITHUB:
creamos un repositorio

- git clone https://github.com/AnderGamer10/git-ejemplo.git

git init -> Inicializa git en el proyecto, se crea una carpeta oculta .git //Working directory
git status -> permite ver los archivos que tenemos en el proyecto.
git add "el archivo que queremos subir".js -> Sube el archivo al stagging area, o lo actualia si ya existe.
git restore "el archivo".js -> Descarta los cambios realizados en el archivo.

Configuramos mi identidad en git mediante el uso de los siguientes comandos:
git config --global user.email "you@example.com" -> Si lo escribes mal vuelves a escribir el comando y no pasa nada.
git config --global user.name "Your Name" 

Y luego implementamos:
git commit -> Crear un primer punto de control del codigo, tomamos un snapshot


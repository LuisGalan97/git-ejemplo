git init -> Inicializa git en el proyecto, se crea una carpeta oculta .git //Working directory
git status -> permite ver los archivos que tenemos en el proyecto.
git add "el archivo que queremos subir".js -> Sube el archivo al stagging area, o lo actualia si ya existe.
git restore "el archivo".js -> Descarta los cambios realizados en el archivo.


Configuramos mi identidad en git mediante el uso de los siguientes comandos:
git config --global user.email "you@example.com" -> Si lo escribes mal vuelves a escribir el comando y no pasa nada.
git config --global user.name "Your Name" 

Y luego implementamos:
git commit -> Crear un primer punto de control del codigo, tomamos un snapshot
-----------------------Luego de crear el primer snapshot--------------------------
git status -> Sigue permitiendo ver si se han hecho modificaciones en el proyecto.
git log -> Revisamos los snapshots.
git checkout -- "archivo".js -> Restauramos el archivo a la version del snapshot.
git diff "archivo".js -> Revisamos las diferencias entre la version actual del archivo y el del snapshot.
                         Presionamos ENTER para avanzar, y la Q para salir.

git add "archivo".js-> Sigue guardando los cambios pero deberemos recurrir al git commit para subirlos como snapshot.
git commit -> Cargamos un nuevo snapshot, presionamos "i" para escribir un comentario arriba de todo,"esc", luego ":wq" para write and quit


//------------------------.gitignore-----------------
Esto no es un comando, es una texto plano donde podemos especificar en forma de directorio o path lo que queremos que se ignore de nuestro repositorio y no se tendra en cuenta con el gitstatus, y por ende no se cargara con los comandos.

//---- Si quiero commitear o usar el git commit sin tener que entrar a la consola, podemos---
git commit -m "el comentario que queremos añadir al snapshot"


git brach "nombre" -> creamos una version alternativa del proyecto en el database de git, si solo colocamos git branch veremos, el master, y las que tengamos.

git checkout "nombre" -> nos desplazamos de la rama master a la rama deseada.


git add . -> Añade todos los archivos dentro del entorno de trabajo o los actualiza. pd: git ignora las carpetas vacias
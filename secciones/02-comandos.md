# 2. Comandos esenciales de Git

Autor: Manuela Arce Elizondo

## 2.1 Las tres zonas

Cuando trabajamos con Git existen tres zonas principales por las que pasan nuestros archivos.
La primera es el directorio de trabajo, que es donde creamos, editamos o eliminamos los archivos normalmente.
La segunda es el área de preparación o staging, donde colocamos los cambios que queremos incluir en el próximo commit.
Para pasar un archivo a esta zona utilizamos el comando `git add`.
La tercera zona es el repositorio local, donde Git guarda los cambios que ya confirmamos mediante un commit.
El comando `git commit` permite registrar esos cambios y conservarlos dentro del historial del proyecto.
Estas tres zonas permiten revisar y organizar los cambios antes de guardarlos definitivamente en el historial.
## 2.2 Configuración inicial

Antes de comenzar a trabajar con Git es importante configurar nuestra identidad.
Git utiliza un nombre y un correo electrónico para identificar quién realizó cada commit.
El nombre se configura utilizando `git config --global user.name "Nombre Completo"`.
El correo se configura con `git config --global user.email "correo@ejemplo.com"`.
Es recomendable utilizar el mismo correo asociado a nuestra cuenta de GitHub.
De esta manera, los commits pueden quedar relacionados correctamente con nuestro perfil.
También podemos usar `git config --global --list` para revisar la configuración que tenemos guardada.
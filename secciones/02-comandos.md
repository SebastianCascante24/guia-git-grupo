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
## 2.3 El ciclo status, add, commit y push

El trabajo con Git sigue un ciclo que nos permite controlar los cambios que realizamos en un proyecto.
Primero usamos `git status` para revisar cuáles archivos fueron modificados y conocer su estado.
Después utilizamos `git add` para preparar los cambios que queremos incluir en el siguiente commit.
Con `git commit -m "mensaje"` registramos esos cambios en nuestro repositorio local y dejamos una descripción de lo realizado.
Luego utilizamos `git push origin main` para enviar nuestros commits al repositorio remoto en GitHub.
Si otro integrante subió cambios antes, puede ser necesario ejecutar `git pull origin main` antes de realizar el push.
Este ciclo ayuda a mantener un historial ordenado y permite que varias personas trabajen sobre un mismo proyecto.
## 2.4 Consultar el historial

Git también permite consultar el historial de los cambios que se han realizado en el proyecto.
El comando `git log` muestra información detallada de los commits registrados en el repositorio.
Si queremos una vista más sencilla podemos utilizar `git log --oneline`.
Este comando presenta cada commit en una sola línea, mostrando su identificador y el mensaje correspondiente.
También podemos usar `git log --pretty=format:"%an"` para consultar los nombres de las personas que realizaron los commits.
Revisar el historial permite comprobar quién hizo cada cambio y seguir la evolución del proyecto.
Esto es especialmente útil cuando varias personas trabajan de manera colaborativa en un mismo repositorio.
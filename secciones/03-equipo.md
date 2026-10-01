## 3.1 Git y GitHub no son lo mismo

Git es un sistema de control de versiones que se utiliza directamente
en la computadora para registrar los cambios realizados en un proyecto.
Git permite crear commits y consultar el historial de modificaciones.
GitHub, en cambio, es una plataforma en linea donde se pueden almacenar
repositorios Git y trabajar con otras personas. Git funciona de manera
local, mientras que GitHub permite compartir el repositorio de forma
remota y colaborar con otros integrantes del equipo.

## 3.3 Conflictos

Un conflicto ocurre cuando dos personas modifican la misma parte de un archivo y Git no puede combinar los cambios automaticamente.
Esto puede suceder al ejecutar `git pull` cuando existen cambios diferentes entre el repositorio local y remoto.
Git muestra las diferencias utilizando las marcas `<<<<<<<`, `=======` y `>>>>>>>`.
Estas marcas permiten identificar que version pertenece a cada cambio.
Para resolver el conflicto, se deben revisar ambas versiones y decidir cual conservar o si se pueden combinar.
Despues de realizar los cambios, se eliminan las marcas del conflicto.
Finalmente, se utiliza `git add` para indicar que el conflicto fue solucionado.
Luego se realiza un `git commit` para guardar la resolucion en el repositorio.

## 3.3 Conflictos

Un conflicto ocurre cuando dos personas modifican la misma parte de un archivo y Git no puede decidir que version conservar.
Esto puede ocurrir al ejecutar `git pull` cuando existen cambios diferentes entre el repositorio local y remoto.
Git muestra las diferencias con las marcas `<<<<<<<`, `=======` y `>>>>>>>`.
Se deben revisar ambas versiones para decidir cual conservar o si se pueden combinar.
Despues de resolverlo, se eliminan las marcas del conflicto y se guarda el archivo.
Luego se utiliza `git add` para indicar que el conflicto fue solucionado.
Finalmente, se realiza un `git commit` para guardar los cambios resueltos.


## 3.4 Buenas practicas de commits

Es recomendable hacer **commits pequenos** para que cada uno represente un cambio especifico.
Se debe procurar hacer un commit por cada cambio realizado en el proyecto.
Los mensajes deben ser **descriptivos** para saber facilmente que se modifico.
Es mejor escribir los mensajes en **presente**, por ejemplo: `Agregar pagina de inicio`.
Tambien se debe evitar mezclar muchos cambios diferentes en un mismo commit.
De esta forma, el historial del proyecto se mantiene ordenado y es mas facil revisar los cambios.

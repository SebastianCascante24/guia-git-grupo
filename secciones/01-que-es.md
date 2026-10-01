# Que es control de versiones

## 1.1 Definición de control de versiones

Es registrar los cambios que se hacen en un repo a lo largo del tiempo, permite que se pueda consultar el historial, comparaciones entre versiones y volver a una version especifica cuando se necesite, cada cambio o commit en este caso queda guardado con:

- quien lo hizo
- cuando lo hizo
- mensaje descriptivo de porque lo hizo (depende de la persona)
- los cambios que hizo y sobre que archivos

## 1.2 El método de las copias con fecha y sus problemas

es duplicar la carpeta o el archivo y le agrega la fecha al nombre 

los principales problemas son:

- desorden por acumulacion de copias
- cada copia guarda todo el proyecto po mas que los cambios sean minimos (se desperdicia espacio)
- el "historial" no es muy util porque solo indica fechas
- comparar entre "versiones" es manual

## 1.3 Qué resuelve un sistema de control de versiones

- cada version se guarda con autor, cambio, fecha y aveces mensaje
- se puede restaurar a versiones anteriores
- muestra que lineas se cambiaron entre las versiones

## 1.4 Centralizado y distribuido

Control de versiones centralizado: un solo servidor con el repositorio completo y su historial. Cada persona descarga una copia de trabajo y envía sus cambios al servidor. 
- ventajas: modelo sencillo, control de accesos en un solo lugar.
- desventajas: depende de la conexión con el servidor para casi todas las operaciones y, si el servidor falla y no hay respaldo, se puede perder el historial.

Control de versiones distribuido: cada persona tiene una copia completa del repositorio con todo el historial. Los cambios se registran localmente y luego se sincronizan con otros repositorios.
- ventajas: se trabaja sin conexión, las operaciones son rápidas, cada copia sirve de respaldo y facilita flujos con ramas.
- desventajas: mayor curva de aprendizaje y conceptos adicionales (clonar, fetch, push, pull).
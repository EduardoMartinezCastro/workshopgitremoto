# Git Stash

El comando git stash almacena temporalmente (o guarda en un stash) los cambios que hayas efectuado en el código en el que estás trabajando para que puedas trabajar en otra cosa y, más tarde, regresar y volver a aplicar los cambios más tarde. Guardar los cambios en stashes resulta práctico si tienes que cambiar rápidamente de contexto y ponerte con otra cosa, pero estás en medio de un cambio en el código y no lo tienes todo listo para confirmar los cambios.

## Uso

`git stash`

Toma todos los archivos con seguimiento y quita del stage las modificaciones realizadas colocandolos en un área de trabajo temporal. Excluye los cambios en archivos ignorados y archivos nuevos que no hayan sido preparados. 

`git stash save "etiqueta"`

Realiza el stash de la misma manera que el comando anterior, con la unica diferencia de que agrega una etiqueta para poder identificarlo a la hora de recuperar los cambios.

`git stash pop`

Recupera los archivos del ultimo stash y los devuelve al stage

`git stash list`

Muestra el listado de los stash almacenados

`git stash pop stash@{indice}`

Te permite recuperar el stash en el indice indicado, este indice puede ser visto cuando ejecutas `git stash list`

`git stash clear`

Elimina todos los stash que tenemos almacenados

## Resumen
El comando `git stash` es muy sencillo de comprender y manejar pero es una herramienta muy poderosa la cual nos permite guardar cambios que son importantes para nosotros y tener un control de nuestros cambios almacenados.

Para conocer más a detalle este comando revisa: [git stash](https://www.atlassian.com/es/git/tutorials/saving-changes/git-stash)
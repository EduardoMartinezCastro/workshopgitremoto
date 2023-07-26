# Git Add

El comando `git add` añade un cambio del directorio de trabajo en el entorno local. De este modo, indica a Git que quieres incluir actualizaciones en un archivo concreto en la próxima confirmación. Sin embargo, `git add` no afecta al repositorio de manera significativa: en realidad, los cambios no se registran hasta que ejecutas git commit.

## Uso 
Para utilizar `git add` puedes utilizar los siguientes comandos.

`git add <archivo>`

Prepara un archivo para el siguiente commit


`git add <directorio>`

Prepara todos los cambios del directorio especificado para el siguiente commit

`git add -A` ó `git add *`

Prepara todos los cambios hechos en el repositorio para el siguiente commit

`git add -p`

Inicia una sesión de entorno de ensayo interactiva que te permite elegir las partes de un archivo que quieres añadir a la siguiente confirmación. Se te presentarán una serie de cambios y se te solicitará un comando. Utiliza y para preparar el fragmento, n para ignorarlo, s para dividirlo en fragmentos más pequeños, e para editarlo manualmente y q para salir.

## Resumen
En resumen, `git add` es el primer comando de una cadena de operaciones que ordena a git que "guarde" el estado del proyecto en ese momento en el historial de confirmaciones.

Para conocer más a detalle este comando revisa: [git add](https://www.atlassian.com/es/git/tutorials/saving-changes)
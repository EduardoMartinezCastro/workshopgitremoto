# Git Pull

El comando `git pull` se emplea para extraer y descargar contenido desde un repositorio remoto y actualizar al instante el repositorio local para reflejar ese contenido. 
El comando `git pull` es, en realidad, una combinación de dos comandos, `git fetch` seguido de `git merge`. En la primera etapa de la operación `git pull` ejecutará un `git fetch` en la rama local a la que apunta HEAD. Una vez descargado el contenido, `git pull` entrará en un flujo de trabajo de fusión. Se creará una nueva confirmación de fusión y se actualizará HEAD para que apunte a la nueva confirmación.

## Uso
El comando git pull ejecuta en primer lugar git fetch, que descarga el contenido del repositorio remoto especificado. Después, se ejecuta git merge para fusionar las referencias y los encabezados del contenido remoto en una nueva confirmación de fusión local.

![image](https://wac-cdn.atlassian.com/dam/jcr:63e58c34-b273-4e48-a6b1-6e3ba4d4a0ea/01%20bubble%20diagram-01.svg?cdnVersion=1132)

En este ejemplo se descargaran los cambios hechos desde que se separaron las ramas local y principal y al ejecutar `git pull` se creará un nuevo commit en donde se incorporen los cambios de la rama remota a la local. Importante saber que al ejecutar este comando los cambios que se realicen quedarán en el repositorio local, por lo que si se requieren subir dichos cambios a la rama remota requerirá pasos extra.

![image](https://wac-cdn.atlassian.com/dam/jcr:0269bb2d-eb7f-43d8-80a2-8afa88d11eea/02%20bubble%20diagram-02.svg?cdnVersion=1132)

Para utilizar `git pull` puedes utilizar los siguientes comandos.

`git pull <remoto>`

Recupera la copia del origen remoto especificado de la rama actual y fusiónala de inmediato en la copia local.

`git pull --no-comit <remoto>`

Recupera el contenido remoto pero no genera una confirmación de la fusión del contenido.

`git pull --rebase <remoto>`

Al momento de la integración de los cambios en lugar de hacer `git merge` hace un `git rebase`

`git pull --verbose`

Proporciona una salida detallada durante la incorporación de cambios que muestra el contenido descargado y los detalles de la fusión

## Resumen
En resumen, `git pull` es el comando que nos permite integrar los cambios del repositorio remoto a nuestro repositorio local.

Para conocer más a detalle este comando revisa: [git pull](https://www.atlassian.com/es/git/tutorials/syncing/git-pull)
# Fetch

El comando git fetch descarga commits, archivos y referencias de un repositorio remoto a tu repositorio local. Esta acción la llevas a cabo cuando quieres ver en qué han estado trabajando los demás. Es similar al comando svn update porque te permite ver cómo ha progresado el historial central, pero no te obliga a fusionar los cambios en tu repositorio. Git aísla el contenido recuperado del contenido local existente sin tener ningún tipo de repercusión sobre el desarrollo local de tu trabajo. El contenido recuperado debe extraerse específicamente con el comando git checkout. Esto permite que la recuperación constituya una forma segura de revisar commits antes de integrarlos en tu repositorio local.

Para descargar contenido de un repositorio remoto, los comandos git pull y git fetch están disponibles para realizar esta tarea. Puedes considerar git fetch como la versión segura de los dos comandos. Este comando descarga el contenido remoto, pero no actualiza el estado de trabajo del repositorio local, por lo que tu trabajo actual no se verá afectado. git pull constituye una alternativa más agresiva, ya que descarga el contenido remoto a la rama local activa e inmediatamente ejecuta git merge para crear un commit fusionado con el nuevo contenido remoto. Si tienes cambios pendientes en curso, esta acción provocará conflictos e iniciará el flujo de resolución de conflictos de fusión.

# Opciones y comandos git fetch 
`git fetch <remote>` :
Recupera todas las ramas del repositorio. También descarga todos los commits y archivos requeridos del otro repositorio.
`git fetch <remote> <branch> :`
Realiza la misma acción que el comando anterior, pero solo recupera la rama especificada.
`git fetch --all` :
Una función potente que recupera todos los repositorios remotos registrados y sus ramas
`git fetch --dry-run` :
La opción --dry-run ejecutará una demo del comando. Genera ejemplos de acciones que realizará durante la recuperación, pero no los aplica.
 
# Resumen 
En resumen, git fetch es un comando principal que se usa para descargar contenidos desde un repositorio remoto. git fetch se usa en combinación con git remote, git branch, git checkout y git reset para actualizar un repositorio local al estado de un remoto. El comando git fetch es una pieza fundamental de los flujos de trabajo colaborativos de git. git fetch presenta un comportamiento similar a git pull, aunque git fetch se puede considerar una versión más segura y menos destructiva.

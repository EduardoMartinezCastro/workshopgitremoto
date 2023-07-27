# Amend

### Modificar último commit

```
git commit --amend
```
El comando anterior es una manera práctica de **modificar el commit más reciente**. Te permite combinar los cambios preparados con el commit anterior en lugar de crear un commit nuevo. También puede usarse para **editar el anterior mensaje del commit** sin cambiar la instantánea. Sin embargo, el comando no se limita a alterar el commit más reciente, sino que lo reemplaza por completo, por lo que el commit corregido será una entidad nueva con su propia referencia. Para Git, se verá como un commit nuevo

### Cambiar mensaje del último commit
Digamos que acabas de realizar un commit y te das cuenta de que hay un error en el mensaje de registro. Ejecutar este comando cuando no hay nada preparado te permite editar el mensaje del commit sin alterar su instantánea.

Los commits prematuros ocurren cada dos por tres durante el curso del desarrollo. Es fácil olvidarse de preparar un archivo o dar el formato incorrecto al mensaje del commit. La marca **--amend** es una manera cómoda de arreglar estos pequeños fallos.

```
git commit --amend -m "an updated commit message"
```
Añadir la opción **-m** te permite escribir un nuevo mensaje desde la línea de comandos sin tener que abrir un editor.

### No modifiques commits públicos
Los commits corregidos son, de hecho, commits totalmente nuevos y el commit anterior ya no estará disponible en tu rama actual. Esto tiene las mismas consecuencias que restablecer una instantánea pública. Procura no corregir un commit en el que otros desarrolladores hayan basado su trabajo, ya que crea una situación confusa para ellos de la cual es complicado recuperarse.

Para más información da clic [aquí](https://www.atlassian.com/es/git/tutorials/rewriting-history).
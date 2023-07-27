# Reset

El commando git reset es un comando complejo y versatil para deshacer
cambios. Tiene 3 formas principales de invocarse:

- soft
- mixed
- hard

```sh git reset ``` cambia, como minimo, donde la rama actual (HEAD) esta apuntado. La diferencia entre ```sh --mixed y  soft```, es si el index es modificado o no. Entonces si estamos en una rama master
con estos commits, desde C:

```sh - A - B - C (master)```

```sh HEAD ``` apunta a ```sh C ``` y el index concuerda con ```sh C ```

Cuando ejecutamos ```sh git reset --soft B ```, ```sh master``` (y por lo tanto ```sh HEAD```) apuntan a ```sh B```, pero el index aun
tiene cambios de ```sh C```; ```sh git status ``` los mostrara como
en staged.

Cuando ejecutamos ```sh git reset --mixed B``` (es la opcion por defecto), ```sh master``` y ```sh HEAD```, apuntan a ```sh B```, pero esta vez el index tambien es modificar para concordar con ```sh B```. Si hacemos ```sh git commit``` en este punto, nada aparecera,
ya que el index hace match con ```sh HEAD```. Todavia hay cambios
en el "Working directory", pero no estan en el index(unstaged).
Para hacer commit de ellos, se debe hacer un ```sh git add``` y despues commitear los cambios.

Finalmente, si corremos ```sh git reset --hard B ```, todos los cambios en ```sh C ```, asi como cualquier cambio no commiteado, sera
removido, y los archivos actuales seran iguales a ```sh B``` .

## En resumen

> ```sh --soft```: "descomitea" los cambios, que permanecen en el index(Staged)

>```sh --mixed```: "descomitea" y "unstagea", los cambios permanecen en el working directory.

>```sh --hard```: "descomitea", "unstagea" y borra los cambios, nada permanece en el working directory.

![Git reset](https://i.stack.imgur.com/qRAte.jpg)

Para una explicacion mas detallada, da click [aqui](https://www.atlassian.com/git/tutorials/undoing-changes/git-reset).
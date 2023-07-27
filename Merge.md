# _Merge_

El comando _git merge_ permite tomar las líneas independientes de desarrollo creadas por git branch e integrarlas en una sola rama. La fusión siempre ocurre en la rama actual, por lo que la rama de función especificada se fusionará con la rama actual.


![](merge01.png 'Estado inicial del repositorio. En este caso, se quiere fusionar la rama Feature con la rama Main.')

![](merge02.png 'Estado final del repositorio tras aplicar el comando git merge.')

Al crear una confirmación de fusión, Git tratará de fusionar automáticamente los historiales independientes. Sin embargo, si encuentra datos que se han cambiado en ambos historiales, no podrá combinarlos de ese modo. En ese caso, se crea un conflicto de control de versiones y Git solicitará la intervención del usuario para poder continuar. 

### Comando

La fusión de dos ramas se lleva a cabo bajo el siguiente comando.

```sh

$ git checkout Main
$ git merge Feature

```
Por medio del comando _checkout_ movemos el puntero a la rama Main, que será la rama actual. Al aplicar el comando _merge_ se indica la rama que se fusionará con la rama actual.

### Más información
  Para más información visita [git merge] (https://www.atlassian.com/es/git/tutorials/using-branches/git-merge)



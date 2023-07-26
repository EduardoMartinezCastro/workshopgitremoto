# Revert

Revierte los cambios de un commit generando un nuevo commit, es decir, revierte los cambios de un commit sin destruir la historia.

Suponiendo que hay una rama ```sh master``` , con los commits A, B y C, y queremos revertir los cambios del ultimo commit "C" :

```sh
    A - B - C  
```

Bien pondemos ejecutar ```sh git revert HEAD ``` o ```sh git revert C ```, esto deshara los cambios hechos en C, y creara un nuevo
commit para ello, ```sh D```

```sh
    A - B - C - D  
```

Para mas info, visita [aqui](https://www.atlassian.com/git/tutorials/undoing-changes/git-revert).
# git-cherry-pick

## Descripción

Copia uno o más commits, creando un nuevo commit en la rama actual con el mismo mensaje y contenido que otro commit.

## Ejemplos

`git cherry-pick hash1 hash2 hashN`
Copia todos los commits especificados a la rama actual.

`git cherry-pick hash1^..hashN`
Copia a la rama actual todos los commits comprendidos entre el rango `hash1` hasta `hashN`.

`git cherry-pick hash1..hashN`
Copia a la rama actual los commits `hash1` y `hashN`, excluyendo los intermedios.

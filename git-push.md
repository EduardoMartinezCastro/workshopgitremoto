# git-push

## Descripción

Actualiza refs remotas usando refs locales, mientras envía los objetos necesarios para completar las refs dadas.

## Ejemplos

`git push`
Funciona como `git push <remote>`, donde `<remote>` es el remote de la rama actual (`origin` por default).

`git push origin`
Empuja la rama actual al upstream configurado si tiene el mismo nombre que la rama actual.

`git push origin master`
Encuentra una ref que coincida con `master` en el repositorio y actualiza la misma ref en el repositorio `origen`con ella. Si `master` no existía de forma remota, se crearía.

## Opciones

`-u, --set-upstream`
Para cada rama que esté actualizada o empujada con éxito, agrega una referencia upstream.

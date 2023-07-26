# Chechkout
![image](https://static.javatpoint.com/tutorial/git/images/git-checkout.png)
### Chechkout para cambiar de rama
```
git checkout <nombreRama>
```
Te permite desplazarte entre las ramas creadas por git branch. Al extraer una rama, se actualizan los archivos en el directorio de trabajo para reflejar la versión almacenada en esa rama y se indica a Git que registre todas las confirmaciones nuevas en dicha rama. Puedes contemplar todo esto como una forma de seleccionar la línea de desarrollo en la que trabajas.

Disponer de una rama específica para cada nueva función supone un cambio drástico en comparación con el flujo de trabajo tradicional de SVN. Hace que resulte ridículamente sencillo probar nuevos experimentos sin temor a arruinar las funciones existentes y permite trabajar al mismo tiempo en muchas funciones que no guardan relación entre sí. Además, las ramas facilitan varios flujos de trabajo colaborativos.

### Chechkout para cambiar y crear una rama

El comando **git checkout** se usa habitualmente junto con **git branch**. El comando **git branch** permite crear una rama nueva. Si quieres empezar a trabajar en una nueva función, puedes crear una rama nueva a partir de la rama main con **git branch new_branch**. Una vez creada, puedes usar **git checkout new_branch** para cambiar a esa rama. Además, el comando **git checkout** acepta el argumento -b, que actúa como un práctico método que creará la nueva rama y cambiará a ella al instante. Puedes trabajar en varias funciones en un solo repositorio alternando de una a otra con git checkout.

```
git checkout -b <nombreRama>
```
ó
```
git checkout -b <nombreRama> <ramaExistente>
```

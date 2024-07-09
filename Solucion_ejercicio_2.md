## Ejercicio 2: Trabajar con ramas

1. Crea una nueva rama llamada "rama-caracteristica".
```git branch rama-caracteristica```
2. Cambia a la nueva rama.
```git checkout rama-caracteristica```
3. Realiza algunos cambios en el archivo README.md.
crear README.md y añadir el texto
4. Añade los cambios al área de preparación y haz un commit.
```git commit -a -m "Añadida información sobre nueva característica"```
o
```git add README.md
git commit -m "Añadida información sobre nueva característica"```
5. Vuelve a la rama principal.
```git checkout main```
6. Fusiona la "rama-caracteristica" con la rama principal.
```git merge rama-caracteristica```
7. Elimina la "rama-caracteristica".
```git branch -d rama-caracteristica```

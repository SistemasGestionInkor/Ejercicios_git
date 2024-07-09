## Ejercicio 4: Etiquetar y comparar cambios

1. Crea una etiqueta anotada para tu versión actual (por ejemplo, "v1.0")
```git tag -a v1.0 -m "Versión 1.0 del proyecto"```

2. Sube la etiqueta al repositorio remoto
```git push origin v1.0```
o
```git push --tags```

3. Realiza algunos cambios en tu proyecto y haz un commit

Realizar cambios en el archivo

```
git add README.md
git commit -m "Actualizaciones post v1.0"
```

4. Utiliza `git diff` para comparar los cambios entre tu versión etiquetada y el estado actual
```git diff v1.0 HEAD```

5. Crea una nueva rama llamada "caracteristica-experimental" y colocarse en ella
```git checkout -b caracteristica-experimental```
o
```
git branch caracteristica-experimental
git checkout caracteristica-experimental
```

6. Realiza algunos cambios en esta nueva rama y haz un commit
añadir cambios al archivo
```
git add README.md
git commit -m "Añadida característica experimental"
```
o

```git commit -a -m "Añadida característica experimental"```

7. Utiliza `git diff` para comparar las diferencias entre la rama principal y la rama caracteristica-experimental
   
```git diff main caracteristica-experimental```

## Ejercicio 3: Deshacer cambios y trabajar con repositorios remotos

1. Realiza algunos cambios en el archivo README.md
crear README.md y añadir el texto

2. Imagina que no quieres mantener estos cambios y reviértelos usando Git
```git checkout -- README.md```

3. Crea un repositorio remoto en GitHub o GitLab
(Este paso se realiza en la interfaz web de GitHub o GitLab)

4. Añade el repositorio remoto a tu repositorio local
```git remote add origin https://github.com/tu-usuario/mi_proyecto.git```

5. Sube tu repositorio local al repositorio remoto
```git push -u origin main```

6. Realiza un cambio en tu archivo README.md en el repositorio remoto usando la interfaz web
(Este paso se realiza en la interfaz web de GitHub o GitLab)

7. Obtén los cambios del repositorio remoto
```git fetch origin```

8. Fusiona los cambios obtenidos en tu repositorio local
```git merge origin/main```
# Soluciones de los Ejercicios de Git

## Solución del Ejercicio 1: Configurar un nuevo repositorio y realizar cambios

```bash
# 1. Inicializa un nuevo repositorio Git en un directorio llamado "mi_proyecto"
mkdir mi_proyecto
cd mi_proyecto
git init

# 2. Crea un archivo llamado "README.md" y añade algún contenido
echo "# Mi Proyecto" > README.md

# 3. Comprueba el estado de tu repositorio
git status

# 4. Añade el archivo README.md al área de preparación (staged area)
git add README.md

# 5. Realiza un commit con los cambios y un mensaje descriptivo
git commit -m "Inicialización del proyecto con README"

# 6. Visualiza el historial de commits
git log
```

## Solución del Ejercicio 2: Trabajar con ramas

```bash
# 1. Crea una nueva rama llamada "rama-caracteristica"
git branch rama-caracteristica

# 2. Cambia a la nueva rama
git checkout rama-caracteristica

# 3. Realiza algunos cambios en el archivo README.md
echo "Nueva característica en desarrollo" >> README.md

# 4. Añade los cambios al área de preparación y haz un commit
git add README.md
git commit -m "Añadida información sobre nueva característica"

# 5. Vuelve a la rama principal
git checkout main

# 6. Fusiona la "rama-caracteristica" con la rama principal
git merge rama-caracteristica

# 7. Elimina la "rama-caracteristica"
git branch -d rama-caracteristica
```

## Solución del Ejercicio 3: Deshacer cambios y trabajar con repositorios remotos

```bash
# 1. Realiza algunos cambios en el archivo README.md
echo "Cambios que no queremos mantener" >> README.md

# 2. Imagina que no quieres mantener estos cambios y reviértelos usando Git
git checkout -- README.md

# 3. Crea un repositorio remoto en GitHub o GitLab
# (Este paso se realiza en la interfaz web de GitHub o GitLab)

# 4. Añade el repositorio remoto a tu repositorio local
git remote add origin https://github.com/tu-usuario/mi_proyecto.git

# 5. Sube tu repositorio local al repositorio remoto
git push -u origin main

# 6. Realiza un cambio en tu archivo README.md en el repositorio remoto usando la interfaz web
# (Este paso se realiza en la interfaz web de GitHub o GitLab)

# 7. Obtén los cambios del repositorio remoto
git fetch origin

# 8. Fusiona los cambios obtenidos en tu repositorio local
git merge origin/main
```

## Solución del Ejercicio 4: Etiquetar y comparar cambios

```bash
# 1. Crea una etiqueta anotada para tu versión actual (por ejemplo, "v1.0")
git tag -a v1.0 -m "Versión 1.0 del proyecto"

# 2. Sube la etiqueta al repositorio remoto
git push origin v1.0

# 3. Realiza algunos cambios en tu proyecto y haz un commit
echo "Nuevas actualizaciones después de la versión 1.0" >> README.md
git add README.md
git commit -m "Actualizaciones post v1.0"

# 4. Utiliza `git diff` para comparar los cambios entre tu versión etiquetada y el estado actual
git diff v1.0 HEAD

# 5. Crea una nueva rama llamada "caracteristica-experimental"
git checkout -b caracteristica-experimental

# 6. Realiza algunos cambios en esta nueva rama y haz un commit
echo "Característica experimental en desarrollo" >> README.md
git add README.md
git commit -m "Añadida característica experimental"

# 7. Utiliza `git diff` para comparar las diferencias entre la rama principal y la rama caracteristica-experimental
git diff main caracteristica-experimental
```

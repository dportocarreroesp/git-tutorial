### Inicializando git en el proyecto
git init

### Agregando la dirección para el repositorio remoto
Ya que ya se hacía uso de git en este proyecto, en lugar de agregar la dirección para el remoto, la actualizaremos.
git remote set-url origin https://github.com/khannom/git-tutorial.git


### Agregando los cambios al staging area
git add .

### Guardando los cambios para subir al repositorio remoto
git commit -m "boton information header"

### Subiendo los archivos al repositorio remoto(Github)
git push origin master

### Creando un branch para editar el readme
git checkout -b readme

### Revisando que se creó el branch y que estamos en este
git branch

### Luego de actualizar el readme, guardamos los cambios en el branch actual
git add .
git commit -m "readme actualizado"

### Para poder subir los cambios al repositorio remoto, necesitamos actualizar el branch master con los cambios del branch readme
Nos movemos al branch master:
git checkout master

### Agregando los cambios del branch readme al branch master
git merge readme

### Comprobando que los cambios fueron guardados con éxito en el branch master
git log

### Supongamos que no me gustó cómo quedó el readme, entonces regreso a la versión anterior






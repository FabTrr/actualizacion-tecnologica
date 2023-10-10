**Comandos git más utilizados**

Git es un sistema de control de versiones que permite rastrear los cambios en un conjunto de archivos. Los comandos git permiten realizar diversas operaciones, como crear un repositorio, agregar archivos, realizar cambios, y enviar los cambios a un repositorio remoto.

**Comando | Descripción | Ejemplo de uso**
---|---|---|
`git init` | Crea un repositorio git en el directorio actual. | `git init`
`git add` | Agrega archivos o directorios al área de staging. | `git add README.md`
`git commit` | Crea un commit con los cambios realizados en el área de staging. | `git commit -m "Añade un nuevo archivo README"`
`git status` | Muestra el estado actual del repositorio. | `git status`
`git log` | Muestra el historial de commits. | `git log`
`git checkout` | Cambia a una rama específica. | `git checkout master`
`git merge` | Combina dos ramas. | `git merge develop`
`git push` | Envia los cambios al repositorio remoto. | `git push origin master`
`git pull` | Trae los cambios del repositorio remoto. | `git pull origin master`

**Ejemplo de uso**

Para crear un nuevo repositorio git, podemos ejecutar el siguiente comando:

```
git init
```

Esto creará un archivo `.git` en el directorio actual.

Para agregar un archivo al área de staging, podemos ejecutar el siguiente comando:

```
git add README.md
```

Esto agregará el archivo `README.md` al área de staging.

Para crear un commit con los cambios realizados en el área de staging, podemos ejecutar el siguiente comando:

```
git commit -m "Añade un nuevo archivo README"
```

Esto creará un commit con el mensaje "Añade un nuevo archivo README".

Para mostrar el estado actual del repositorio, podemos ejecutar el siguiente comando:

```
git status
```

Esto mostrará una lista de los archivos que han sido modificados o agregados.

Para mostrar el historial de commits, podemos ejecutar el siguiente comando:

```
git log
```

Esto mostrará una lista de todos los commits realizados en el repositorio.

Para cambiar a una rama específica, podemos ejecutar el siguiente comando:

```
git checkout master
```

Esto cambiará a la rama `master`.

Para combinar dos ramas, podemos ejecutar el siguiente comando:

```
git merge develop
```

Esto combinará la rama `develop` con la rama actual.

Para enviar los cambios al repositorio remoto, podemos ejecutar el siguiente comando:

```
git push origin master
```

Esto enviará los cambios al repositorio remoto llamado `origin`.

Para traer los cambios del repositorio remoto, podemos ejecutar el siguiente comando:

```
git pull origin master
```

Esto traerá los cambios de la rama `master` del repositorio remoto llamado `origin`.

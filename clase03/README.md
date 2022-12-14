# Clase 03

## Crear repositorio en GitHub

![crear-repo](imgs/creo-repo.png)

### Si el repo no esta creado

```sh
…or create a new repository on the command line
echo "# nombre-repo" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/mlapeducacionit/nombre-repo.git
git push -u origin main
```

### Si el repo local esta creado

…or push an existing repository from the command line

```sh
git remote add origin https://github.com/mlapeducacionit/nombre-repo.git
git branch -M main # No es necesario
git push -u origin main
```

## GIT REMOTE
Si quiero saber si tengo un remoto

```sh
git remote
```

> Más detalle sobre los remotos

```sh
git remote -v
```

> Para agregar un remoto

```sh
git remote add <alias> <url-del-remoto>
```

> Para borrar un remoto

```sh
git remote remove <alias>
```

## Si quiero subir al repositorio remoto el local

> La primera vez

```sh
git push -u <alias-del-remoto> <rama-local-que-quiero-subir>
git push -u origin main
```

> Las siguientes veces que quiera subir

```sh
git push
```

## cuando se genera un conflicto entre el repositorio subido y el que queremos subir (cambio de hash)
git push -f

## archivo .gitignore
informo que archivos o carpetas no subir al servidor

## archivo .gitkeep
indica a git que una carpeta va a quedar vacia pars futuros usos

## GIT ADD patch (dividir varios commit)
git add --patch
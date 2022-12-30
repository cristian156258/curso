## tag (puntero)
Sirve para marcar las versiones de mi aplicaxion. Apuinta a un commit
git tag (nombre del tag)

## otra forma de crear tag
git tag -a (version del programa) -m (mensaje opcional)

## ver info sobre el tag
git show (nombre del tag)

## hacer tag de un commit anterior al ultimo
git tag (hash del commit deseado)


## borrar un tag
git tag -d (nombre del tag)

## borrar un tag remoto
git push delete origin (nombre del tag)


## subir un tag
### subir un tag especifico
git push (nombre del tag)

## punteros estaticos 
branches, tags

## puntero dinamico
HEAD


## Trabajar en proyectos Open Source (Pull Request)
Hacer un fork del proyecto. Del proyecto del cual quiero contribuir (Me voy copiar en mi cuenta el repo del proyecto original)
Me clono el fork desde mi cuenta github
Trabajo normalmente. Subo los cambios (A repo propio)
Me voy al proyecto original en el apartado Pull Request. Creo un nuevo Pull Request. Algunas veces aparece en mi repo la posibilidad Pull Request.
Si el repo original sufrió más modificaciones. (Commits). Voy a tener que actualizar mi fork.

Voy a la cuenta del proyecto original y me copio la url del repositorio

Y agrego en mi repositorio local, la url (el remoto) del proyecto original.

git remote upstream

Me traigo los cambios del repositorio original a mi repo local

git pull upstream

Subo a mi repositorio remoto (Fork) las actualizaciones del repo local

git push origin


## git rebase
lo mismo que el merge
git rebase (nombre de rama)

## rebase interactivo
git rebase -i
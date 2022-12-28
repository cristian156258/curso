## TIPOS DE MERGE (FISIONES)
Fast-forward (ningun conflicto. Automatico - no agrega un commit)
recursivo (automatico sin conflicto - agrega un commit )
Manual (hay conflictos que el usuario tiene que resolver)

## para crear una rama y moverme a esa rama en simultaneo   agregadoooooooooo
git switch -c (nombre de rama) agregadooooooooooo
cambiooooooooooooooooooooooooooooooooooooooooooooooooooooooo



cambiooooooooooooooooo
cambiooooooooooooo


## stash
trabaja con juna estructura de datos tipo pila
el primero que entra sale ultimo
permite resgistrartemporalmente cambios que estan en el area de trabajo, que todavia no estan listo para ser commiteados

## crear stash
git stash

## listar los stash
git stash list

## Eliminar un stack
git stack drop


## Listo los stashes
git stash list
## Veo en detalle lo que hay dentro del stash
git stash show -p # Me muestra la info detalla del contenido del último stash
git stash show -p stash@{5} # Me muestra la info detalla del contenido del stash indicado
## Comparar con ramas los stashes
git diff <número-de-stash> <rama>
git diff stash{0} main
## Recupero el último stash que tengo en la pila
git stash pop
## Borrar un stash
git stash drop # Me va borrar el último stash
git stash drop <numero-stash> # Borro un stash en particular
git stash drop stash@{1}
## Aplicar un stash diferente si quisiera del último
git stash apply # Me va aplicar el último stash
git stash apply <numero-stash> # Aplico un stash en particular
git stash apply stash@{1}
## Para borrar todos los stashes
git stash clear
## A partir de un stash crear un rama
git stash branch <nombre-de-ramas>

## git reset
reset soft (suave) No destrictivo. borra el commit, pero deja los cambios en el stage area
reset mixed (mixed) No destructivo. Borra el commit, pero camvbios los deja en el working directory
reset hard (dura) Destructivo. Borra el commit y no deja los cambios en nigun lado
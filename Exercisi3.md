# Exercisi 1
## Aquest procés ens permet eliminar l'última línia del fitxer index.txt, desfer els canvis realitzats i tornar al seu estat anterior.
>git status
>
>En la branca master
>
>Canvis no «staged» per a cometre:
>
>(useu «git add <fitxer>...» per a actualitzar què es cometrà)
>
>(useu «git restore <fitxer>...» per a descartar canvis en el directori de treball) modificat: index.txt
>
>no hi ha canvis afegits a cometre (useu «git add» o «git commit -a»)
>
>git restore index.txt
>
>git status
>
>En la branca master no hi ha res a cometre, l'arbre de treball està net
>

# Exercisi 2

## Aquest procés ens permet explorar diferents estats del repositori, ja que traem i reintegrem canvis de la zona d'intercanvi temporal i el directori de treball.

>sed -i '$d' index.txt
>
>git add index.txt
>
>git status
>
>En la branca master
>
>Canvis a cometre: (useu «git restore --staged <fitxer>...» per a fer «unstage») modificat: index.txt
>
>git reset index.txt
>
>Canvis «unstaged» després del restabliment: M capitols/index.txt
>
>git status
>
>En la branca master
>
>Canvis no «staged» per a cometre:
>
>(useu «git add <fitxer>...» per a actualitzar què es cometrà)
>
>(useu «git restore <fitxer>...» per a descartar canvis en el directori de treball) modificat: index.txt
>
>no hi ha canvis afegits a cometre (useu «git add» o «git commit -a»)
>
>git restore index.txt
>
>git status
>
>En la branca master no hi ha res a cometre, l'arbre de treball està netExercisi 3


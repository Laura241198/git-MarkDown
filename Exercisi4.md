# Exercisi 1

>git branch bibliografia
>git branch
>bibliografia
>** master

# Exercisi 2
## Amb aquestes comandes, hem creat un nou fitxer "capitol4.txt", afegit els canvis a la zona d'intercanvi temporal i fet un commit amb el missatge "Afegit capítol 4.". L'última comanda git log --all, mostrarà la història completa del repositori, incloent totes les branques.

>git add capitol4.txt
>git commit -m "Afegit capítol 4"
>git log --all

# Exercisi 3

>git checkout bibliografia
>echo "- Chacon, S..."
>git add bibliografia.txt

# Exercisi 4
## Fusionem amb git merde i mostrem l'historial però que no copie ací ja que es mostra abans i desprès (i que és molt llarg i no em cabia en tota la captura d'una pantalla).

>git checkout master
>
>S'ha canviat a la branca «master»
>
>git merge bibliografia
>
>Merge made by the 'ort' strategy.
>
>capitols/bibliografia.txt | 1 +
>
>1 file changed, 1 insertion(+)
>
>create mode 100644 capitols/bibliografia.txt
>
>git log --all
>
>---------------mostra l'historial---------------
>
>git branch -d bibliografia
>
>S'ha suprimit la branca bibliografia (era 4445f92).
>
>git log --all

# Exercisi 5
## Ara, hem creat i canviat a la branca "bibliografia", fet canvis als fitxers bibliografia.txt en cada branca, fet commits, fusionat les branques resolent un conflicte i finalment mostrant la història del repositori incloent totes les branques.

>git branch bibliografia
>
>git checkout bibliografia
>
>S'ha canviat a la branca «bibliografia»
>
>echo "- Scott Chacon Ben Straub. Pro Git. Apress" > bibliografia.txt
>
>echo "- Ryan Hodson. Ry's Git Tutorial. Smashwords (2014)" >> bibliografia.txt
>
>git add bibliografia.txt
>
>git commit -m "Afegida nova referència bibliogràfica."
>
>[bibliografia e566c2f] Afegida nova referència bibliogràfica.
>
>1 file changed, 2 insertions(+), 1 deletion(-)
>
>git checkout master
>
>S'ha canviat a la branca «master»
>
>echo "- Chacon, S. and Straub, B. Pro Git. Apress" > bibliografia.txt
>
>echo "- Loeliger, J. and McCullough, M. Version control with Git. O'Reilly" >> bibliografia.txt
>
>git add bibliografia.txt
>
>git commit -m "Afegida nova referència bibliogràfica."
>
>[master 0e6ffb1] Afegida nova referència bibliogràfica.
>
>1 file changed, 2 insertions(+), 1 deletion(-)
>
>git merge bibliografia
>
>S'està autofusionant capitols/bibliografia.txt
>
>CONFLICTE (contingut): Conflicte de fusió en capitols/bibliografia.txt
>
>La fusió automàtica ha fallat; arregleu els conflictes i després cometeu el resultat.
>
>git add bibliografia.txtlaura@a217pc03:~/llibre/capitols$ git commit -m "Resolt conflicte de bibliografia."
>
>[master 3816abd] Resolt conflicte de bibliografia.

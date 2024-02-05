# Exercici 1

## Creació d'un nou repositori i configuració de Git

1. Crea un nou repositori anomenat "llibre" i mostra el seu contingut.
2. Configura Git definint el nom d'usuari, el correu electrònic i activa la sortida en color.
3. Mostra la configuració final.

mkdir llibre
cd llibre
git init
echo "Contingut del llibre" > llibre.txt
git add llibre.txtt
git commit -m "Afegir fitxer de mostra"
git config --global user.name "Laura Jorda"
git config --global user.email "laujortom@alu.edu.gva.es"
git config --global color.ui true

# Exercici 2

## Estes comandes verifiquen l'estat del repositori abans de realitzar canvis. Crea un fitxer anomenat "index.txt" amb el contingut proporcionat, verifica l'estat del repositori després de crear el fitxer, afig el fitxer "index.txt" a la zona d'intercanvi temporal i verifica l'estat del repositori després d'afegir el fitxer a la zona d'intercanvi temporal.

git status
echo -e "Capitol1(etc)"
git add .
git status

# Exercici 3

## Estes comandes fan un commit dels canvis realitzats amb el missatge "Afegit índex del llibre." i verifiquen l'estat del repositori per veure si hi ha canvis pendents o si tot està actualitzat.

git commit -m "Afegir index del llibre"
git status

# Exercici 4

## Amb estes comandes, s'actualitza el repositori amb el nou contingut de l'arxiu index.txt i es crea un commit amb el missatge desitjat.

echo -e "Capítol 1: Introducció a GIT\nCapítol 2: Fluxe de treball bàsic\nCapítol 3: Gestió de branques\nCapítol 4: Repositoris remots" > index.txt
 git diff
diff --git a/index.txt b/index.txt
index 4bbbb6a..463e85c 100644
--- a/index.txt
+++ b/index.txt
@@ -1,3 +1,4 @@
Capítol 1: Introducció a GIT
Capítol 2: Fluxe de treball bàsic
-Capítol 3: Repositoris remots
+Capítol 3: Gestió de branques
+Capítol 4: Repositoris remots
git add index.txt
git commit -m "Afegit capítol 3 sobre gestió
de branques"
[master 34af297] Afegit capítol 3 sobre gestió de branques
1 file changed, 2 insertions(+), 1 deletion(-)

# Exercici 5

## Mostra els canvis de l'última versió del repositori respecte a l'anterior utilitzant `git diff HEAD^ HEAD`.

git diff HEAD^ HEAD
git commit --amend -m "Afegit capítol 3"

# Exercici 6

## Amb aquests passos, els fitxers que comencen per "daw", tots els fitxers amb extensió "out" i les imatges (jpg, png, bmp i gif) seran ignorats per Git.

nano .gitignore
git add
git commit -m "Afegit .gitignore per ignorar fitxers específics."
[master b79dd53] Afegit .gitignore per ignorar fitxers específics.
1 file changed, 6 insertions(+)
create mode 100644 .gitignore

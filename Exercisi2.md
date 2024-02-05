# Exercisi 1

## Amb aquestes comandes, s'ha creat i registrat el primer capítol del llibre al repositori Git.

git log

# Exercisi 2

## La sortida de les comandes mostra la diferència entre el primer i segon commit, eliminant el fitxer `capitol1.txt`.

>git diff HEAD^ HEAD^^
>
>diff --git a/capitols/capitol1.txt b/capitols/capitol1.txt
>
>deleted file mode 100644
>
>index 39ad366..0000000
>
>--- a/capitols/capitol1.txt
>
>+++ /dev/null
>
>@@ -1 +0,0 @@
>
>-Git és un sistema de control de versions ideat per Linus Torvalds.

# Exercisi 3

## Amb aquestes comandes, hem afegit un nou capítol al llibre i mostrat les diferències entre la primera i l'última versió del repositori Git.

# Exercisi 4

## Amb aquestes comandes, hem afegit una nova línia al fitxer index.txt, afegit els canvis a la zona d'intercanvi temporal i fet un commit amb el missatge desitjat. La comanda git blame mostra qui ha fet canvis sobre el fitxer index.txt i en quina línia cada canvi s'ha produït.

>echo "Capítol 5: Conceptes avançats" >> index.txt
>
>git add index.txt
>
>git commit -m "Afegit capítol 5 a l'índex."
>
>[master c391fae] Afegit capítol 5 a l'índex.
>
>1 file changed, 1 insertion(+)
>
>create mode 100644 capitols/index.txt
>
>git blame index.txt
>
>c391fae4 (Laura Jorda 2024-01-29 12:55:20 +0100 1) Capítol 5: Conceptes avançats

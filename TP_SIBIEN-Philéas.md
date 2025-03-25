# Commandes Linux: édition salade de fruits

Si besoin, utilisez la commande `man [commande]` pour afficher la documentation sur une
commande en particulier.

## Mise en place d’un dossier

1. Vérifiez votre chemin actuel.
2. Placez vous dans le dossier `/home/[nom d'utilisateur]` en une seule
    commande.
3. Créez un dossier `TP` et un fichier texte `fichier1.txt` dans ce répertoire.
4. Affichez le contenu du répertoire `/home/[nom d'utilisateur]` et assurez-vous que
    le fichier et le dossier ont bien été créés.
5. Déplacez `fichier1.txt` dans `TP`.
6. Déplacez vous dans `TP`, puis affichez son contenu, le tout en une seule commande.

## Ajout de contenu dans un fichier

7. En utilisant la commande echo, insérez le texte suivant dans `fichier1.txt`

**`pomme\nbanane\norange\nfraise\nmangue`**

(indice: utilisez le paramètre -e pour interpréter les line breaks.)

8. Affichez le contenu du fichier pour confirmer son ajout.
9. Videz le terminal.

## Copie d’un fichier

10. Créez un fichier texte `fichier2.txt` dans `TP` puis affichez le contenu du dossier, le
    tout en une seule commande.
11. Copiez le contenu de `fichier1.txt` dans `fichier2.txt`.
12. Affichez `fichier2.txt`. Le contenu de `fichier1.txt` devrait apparaître.
13. Supprimez `fichier1.txt`.

## Filtrage d’un fichier

14. Filtrez toutes les lignes contenant la lettre **o** dans `fichier2.txt` et ajoutez le
    résultat dans un nouveau fichier `fruit_o.txt`, le tout en une seule commande.
15. Faites de même pour la lettre **n** , dans un nouveau fichier `fruit_n.txt`.
16. Affichez les contenus des deux fichiers. Quels fruits sont listés?


## Commandes à utiliser:

`man, pwd, cd, mkdir, touch, ls, echo, >, mv, cp, rm, grep`
TP par SIBIEN Philéas

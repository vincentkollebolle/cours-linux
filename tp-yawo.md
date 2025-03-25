_Comment créer un dossier dans le terminal sous Linux ? Donne la commande et explique son fonctionnement.

Comment vérifier l'espace disque disponible sur ton système Linux ? Quelle commande utilises-tu ?

Comment afficher la liste des fichiers et dossiers présents dans un répertoire ?

Comment renommer un fichier ou un dossier sous Linux ? Donne la commande et un exemple.

Comment déplacer ou copier un fichier d'un répertoire à un autre ? Donne la commande pour cela.

Comment afficher le contenu d'un fichier texte dans le terminal ? Quelle commande utilises-tu ?

Comment créer un fichier texte et y insérer du texte à partir du terminal ? Quelle commande utilises-tu ?

Comment supprimer un fichier ou un dossier sous Linux ? Quelle est la différence entre rm et rmdir ?

Comment rechercher un mot spécifique à l’intérieur d’un fichier texte avec le terminal ? Donne un exemple de commande.

Comment afficher les processus en cours sur ton système Linux et comment arrêter un processus ? Quelle commande utilises-tu ?






Créer un dossier :
mkdir nom_du_dossier

Vérifier l'espace disque :
df -h

Lister les fichiers :
ls

Renommer un fichier :
mv ancien_nom nouveau_nom

Déplacer ou copier un fichier :
Déplacer : mv fichier destination/
Copier : cp fichier destination/

Afficher le contenu d’un fichier :
cat fichier.txt

Créer un fichier et ajouter du texte :
echo "Texte" > fichier.txt

Supprimer un fichier ou dossier :
Supprimer fichier : rm fichier.txt
Supprimer dossier vide : rmdir dossier
Supprimer dossier non vide : rm -r dossier

Rechercher un mot dans un fichier :
grep "mot" fichier.txt

Afficher les processus et tuer un processus :
Afficher : ps aux
Tuer : kill PID

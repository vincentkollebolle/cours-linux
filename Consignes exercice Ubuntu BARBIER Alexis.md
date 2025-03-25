Feuille envoyer à Tetsuô Mariotti

Commandes :

1.  **Afficher le chemin absolu du répertoire courant**
2.  **Lister les fichiers et dossiers du répertoire courant avec
    détails**
3.  Créer un dossier nommé ExerciceUbuntu dans votre dossier personnel
4.  Créer un fichier fichier.txt dans ExerciceUbuntu
5.  Écrire \"Bonjour Ubuntu\" dans test.txt
6.  Afficher le contenu de test.txt
7.  Renommer fichier.txt en exercice.txt
8.  Supprimer le fichier exercice.txt
9.  Supprimer le dossier ExerciceUbuntu

Questions :

1.  Quelle commande permet d'afficher les fichiers cachés dans un
    dossier ?
2.  Quelle est la différence entre rm et rmdir ?
3.  Que fait la commande ls -al ?
4.  Quelle commande permet d\'afficher les 10 premières lignes d'un
    fichier texte ?
5.  Quelle commande permet d\'afficher l'espace disque utilisé sur le
    système ?

Correction :

Réponses commandes :

1.  Pwd
2.  ls -l
3.  mkdir \~/ExerciceUbuntu
4.  touch \~/ExerciceUbuntu/fichier.txt
5.  echo \"Bonjour Ubuntu\" \> \~/ExerciceUbuntu/fichier.txt
6.  cat \~/ExerciceUbuntu/fichier.txt
7.  mv \~/ExerciceUbuntu/fichier.txt \~/ExerciceUbuntu/exercice.txt
8.  rm \~/ExerciceUbuntu/exercice.txt
9.  rm \~/ExerciceUbuntu/exercice.txt

Réponses questions :

1.  ls -a
2.  rm va supprimer des fichiers et des dossiers ( -r pour les dossiers)
    et rmdir ne peut supprimer que des dossiers vides.
3.  Elle affiche la liste détaillée (-l) de tous les fichiers, y compris
    les fichiers cachés (-a).
4.  head -n 10 monfichier.txt
5.  df -h

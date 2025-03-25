Questions :

1.  Crée un dossier nommé Exercice_linux
2.  Entrer de ce dossier
3.  Crée deux sous-dossiers : dossier1 et dossier2
4.  Dans dossier1 crée un fichier nommé fichier1.txt
5.  Ajoute le texte « Linux est un système d'exploitation open-source
    basé sur Unix. Linux est reconnu pour sa stabilité, sa sécurité et
    sa flexibilité. De nombreuses distributions Linux existe, adaptées
    aux besoins des utilisateurs » dans fichier1.txt
6.  Vérifie son contenu
7.  Copie fichier1.txt dans dossier2
8.  Renomme le fichier copié en fichier2.txt dans dossier2
9.  Déplace fichier2.txt vers dossier1
10. Vérifie les fichiers présents dans dossier1 et dossier2
11. Recherche le mot « Linux » dans fichier1.txt
12. Compte le nombre de fois qu'il y a la lettre « e »

Réponses :

1.  mkdir exercice_linux
2.  cd exercice_linux
3.  mkdir dossier1 dossier2
4.  touch dossier1/fichier1.txt
5.  echo \" Aujourd'hui nous allons voir Linux\" \>
    dossier1/fichier1.txt
6.  cat dossier1/fichier1.txt
7.  cp dossier1/fichier1.txt dossier2/
8.  mv dossier2/fichier1.txt dossier2/fichier2.txt
9.  mv dossier2/fichier2.txt dossier1/
10. ls
11. grep \"Linux\" dossier1/fichier1.txt
12. 25 « e »

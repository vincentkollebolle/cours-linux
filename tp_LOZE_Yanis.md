TP : Manipulation des Commandes de Base sous Linux

Annexe : commande utile
1.Affichez le manuel d'une commande (exemple : ls) avec man
2.Nettoyez l'écran du terminal avec clear

    Navigation dans le système de fichiers
    1.Ouvrez un terminal et affichez le répertoire courant avec pwd
    2.Créez un nouveau dossier nommé « test_linux » avec mkdir
    3.Déplacez-vous dans ce dossier avec cd
    4.Créez un fichier vide fichier1.txt avec touch
    5.Listez le contenu du dossier avec détails en utilisant ls, utilisez man
    pour trouver l’option
    6.Revenez au dossier parent en utilisant cd

    Manipulation de fichiers
    1.Créez deux fichiers file1.txt et file2.txt dans test_linux avec un seule
    ligne de commande
    2.Copiez file1.txt dans copie_file1.txt avec cp
    3.Renommez file2.txt en renamed_file.txt avec mv

    Lecture et traitement de texte
    1.Créez un fichier avec ecrit « Bonjour Linux » en utilisant echo et un
    operateur de redirection
    2.Affichez son contenu avec cat ou less
    3.Affichez les 2 premières lignes avec head
    4.Affichez la dernière ligne avec tail
    5.Cherchez le mot "Linux" dans le meme fichier avec grep
    6.Remplacez "Bonjour" par "Salut" et affichez le résultat avec sed
    7.Affichez uniquement la première colonne d'un fichier séparé par des
    espaces avec awk

    Redirections et Pipes
    1.Redirigez la sortie d'un ls vers un fichier avec «>»
    2.Ajoutez du texte à ce fichier avec «>>»
    3.Affichez les 5 premières lignes et lisait les avec less grace a «|»
    4.Comptez le nombre de fichiers et dossiers dans le répertoire courant
    grâce a « | » et la commande wc (main wc pour plus d’infos)





    Correction

    TP : Manipulation des Commandes de Base sous Linux

Annexe : Commandes utiles
    1.Affichez le manuel d'une commande (exemple : ls) avec man

     2.Nettoyez l'écran du terminal avec clean

1. Navigation dans le système de fichiers
    1.Ouvrez un terminal et affichez le répertoire courant avec pwd
       pwd
    2.Créez un nouveau dossier nommé « test_linux » avec mkdir
       mkdir test_linux
    3.Déplacez-vous dans ce dossier avec cd
       cd test_linux
    4.Créez un fichier vide fichier1.txt avec touch
       touch fichier1.txt
    5.Listez le contenu du dossier avec détails en utilisant ls, utilisez man
       pour trouver l’option
       ls -l
    6.Revenez au dossier parent en utilisant cd
     cd ..
2. Manipulation de fichiers
    1.Créez deux fichiers file1.txt et file2.txt dans test_linux avec une seule
       ligne de commande
       touch file1.txt file2.txt
    2.Copiez file1.txt dans copie_file1.txt avec cp
       cp file1.txt copie_file1.txt
    3.Renommez file2.txt en renamed_file.txt avec mv
       mv file2.txt renamed_file.txt
3. Lecture et traitement de texte
    1.Créez un fichier avec ecrit «Bonjour Linux» en utilisant echo et un
       operateur de redirection
       echo «Ceci est un fichier Linux» > fichier.txt
    2.Affichez son contenu avec cat ou less
       cat fichier.txt ou less fichier.txt
    3.Affichez les 2 premières lignes avec head
       head -n 2 fichier.txt
    4.Affichez la dernière ligne avec tail
       tail -n 1 fichier.txt
    5.Cherchez le mot "Linux" dans le même fichier avec grep
       grep "Linux" fichier.txt
    6.Remplacez "Bonjour" par "Salut" et affichez le résultat avec sed
       sed 's/Bonjour/Salut/g' fichier.txt
    7.Affichez uniquement la première colonne d'un fichier séparé par des
       espaces avec awk
       awk '{print $1}' fichier.txt
4. Redirections et Pipes
        1.Redirigez la sortie d'un ls vers un fichier avec « > »
       ls > liste_fichiers.txt
        2.Ajoutez du texte à ce fichier avec « >> »
       echo "Texte additionnel" >> liste_fichiers.txt
       3.Affichez les 5 premières lignes et lisez-les avec less grâce à « | »
       head -n 5 liste_fichiers.txt | less
    4.Comptez le nombre de fichiers et dossiers dans le répertoire courant
       grâce à « | » et la commande wc
       ls | wc -l


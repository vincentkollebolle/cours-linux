énoncé

1 trouver un moyen de se localiser depuis la racine
2 créer un dossier « exemple »
3 ecrire du texte en forme de liste en 2 colone dans un fichier « test.txt »
4 afficher le contenu de ce fichier test.txt
5 faire une copie du contenu du fichier dans un deuxieme fichier nommé « test2.txt »
6 afficher la colonne 2 
7 rebalancer la colonne 2 du test2.txt dans le fichier original test.txt
8 supprimer le fichier « test2.txt »

correction

1 pwd, si pas dans la racine faire cd /home/user
2 mkdir exemple
3 touch test.txt, nano test.txt => ecrire les listes de mots
4 ls test.txt
5 cp test.txt > test2.txt
6 awk '{print $2}' test2.txt
7 awk '{print $2}' fichier.txt > test.txt
8 rm -f test2.txt
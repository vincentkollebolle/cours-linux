1) Ecrire bonjour sur la ligne de commande

`echo bonjour  OU echo “bonjour”`

2) Créez un dossier nommé “example”

mkdir example

3) Créez un fichier nommé “blabla.txt” dans le dossier “example”

touch blabla.txt

4) Créez un deuxième fichier nommé “blabla2.txt”

touch blabla2.txt

5) Vérifiez que vos 2 fichiers ont bien été créés

ls

6) Déplacez le fichier “blabla2.txt” vers un sous dossier nommé 
“bonjour”

mkdir bonjour
cp blabla2.txt bonjour/
rm blabla2.txt

7) Dans le fichier “blabla2.txt”, mettre au minimum 2 lignes avec une destination et un prix.
cd bonjour
vim blabla2.txt
i
:wq 

8) Afficher uniquement les prix, puis dans un second temps, les destinations.

awk '{print $2}' blabla2.txt
awk '{print $1}' blabla2.txt

9) Changer une destination

sed ‘s/brest/saint-jean/’ blabla2.txt

10) Copiez les prix et mettez les dans un fichier “prix.txt”

awk '{print $2}' blabla2.txt > prix.txt

11) Faites de même pour les Destination avec un fichier nommé destination.txt

awk '{print $1}' blabla2.txt > destination.txt

12) Créer un fichier noms_des_fichiers.txt avec le nom des fichiers dans le dossier bonjour.

ls bonjour > noms_des_fichiers.txt

13) Lire le fichier noms_des_fichiers.txt d’une autre façon que dans la question

less noms_des_fichiers.txt

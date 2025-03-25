### **Exercice : Gestion de fichiers et manipulation de texte sous Linux**

**Objectif :** Se familiariser avec les commandes Linux pour naviguer
dans le terminal, gérer des fichiers et manipuler du texte.

#### **Étape 1 : Navigation et création de fichiers**

1.  Vérifiez dans quel répertoire vous vous trouvez actuellement.

pwd

1.  Créez un nouveau dossier nommé *exercice_linux* dans votre
    répertoire personnel.

mkdir exercice_linux

1.  Accédez à ce dossier.

cd exercice_linux

1.  Créez un fichier vide nommé *fichier1.txt*.

touch fichier1.txt

1.  Affichez la liste des fichiers du répertoire avec des détails
    supplémentaires.

ls -l

#### **Étape 2 : Manipulation de fichiers et de répertoires**

6.  Ajoutez une phrase dans *fichier1.txt*.

echo \"Bonjour, ceci est un fichier de test.\" \> fichier1.txt

6.  Affichez le contenu de ce fichier.

cat fichier1.txt

6.  Créez un second fichier *fichier2.txt* et copiez-y le contenu du
    premier.

cp fichier1.txt fichier2.txt

6.  Renommez *fichier2.txt* en *backup.txt*.

mv fichier2.txt backup.txt

6.  Créez un sous-dossier nommé *archives* et déplacez *backup.txt*
    dedans.

mkdir archives

mv backup.txt archives/

6.  Affichez de nouveau la liste des fichiers et dossiers du répertoire.

ls -l

#### **Étape 3 : Manipulation de texte**

12. Ajoutez plusieurs lignes dans *fichier1.txt*, dont une contenant le
    mot \"Linux\".

echo \"Deuxième ligne\" \>\> fichier1.txt

echo \"Troisième ligne avec un mot clé : Linux\" \>\> fichier1.txt

12. Recherchez les lignes contenant le mot \"Linux\".

grep \"Linux\" fichier1.txt

12. Affichez uniquement la deuxième colonne du fichier, en considérant
    que les mots sont séparés par des espaces.

awk \'{print \$2}\' fichier1.txt

12. Remplacez le mot \"Bonjour\" par \"Salut\" dans *fichier1.txt*.

sed -i \'s/Bonjour/Salut/\' fichier1.txt

12. Affichez le contenu du fichier ligne par ligne de manière
    interactive.

less fichier1.txt

#### **Étape 4 : Commandes diverses**

17. Effacez le contenu affiché dans le terminal.

clear

17. Consultez la documentation d'une commande permettant d'afficher les
    fichiers d'un dossier.

man ls

17. Supprimez le fichier *fichier1.txt*.

rm fichier1.txt

17. Supprimez le dossier *archives* ainsi que son contenu.

rm -r archives

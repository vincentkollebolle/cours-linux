Exercice Piya pour Alernes
o Crée un dossier appelé Mon_Projet
o Entre dans ce dossier
o Crée un fichier notes.txt
o Écris "Je suis en premier année dans informatique" dedans
o Affiche son contenu
o Copie notes.txt en notes_backup.txt
o Renomme notes_backup.txt en sauvegarde.txt
o Affiche la liste des fichiers dans Mon_Projet
o Trouve quel fichier contient le mot "premier"
o Crée un dossier Backup
o Déplace sauvegarde.txt dans Backup
o Affiche le chemin complet de ton dossier actuel
Question bonus
Comment afficher seuleent les 3 premières lignes d’un fichier?
Comment supprimer le fichier notes.txt?

Correction
Créer un dossier et des fichiers

cd ~ # Se place dans le dossier personnel
mkdir Mon_Projet # Crée le dossier "Mon_Projet"
cd Mon_Projet # Entre dans ce dossier
Créer et remplir un fichier texte
touch notes.txt # Crée le fichier
echo " Je suis en premier année dans informatique ." > notes.txt # Écrit dedans
cat notes.txt # Affiche le contenu
Copier et renommer un fichier
cp notes.txt notes_backup.txt # Copie le fichier
mv notes_backup.txt sauvegarde.txt # Renomme la copie
Lister et chercher des fichiers
ls # Liste les fichiers (doit afficher notes.txt et sauvegarde.txt)
grep "premier" * # Cherche le mot "premier" dans tous les fichiers
Créer un sous-dossier et déplacer un fichier
mkdir Backup # Crée le dossier Backup
mv sauvegarde.txt Backup/ # Déplace le fichier dedans
Vérifier où tu es
pwd # Affiche le chemin complet (ex: /home/votre_user/Mon_Projet)
Correction questions bonus

head -n 3 notes.txt
rm notes.txt

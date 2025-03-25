Exercice Alernes pour Piyathad

Contexte : Vous êtes administrateur système et devez organiser, analyser et manipuler
des fichiers dans un dossier Projet.

1. Préparation de l'environnement
- Créez un dossier Projet dans votre répertoire personnel (~/Projet).
- Dans Projet, créez 3 sous-dossiers : Docs, Data, Backup.
2. Création et copie de fichiers
- Dans Docs, créez 5 fichiers .txt nommés fichier1.txt à fichier5.txt.
- Écrivez "Ceci est le fichier X" dans chaque fichier (remplacez X par le numéro du
fichier).
- Copiez tous les fichiers .txt dans Backup.
3. Recherche et filtrage
- Trouvez tous les fichiers .txt dans Projet et enregistrez leur liste dans un
fichier liste_fichiers.txt dans Data.
- Utilisez grep pour trouver les fichiers contenant le mot "fichier 3" et sauvegardez
le résultat dans resultat_grep.txt.
4. Manipulation de texte avec awk
- Créez un fichier notes.csv dans Data avec le contenu suivant :

Copy

Nom,Note

Alice,

Bob,

Charlie,

David,

Utilisez awk pour afficher uniquement les noms des étudiants ayant une note
supérieure à 14.
5. Renommage et déplacement
Renommez fichier5.txt en important.txt dans Docs.
Déplacez important.txt dans Backup.
6. Affichage et navigation
Affichez le contenu de resultat_grep.txt avec less.
Utilisez cat pour concaténer fichier1.txt et fichier2.txt dans un nouveau
fichier fusion.txt dans Data.
7. Vérification des chemins
Affichez le chemin absolu du dossier Backup avec pwd et enregistrez-le
dans chemin_backup.txt.
8. Suppression et recréation
Supprimez tous les fichiers .txt dans Docs sauf fichier1.txt.
Recréez fichier4.txt avec touch.
9. Options avancées de ls
Affichez la liste des fichiers de Projet triés par date de modification (du plus
récent au plus ancien).
Affichez les fichiers cachés dans votre répertoire personnel.
10. Redirection et echo
Utilisez echo pour ajouter "Fin de l'exercice" à la fin de fusion.txt.
11. Bonus : Recherche récursive
Trouvez tous les fichiers .txt modifiés dans les dernières 24 heures sous Projet.
12. Bonus : Scripting rapide
Écrivez une commande qui compte le nombre de lignes de chaque
fichier .txt dans Backup et enregistre le résultat dans stats.txt.
Correction :

mkdir -p ~/Projet/{Docs,Data,Backup}
touch ~/Projet/Docs/fichier{1..5}.txt + echo "Ceci est le fichier X" >
fichierX.txt (pour chaque fichier)
find ~/Projet -name "*.txt" > ~/Projet/Data/liste_fichiers.txt
grep "fichier 3" ~/Projet/Docs/*.txt > ~/Projet/Data/resultat_grep.txt
awk -F',' '$2 > 14 {print $1}' ~/Projet/Data/notes.csv
mv ~/Projet/Docs/fichier5.txt ~/Projet/Docs/important.txt puis mv
~/Projet/Docs/important.txt ~/Projet/Backup/
less ~/Projet/Data/resultat_grep.txt
cat ~/Projet/Docs/fichier{1,2}.txt > ~/Projet/Data/fusion.txt
pwd > ~/Projet/Data/chemin_backup.txt (exécuté depuis Backup)
ls -lt ~/Projet et ls -a ~
echo "Fin de l'exercice" >> ~/Projet/Data/fusion.txt
find ~/Projet -name "*.txt" -mtime - 1
wc -l ~/Projet/Backup/*.txt > ~/Projet/Data/stats.txt

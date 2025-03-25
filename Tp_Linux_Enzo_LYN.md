# Exercice Linux : Manipulation Ultra-Avancée de Fichiers et Données

## Étape 1 : Création de l’environnement de travail

1. Crée un dossier nommé `projet_linux` et assure-toi qu’il a des permissions restrictives.
2. À l’intérieur de `projet_linux`, crée quatre sous-dossiers : `docs`, `logs`, `archives`, et un dossier caché `.config`.
3. Fais en sorte que seul un utilisateur spécifique ait un accès complet à `projet_linux`.
4. Utilise une commande pour générer une arborescence des dossiers et fichiers de `projet_linux` et consigne-le dans un fichier, avec des informations sur les droits d'accès.
5. Utilise `find` pour rechercher un dossier contenant des fichiers de plus de 1 Mo. Sauvegarde cette recherche dans un fichier texte.

## Étape 2 : Création et modification de fichiers

6. Dans `docs`, crée des fichiers dont les noms sont générés aléatoirement avec un format horaire.
7. Insère du texte dynamique dans ces fichiers, mais crée des variations dans le texte en utilisant des variables environnementales ou des données système (date, utilisateur courant, hostname).
8. Utilise des outils comme `seq` ou `shuf` pour insérer des lignes dans un fichier, mais de manière à générer un contenu qui varie en fonction de paramètres externes (comme l’heure du jour).
9. Automatise l'ajout de texte dans ces fichiers en créant un petit script qui crée une nouvelle ligne toutes les 5 secondes, mais dans des fichiers différents à chaque itération.

## Étape 3 : Organisation et gestion des fichiers

10. Effectue une copie incrémentale des fichiers dans `docs` vers `archives`, de manière à ne copier que ceux modifiés après une date donnée, mais en prenant soin de préserver leurs permissions et attributs.
11. Déplace aléatoirement certains fichiers dans `docs` vers `logs`, en utilisant un script qui choisit ces fichiers en fonction de critères dynamiques (par exemple, fichiers de plus de 100 lignes, ou ceux créés à une heure spécifique).
12. Renomme tous les fichiers dans `docs` en ajoutant un préfixe horaire ou un suffixe unique basé sur des propriétés système (comme le nom d'utilisateur ou l'adresse IP).

## Étape 4 : Recherche et analyse

13. Affiche les fichiers dans un dossier, mais trie-les d'abord par extension et ensuite par taille décroissante.
14. Recherche un mot spécifique dans un fichier, mais exclut les occurrences qui apparaissent dans les lignes commençant par une date. Sauvegarde les résultats dans un fichier de log détaillant les résultats.
15. Affiche les 10 premières lignes d’un fichier après avoir filtré les commentaires, et affiche aussi un compte des lignes supprimées.
16. Cherche et affiche les lignes contenant des nombres au format spécifique (par exemple, décimaux, hexadécimaux, etc.), mais sans afficher les doublons.

## Étape 5 : Manipulation avancée de fichiers texte

17. Effectue une opération de remplacement dans plusieurs fichiers à la fois en excluant certains fichiers basés sur leur taille (par exemple, ne remplace que dans les fichiers dont la taille est inférieure à 500 octets).
18. Divise les lignes d'un fichier en colonnes multiples basées sur des délimiteurs spécifiques (espaces, tabulations, virgules, etc.) et manipule ces données avant de les réécrire dans un autre fichier.
19. Crée un fichier de log qui enregistre l'ensemble des fichiers modifiés, avec des informations détaillées sur chaque modification (nom du fichier, ligne modifiée, ancien et nouveau contenu).
20. Réorganise l’ordre des colonnes dans chaque fichier texte mais applique un filtre pour ne conserver que les colonnes avec des données numériques. Enregistre les résultats dans un fichier de sortie.

## Étape 6 : Téléchargement et extraction de données

21. Télécharge un fichier texte depuis un serveur FTP sécurisé avec authentification, et place-le dans `archives`, tout en appliquant des permissions strictes à ce fichier.
22. Filtre et extrait des lignes spécifiques d'un fichier téléchargé en fonction de plusieurs critères dynamiques (par exemple, ligne contenant des chiffres, mais pas des dates).
23. Ajoute un numéro de ligne au début de chaque ligne du fichier filtré, mais uniquement pour les lignes qui ne sont pas vides ou commentées.

## Étape 7 : Fusion et Formatage

24. Fusionne plusieurs fichiers texte tout en supprimant les doublons, mais conserve la structure d’origine des fichiers. Trie ensuite les résultats par ordre croissant de longueur de ligne.
25. Supprime toutes les lignes vides d'un fichier, mais vérifie les sections de chaque fichier avant pour éviter de supprimer des lignes contenant uniquement des espaces.

## Étape 8 : Nettoyage et suppression sécurisée

26. Déplace tous les fichiers modifiés dans `archives`, mais avant cela, compresse-les en format `.tar.gz` tout en ajoutant une timestamp à chaque fichier compressé.
27. Supprime proprement les fichiers temporaires en utilisant une méthode de suppression sécurisée, et vérifie qu'ils ne peuvent pas être récupérés avec des outils comme `testdisk`.
28. Vérifie l’intégrité du système après chaque suppression pour t’assurer qu’il n'y a pas de fichiers résiduels ou de corruption.

## Étape 9 : Sécurisation et Permissions

29. Change les permissions sur `docs`, `logs` et `archives` pour que seuls certains groupes d’utilisateurs (et non les utilisateurs individuels) puissent y accéder, en créant des groupes spécifiques.
30. Active l’audit des fichiers modifiés pour tous les fichiers dans `docs` et `logs`, puis génère un rapport complet des modifications effectuées (ajout, suppression, modification).

## Étape 10 : Automatisation et Monitoring

31. Crée un script de surveillance qui enregistre toutes les actions effectuées dans `projet_linux` (modifications de fichiers, création de fichiers, changements de permissions), et qui envoie un résumé des activités à un administrateur.
32. Automatise la création d'un rapport mensuel de l’usage des fichiers dans `projet_linux`, en incluant des statistiques comme la fréquence de modification, l’utilisation d’espace disque, et le nombre de fichiers créés.

## Objectif final

Construire un environnement de fichiers sécurisé, audité, et automatisé, où les utilisateurs doivent avoir un contrôle précis sur les permissions et la gestion des données, tout en optimisant l'efficacité des manipulations avec des outils et scripts.


# Correction de l'Exercice Linux : Manipulation Ultra-Avancée de Fichiers et Données

## Étape 1 : Création de l’environnement de travail

1. **Création du dossier projet_linux :**
    - Commande : `mkdir projet_linux`
    - Vérification : Utilise `ls -l` pour vérifier l’existence et les permissions du dossier. Donne un accès complet à l’utilisateur uniquement.
   
2. **Création des sous-dossiers docs, logs, archives et .config :**
    - Commande : 
      ```bash
      mkdir projet_linux/docs projet_linux/logs projet_linux/archives projet_linux/.config
      ```
    - Vérification : Utilise `ls -l` pour lister le contenu et s'assurer de la structure.

3. **Permissions restrictives sur projet_linux :**
    - Commande : `chmod 700 projet_linux`
    - Explication : Cela signifie que seul l’utilisateur courant peut lire, écrire et exécuter dans ce dossier.

4. **Générer l’arborescence avec les droits d'accès :**
    - Commande : `find projet_linux -type d -exec ls -ld {} \; > projet_linux/structure.txt`
    - Explication : Cette commande génère un fichier texte qui contient l’arborescence des dossiers et leurs permissions.

5. **Recherche de dossiers contenant des fichiers de plus de 1 Mo :**
    - Commande : `find projet_linux -type f -size +1M`
    - Explication : Cette commande cherche les fichiers de plus de 1 Mo et renvoie leur chemin.

## Étape 2 : Création et modification de fichiers

6. **Création des fichiers avec des noms aléatoires :**
    - Commande :
      ```bash
      touch projet_linux/docs/$(date +%Y-%m-%d_%H-%M-%S)_file1.txt
      touch projet_linux/docs/$(date +%Y-%m-%d_%H-%M-%S)_file2.txt
      touch projet_linux/docs/$(date +%Y-%m-%d_%H-%M-%S)_file3.txt
      ```
    - Explication : Le nom des fichiers intègre la date et l'heure actuelles, garantissant leur unicité.

7. **Insertion de texte dynamique dans ces fichiers :**
    - Commande :
      ```bash
      echo "Date: $(date)" > projet_linux/docs/$(date +%Y-%m-%d_%H-%M-%S)_file1.txt
      echo "User: $(whoami)" >> projet_linux/docs/$(date +%Y-%m-%d_%H-%M-%S)_file2.txt
      echo "Host: $(hostname)" >> projet_linux/docs/$(date +%Y-%m-%d_%H-%M-%S)_file3.txt
      ```
    - Explication : Le texte inséré varie en fonction des variables système comme la date, l'utilisateur et l’hôte.

8. **Insertion de lignes aléatoires avec shuf :**
    - Commande :
      ```bash
      shuf -i 1-1000 -n 50 >> projet_linux/docs/$(date +%Y-%m-%d_%H-%M-%S)_file1.txt
      ```
    - Explication : Cette commande insère 50 lignes aléatoires allant de 1 à 1000 dans le fichier spécifié.

9. **Automatisation de l'ajout de lignes toutes les 5 secondes :**
    - Script :
      ```bash
      while true; do echo "Random line $(date)" >> projet_linux/docs/$(date +%Y-%m-%d_%H-%M-%S)_file1.txt; sleep 5; done
      ```
    - Explication : Ce script ajoute une ligne toutes les 5 secondes dans un fichier donné.

## Étape 3 : Organisation et gestion des fichiers

10. **Copie incrémentale vers archives :**
    - Commande : `rsync -av --ignore-existing projet_linux/docs/ projet_linux/archives/`
    - Explication : `rsync` permet de copier les fichiers modifiés vers `archives` sans copier les fichiers déjà présents.

11. **Déplacement aléatoire de fichiers vers logs :**
    - Script :
      ```bash
      files=( $(ls projet_linux/docs) )
      mv projet_linux/docs/${files[$RANDOM % ${#files[@]}]} projet_linux/logs/
      ```
    - Explication : Ce script déplace aléatoirement un fichier de `docs` vers `logs`.

12. **Renommage des fichiers avec un préfixe basé sur la date :**
    - Commande :
      ```bash
      for file in projet_linux/docs/*; do mv "$file" "$(date +%Y-%m-%d)_$file"; done
      ```

## Étape 4 : Recherche et analyse

13. **Affichage trié des fichiers par extension et taille :**
    - Commande : `find projet_linux -type f -exec ls -l {} \; | sort -t. -k2,2 -k5,5n`
    - Explication : Trie d’abord par extension, puis par taille.

14. **Recherche d’un mot spécifique avec exclusion de dates :**
    - Commande : `grep -v "^\$(date +%Y-%m-%d)" projet_linux/docs/* | grep "mot_clé"`
    - Explication : Cette commande exclut les lignes commençant par la date actuelle avant de chercher le mot-clé.

15. **Affichage des 10 premières lignes après filtrage des commentaires :**
    - Commande : `grep -v "^#" projet_linux/docs/* | head -n 10`

16. **Recherche de lignes contenant des nombres spécifiques :**
    - Commande : `grep -E '\b[0-9]+\b' projet_linux/docs/* | sort -n`

## Étape 5 : Manipulation avancée de fichiers texte

17. **Remplacement d’un mot spécifique dans plusieurs fichiers :**
    - Commande :
      ```bash
      find projet_linux/docs -type f -exec sed -i 's/ancien_mot/nouveau_mot/g' {} \;
      ```
    - Explication : Remplace un mot dans tous les fichiers de `docs`.

18. **Division des lignes en plusieurs colonnes :**
    - Commande :
      ```bash
      awk '{print $1, $3}' projet_linux/docs/file1.txt > projet_linux/docs/columns_output.txt
      ```

19. **Création d'un fichier log des modifications :**
    - Script :
      ```bash
      for file in projet_linux/docs/*; do
      echo "Modification: $(date) in file $file" >> projet_linux/logs/modifications.log
      done
      ```

20. **Réorganisation des colonnes :**
    - Commande :
      ```bash
      awk '{print $2, $1}' projet_linux/docs/file1.txt > projet_linux/logs/reordered_file.txt
      ```

## Étape 6 : Téléchargement et extraction de données

21. **Téléchargement depuis un FTP sécurisé :**
    - Commande : 
      ```bash
      wget --ftp-user=USERNAME --ftp-password=PASSWORD ftp://example.com/file.txt -P projet_linux/archives/
      ```

22. **Filtrage et extraction des lignes spécifiques :**
    - Commande : 
      ```bash
      grep "mot_clé" projet_linux/archives/file.txt > projet_linux/logs/filtered_file.txt
      ```

23. **Ajout de numéro de ligne pour le fichier filtré :**
    - Commande : 
      ```bash
      nl projet_linux/logs/filtered_file.txt > projet_linux/logs/numbered_filtered.txt
      ```

## Étape 7 : Fusion et Formatage

24. **Fusion de fichiers en supprimant les doublons et tri par taille :**
    - Commande : 
      ```bash
      cat projet_linux/docs/* | sort -u > projet_linux/logs/merged_sorted.txt
      ```

25. **Suppression des lignes vides et rapport de suppression :**
    - Commande : 
      ```bash
      grep -v '^\[\[:space:\]\]*$' projet_linux/docs/file1.txt > projet_linux/logs/cleaned_file.txt
      ```

🗑 **Étape 8 : Nettoyage et suppression sécurisée**

26. **Déplacement et compression des fichiers modifiés :**
    - Commande :
      ```bash
      tar -czf projet_linux/archives/files_backup_$(date +%Y-%m-%d).tar.gz projet_linux/docs/*
      ```

27. **Suppression sécurisée avec shred :**
    - Commande : `shred -u projet_linux/docs/file1.txt`

## Étape 9 : Sécurisation et Permissions

28. **Modification des permissions avec chmod :**
    - Commande : 
      ```bash
      chmod 750 projet_linux/docs
      chown root:admin projet_linux/docs
      ```

29. **Audit des fichiers modifiés avec auditd :**
    - Commande : `auditctl -w projet_linux/docs -p wa`
    - Explication : Enregistre les modifications sur `docs`.

## Étape 10 : Automatisation et Monitoring

30. **Création d’un script de surveillance :**
    - Script :
      ```bash
      while true; do
      inotifywait -r -e modify,create,delete projet_linux/
      echo "Changement détecté à $(date)" >> projet_linux/logs/activity.log
      done
      ```

31. **Automatisation d’un rapport mensuel :**
    - Commande : Utilise `cron` pour planifier l'exécution du script de rapport.

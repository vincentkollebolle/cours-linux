Exercice Linux :
 Manipulation Avancée de Fichiers et Données
 Tu vas devoir créer, organiser, manipuler et transformer des fichiers texte en utilisant
 uniquement le terminal. Cet exercice demandera d'explorer des commandes avancées
 et de chercher par toi-même les solutions.

 Étape 1 : Création de l’environnement de travail
    1. Crée un dossier nommé projet_linux et place-toi dedans.
    2. À l’intérieur, crée trois sous-dossiers : docs, logs et archives.
 Étape 2 : Création et modification de fichiers
    3. Dans docs, crée trois fichiers texte avec des noms différents.
    4. Ajoute du texte dans chacun des fichiers avec une commande permettant
        d’écrire du contenu sans ouvrir un éditeur.
 Étape 3 : Organisation et gestion des fichiers
    5. Copie un des fichiers vers le dossier archives.
    6. Déplace un autre fichier du dossier docs vers logs.
    7. Renomme le dernier fichier restant dans docs.
 Étape 4 : Recherche et analyse
    8. Affiche uniquement les fichiers d’un dossier avec leurs tailles.
    9. Recherche un mot spécifique dans un des fichiers et affiche les lignes
        correspondantes.
    10.Affiche uniquement les 5 premières lignes d’un fichier.
    11.Affiche uniquement les 3 dernières lignes d’un fichier.
 Étape 5 : Manipulation avancée de fichiers texte
    12.Affiche uniquement la deuxième colonne d’un fichier texte contenant des mots
        et nombres séparés par des espaces.
    13.Affiche les lignes contenant un nombre supérieur à une valeur donnée (par
        exemple, supérieur à 50).
    14.Inverse l’ordre des colonnes de chaque ligne du fichier et enregistre le résultat
        dans logs/resultat1.txt.
    15.Remplace un mot spécifique par un autre dans un fichier et enregistre le
        résultat dans logs/resultat2.txt.
    16.Supprime les lignes contenant un mot précis et enregistre dans un nouveau
        fichier.
 Étape 6 : Téléchargement et extraction de données
    17.Télécharge un fichier texte depuis internet et place-le dans archives.
    18.Filtre uniquement les lignes contenant un mot-clé et enregistre-les dans un
        nouveau fichier.
    19.Ajoute un numéro de ligne au début de chaque ligne du fichier filtré.
 Étape 7 : Fusion et Formatage
    20.Fusionne deux fichiers texte en un seul, en triant les lignes par ordre
        alphabétique.
    21.Supprime toutes les lignes vides d’un fichier.
🗑 Étape 8 : Nettoyage et suppression sécurisée
    22.Déplace les fichiers modifiés dans archives.
    23.Supprime proprement les fichiers temporaires sans possibilité de
        récupération. 

> **Correction** **de** **l'Exercice** **Linux** **:** **Manipulation**
> **Avancée** **de** **Fichiers** **et** **Données**
>
> **Étape** **1** **:** **Création** **de** **l’environnement** **de**
> **travail**

mkdir projet_linux && cd projet_linux

mkdir docs logs archives

> **Étape** **2** **:** **Création** **et** **modification** **de**
> **fichiers**

touch docs/fichier1.txt docs/fichier2.txt docs/fichier3.txt

echo "Première ligne de texte" \> docs/fichier1.txt

echo "Deuxième fichier avec un texte différent" \> docs/fichier2.txt

echo "Troisième fichier avec un autre texte" \> docs/fichier3.txt

> **Étape** **3** **:** **Organisation** **et** **gestion** **des**
> **fichiers**

cp docs/fichier1.txt archives/

mv docs/fichier2.txt logs/

mv docs/fichier3.txt docs/fichier_renomme.txt

> **Étape** **4** **:** **Recherche** **et** **analyse**

ls-lh docs logs archives \# Afficher les fichiers avec leurs tailles

grep "texte" docs/fichier_renomme.txt \# Recherche un mot spécifique

head-n 5 docs/fichier_renomme.txt \# Afficher les 5 premières lignes

tail-n 3 docs/fichier_renomme.txt \# Afficher les 3 dernières lignes

> **Étape** **5** **:** **Manipulation** **avancée** **de** **fichiers**
> **texte**

**Création** **d’un** **fichier** **contenant** **des** **colonnes**
**de** **texte** **et** **nombres**

echo -e "Alice 25\nBob 30\nCharlie 55\nDavid 12\nEmma 60" \>
docs/donnees_brutes.txt

**Extraction** **de** **la** **deuxième** **colonne**

awk '{print \$2}' docs/donnees_brutes.txt

**Affichage** **des** **lignes** **contenant** **un** **nombre**
**supérieur** **à** **50**

awk '\$2 \> 50' docs/donnees_brutes.txt

**Inversion** **des** **colonnes** **et** **sauvegarde**

awk '{print \$2, \$1}' docs/donnees_brutes.txt \> logs/resultat1.txt

**Remplacement** **d’un** **mot** **spécifique**

sed 's/Charlie/Charlotte/g' docs/donnees_brutes.txt \>
logs/resultat2.txt

**Suppression** **des** **lignes** **contenant** **"David"**

grep-v "David" docs/donnees_brutes.txt \> logs/sans_david.txt

> **Étape** **6** **:** **Téléchargement** **et** **extraction** **de**
> **données**

wget-O archives/data.txt https://www.gutenberg.org/files/1342/1342-0.txt
\# Exemple : "Pride and Prejudice"

grep "Elizabeth" archives/data.txt \> logs/elizabeth.txt

awk '{for (i=NF; i\>0; i--) printf "%s ", \$i; print ""}'
logs/elizabeth.txt \> logs/elizabeth_inverse.txt

nl logs/elizabeth_inverse.txt \> logs/elizabeth_num.txt

> **Étape** **7** **:** **Fusion** **et** **Formatage**

cat logs/resultat1.txt logs/resultat2.txt \| sort \> logs/fusionne.txt

sed-i '/^\$/d' logs/fusionne.txt \# Suppression des lignes vides

🗑 **Étape** **8** **:** **Nettoyage** **et** **suppression**
**sécurisée**

mv logs/\*.txt archives/

rm-rf logs

shred-u archives/sans_david.txt \# Suppression sécurisée

> **Tout** **est** **structuré** **et** **propre,** **mission**
> **accomplie** **!**
